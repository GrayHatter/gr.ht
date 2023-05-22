+++
layout = "post"
title = "Your adversary will gaze back"
email = "gaze"
date = 2023-05-17
tags = ["data", "on-topic"]

# summary = """"""
+++

There's a corollary to one of my favorite memes

> You either die in alpha; or live long enough to see yourself implement content
> moderation.

It goes something like, 'When you gaze into the adversary, the adversary will
gaze back.' I could quickly give a few dozen translations for this aphorism I
just made up; but in opposition to my normal style of never ending rant. I'll
make an attempt to stick to a single meaning.

Obviously, for any service, there will eventually be a group of malcontents
willing to play a negative sum game. Thus InfoSec was born. Made up of that very
rare breed of engineers, security engineers, who's job it is to figure out what
the baddies are doing, and make them stop. Among this select group, the people
who are normally the best at this job are unsurprisingly hackers. The whole
takes one to know one works especially well when talking scenarios outside of
what's normally expected. Reverse engineering some system to make it do
something it's not is the specialty of hackers after all. And thus the players,
on both sides of this fence are hackers. Again, unsurprisingly, people who love
this are the best at it. They do it because they love it, they will take any
opportunity to do it. Which means, they don't go home at the end of the day, nor
will they pick up a different project for that sweet sweet performance review
credit.

That could just as easily be reduced to; hackers gonna keep hacking. (wow, I'm
bad at this not ranting thing...) What's secure today, is vulnerable tomorrow.
The mitigations that worked today, get defeated tomorrow. ...Or rather, the
mitigations built in [[checks
notes]](https://en.wikipedia.org/wiki/Firefox_version_history#Firefox_91_through_101p)
a long time ago[^ff92], just make it easier for the bad guys to hide from you.

[^ff92]: Firefox 92 was released on September 7, 2021

As a security engineer, you have to be good at everything! And by good at
everything I mean good enough to understand the first 20%. This time, we're
talking about UX, if you want to have a good user experience, you have to
remember who you're designing systems for. When security is designing systems,
they're building them for hackers, unfortunately for the ones who want to use
your own services against you. You'll never hear me advocate for security
through obscurity, but it's still critical that you understand **exactly** what
information you're leaking, or more importantly, how that information will be
used against you. While it's a toss up if someone's gonna find or look at any
one of your surfaces, it's almost guaranteed that someone will be looking at the
security systems or mitigations you create.

The same goes for when you decide it's better to lie. First, don't lie. I say
that for security systems and services for all the same reasons everyone else
says it about conversations or relationships[^al0][^fn][^al1][^gw][^vr]. One of
them is so good, that it even gets quoted in line!

> If you tell the truth, you don't have to remember anything.

-- Mark Twain

I'm pretty sure that's just a typo, and what he meant to say is: "If you tell
the truth, you never have to maintain any of the code you wrote." -- Mark Twain

But, I'm not naive enough to think you can always tell the truth and win. So...
when you are forced to lie, you'd better make sure your lie is believable. If
you don't you're just giving out better signal to doxx yourself. Then, and this
is the important part. **You have to remember the lie!** From now on, in
everything you do, the lie must be real. Because once you get caught, that lie,
and any other lie that looks like it, will never work again. And now they know.
Which means now they're looking.

Now it just got complicated, what outside the lie are they looking for?
Unfortunately, everything. If they've figured out your lie, you've given them
your fingerprint. They can study every loop and whorl, and arch[^fprint]. Were
they able to enumerate the entire IP set? Probably doesn't matter if you're
using a single well built data center.

    $ whois $IPADDR

    [ ... ]
    NetName:        GOOGLE-CLOUD
    [ ... ]
    Comment:        *** The IP addresses under this Org-ID are in use by Google Cloud customers ***

That datacenter will helpfully announce itself as *[not a real user]*. Which
just gives them an easy way to serve your "Shady Context ID Service"⟨™⟩ a
different file then they serve your users.

[^fprint]: https://www.forensicsciencesimplified.org/prints/principles.html

But before you exclaim that, "I can't just use my real UA:[^realua]

[^realua]: Mozilla/5.0 (compatible; <span style="color: black;
    background-color:black" title="No, this is actually redacted, but nice try
    :)">[REDACTED]</span>/2.0; +https://<span style="color: black;
    background-color:black" title="No, this is actually redacted, but nice try
    :)">[REDACTED]</span>.com)

Despite my warning about lying, I wouldn't actually suggest telling the truth
here. I'm suggesting that you have to lie better. Select from a random set of
real user agents that are actually using your app right now. Write some code to
keep that list always up to date. The moral of the story is: pay close attention
to the amount of information you're leaking. Leak as little as possible, and
if you want extra points. Mix in a bit of noise into your signal. The harder it
is to doxx your security services, the longer it'll take before they break them.

Bonus tip: Be careful of the company you keep. It doesn't do any good to try to
obscure who you really are, if your friend always follows you everywhere you go.

```
127.0.0.1 - [2023-05-17 18:14:10] gr.ht "GET /assets/wtfit.gif HTTP/1.1" 200 917653 "Mozilla/5.0 (compatible; [REDACTED]/2.0; +https://[REDACTED].com)" "-"
127.0.0.1 - [2023-05-17 18:14:10] gr.ht "GET /assets/wtfit.gif HTTP/1.1" 200 917653 "Mozilla/5.0 (Macintosh; Intel Mac OS X 11.6; rv:92.0) Gecko/20100101 Firefox/92.0" "-"
```

TIL: The Trust and Safety team at <span style="color: black;
background-color:black" title="">[COMPANY]</span> uses Firefox on a Mac book...
Interesting...


[^al0]: *“No man has a good enough memory to be a successful liar”* -- Abraham
    Lincoln

[^fn]: *“I'm not upset that you lied to me, I'm upset that from now on I can't
    believe you.”* -- Friedrich Nietzsche

[^al1]: *“You can fool some of the people all of the time, and all of the people
    some of the time, but you can not fool all of the people all of the time.”*
    -- Abraham Lincoln

[^gw]: *“It is better to offer no excuse than a bad one.”* -- George Washington

[^vr]: *“Lies require commitment.”* ― Veronica Roth, Divergent

[^ua]: Mozilla/5.0 (Macintosh; Intel Mac OS X 11.6; rv:92.0) Gecko/20100101 Firefox/92.0
