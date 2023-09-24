+++
layout = "post"
title = "Keep Yourself Drain Ready"
email = "drainready"
date = 2023-08-08
lastmod = 2023-09-24
draft = false
tags = ["off-topic", "balance", "human"]


summary = """You have a direct personal, professional, and ethical
responsibility to keep yourself drain ready at all times.""" 

+++

I used to work for a big data company. One of the responsibilities I had, was to
help ensure the availability of all of our services. My individual slice was a
very narrow subset of what could be considered the prime directive for my org as
a whole.

> Keep the site up.

So critical was this one directive, in what seemed to be daily drills, someone
would turn off one of the many data centers, and route all that traffic to the
other data centers. One of the critical prerequisites of these tests, was the
constant maintenance of the excess buffer of global capacity and availability.
Any violation or loss of this buffer immediately became an internal incident,
one that would get managed as an emergency, and then would complete the incident
review process. There didn't need to be any noticeable symptoms, or degradation
of the services. Merely the loss of the buffer became its own incident.

The buffer size for us was `$CAPACITY_LARGEST_DC + $TOTAL_GLOBAL_CAPACITY * 7%`.
That was the line in the sand we drew to keep the site "drain ready". But,
that's *our* bar that we used for *our* site/servers. I assume you have
something that's more important to you than our site, right? Where's your bar?
How do you know that **you** are drain ready?

### Load Shedding

Please forgive this tangent, but would you like to see something cool? You can
make any civil engineer turn white, no really, it'll work on just about anyone
who works energy generation or power delivery, you can get any of them to turn
dead white. Just find one, and repeat to them: *"mandatory load shedding"*. (or
if you're in the EU it's *compulsory load shedding*). Cool right? You can also
try *black start* if you want to try to make them break out into a cold sweat
too.

For the uninitiated, load shedding is the process (generally) for disconnecting
power consumers from the energy grid. Usually the goal here is to protect the
energy grid from total colapse, and avoid that same *black start*. Keeping an
energy system running is so much easier than starting, or restarting one that
"avoid a black start" is the equivalent to "keep the site up".

If you're ~~an engineer~~ a human, you should hold yourself to the same
standards. You should do *everything* in your power to avoid having to black
start yourself. Including making those decisions, as early as you're able to so
you don't have to make them when the pressure is on. There's far to many
variables for me to be able to give you a distinct number that will be useful
for you. But mine is 4. Studies have shown that once humans go over 8 disparate
responsibilities, it becomes exponentially easier to make a mistake, miss
something, lose track of the current state, or simply see degraded performance.
4 is just where I start because I want to have made the decision, well in
advance of the case where I suddenly need to double my workload with more urgent
items.

That decision, is what specifically you're going to **intentionally** drop on
the floor. Ask yourself. If I picked up X number more urgent things that I
couldn't ignore, or deal with later, which of the tasks am I currently dealing
with, will I drop, ignore, passoff, set aside, call good enough, which ever name
you decide to give it; so long as the result is, it's no longer something you
allow yourself to spend any time, or give ***any*** attention. And then, make it
a rule! The decision can *not* be, "what will I ignore unless it's really
important." It **must** be "What will I ignore so I can save my attention for
the more important stuff".

### My Drain Readiness

I can still clearly recall the sudden feeling of unease, back at
`$BIGDATACOMPANY` I was sitting in a meeting with a number of engineers, when a
manager asked, what's your capacity. Nearly everyone at the table, across
multiple teams, said they were at 100% capacity. Everyone gave an answer over
90%.

This was shortly after I had more than a few engineers, all of whom I deeply
respect tell me either, not to burn myself out trying to do my job, or ask me if
I was sure I was doing ok, and I wasn't getting over loaded. After taking a
minute to make sure I really was doing ok. I said yes, I wasn't at risk of going
over my total capacity, but I was out of buffer, and starting to enter red line.
That's when I decided that it was well past time for me to shed some load
myself.

My intent was to hand off one of the incidents I was working on, but everyone I
wanted to trust was already at, or over the capacity they should have. My first
reaction was much closer to disappointment, that there wasn't anyone I could
trust to help. But that was short lived, and replaced by that feeling of dread
when I realized, that I wouldn't have been able to volunteer either. I wasn't
drain ready myself, I was *way* to close to redline. 

### Your Drain Readiness

Avoiding a black start is an emergency situation, something has already gone
wrong, and now you're way past just triage mode. There are now more problems
than there are people who are able to work on resolving said problems. Which
means, priority 0 is now not allowing yourself to become an additional problem.
If you lose the ability to help, you're only going to make everything worse, for
everyone. Don't allow yourself to get there! Start **your** load shedding
procedures, and start deliberately ignoring everything you need to make sure
you're doing a good job at what does have your attention!

No matter how perfect the metrics you use to predict how capable you are as an
individual, or how excellent you are at triaging under stress, unless you're
omniscient, there still might be something much more important around the corner
that you didn't predict. And if it's something important to you, that's the only
thing that should get your attention. So don't allow yourself to make the
mistake that I made, just because you have some personal buffer you can tap
into, that doesn't mean you're drain ready. If you spend your personal buffer,
you've just lost the ability to protect yourself, which also means you've lost
the ability to prevent yourself, and the problems you were fixing from dropping
on top of someone else.

And now, I'm going to say the exact same thing again, because everyone thinks
they're fine because they're not even at their capacity yet. But that's the
whole point! You're not drain ready if you're still "under capacity"! You're
**only** drain ready when you can cut a **full 4 hours** from your day[^sleep],
every day for a few weeks and still be within your personal capacity. 



[^sleep]: If you lost 4 hours, what would you cut out? I'd bet for a lot of us
    the first on the list is sleep. How long could you be you with 4 hours less
    sleep? How many of us are now getting negative sleep?

