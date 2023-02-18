---
layout: post
title:  "It seemed like a good idea at the time..."
date:   2019-06-09
tags: at-the-time
---
Context: While working on wifi functionality for HUDTDS (heads up display that doesn't suck), because `iw` warns not to
screen scrape, I looked into exactly how it works and learned about a cool thing you can do. Because I've never seen
anything like this, I thought it was interesting.

Have you ever wanted to add a series of structs to your application, but enumerating them all in a single location
seems like way too much work? Well you're in luck! There's a GNU extension that allows you to create your own named
object segments. Anything you declare with `__attribute__ (( segment("__named") ))` will be stored in it's own segment.
Doing it this way you can simply define whatever data you want, each in it's own self-contained file.

I'm sure you're wondering, "If all this data is only declared in a single file, how would you access it at all?" That's
why we named it. So that anywhere you want to access the data, include `extern struct my_struct __start___named;`
You'll have to calculate the size offset at runtime, but that's simple enough. Add an empty file that adds a two dummy
entries, (in our case we'll use `__section_[set/get]`) to the segment, then the absolute of
`__section_set - __section_get` will get you the offset size. Then you can write a for loop that adds the offset size.
Be very careful not to increment the pointer by the struct size, as the size of the struct may not be the size you need
to seek for each iteration.

Also, because each of these objects need to be stored in a shared segment, but without the other files knowing about
each other; you'll need to make sure each struct has it's own *unique* name. The other files not being allowed to know
about each other means the compiler might think some of these structs aren't actually used, and will try to optimize
them out for you. This is obviously not what you want, so be sure to include an `__attribute__ (( used ))` as well.

All of this is starting to get a little complicated, so it's time to write a macro! This is what the one in `iw` looks
like. https://git.kernel.org/pub/scm/linux/kernel/git/jberg/iw.git/tree/iw.h#n107

```c
#define __COMMAND(_section, _symname, _name, _args, _nlcmd, _flags, _hidden, _idby, _handler, _help)\
    static struct cmd                       \
    __cmd ## _ ## _symname ## _ ## _handler ## _ ## _nlcmd ## _ ## _idby ## _ ## _hidden\
    __attribute__((used)) __attribute__((section("__cmd"))) = { \
        .name = (_name),                    \
        .args = (_args),                    \
        .cmd = (_nlcmd),                    \
        .idby = (_idby),                    \
        .handler = (_handler),                  \
        .help = (_help),                    \
        .parent = _section,                 \
     }
```

If you can't remember all of this, or are in a hurry, or are tired of explaining every little detail during code review
you could use a command array. [This one](https://git.sr.ht/~emersion/mrsh/tree/master/builtin/builtin.c#L9-42) in
`mrsh` is *an* example. But doing it that way you'd need a
[header file](https://git.sr.ht/~emersion/mrsh/tree/master/include/builtin.h#L11-34) too.

But that way is boring, now that you know you can create your own object segments whenever you want to, you can do so
many more cool things!

"It's probably better that you don't know that unless you're a kernel hacker" -- [ddevault](https://drewdevault.com/)

P.S.: I thought it went without saying but please, **don't** do this. Always prefer simplicity over... editing multiple
files.

P.P.s. Dear `iw` guys, this is tongue in cheek, I love you guys. Without your work I wouldn't be working on replacing
the *actually* bad software on my car.
