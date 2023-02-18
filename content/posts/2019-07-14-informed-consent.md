---
layout: post
title:  "Informed Consent"
email: infcon
date:   2019-07-14
publishdate: 2019-07-14
lastmod: 2023-02-17

tags: security, privacy, on-topic
---

In news that's surprising to no one who'd read this. [OK Google Voice recordings
leaked](https://arstechnica.com/information-technology/2019/07/google-defends-listening-to-ok-google-queries-after-voice-recordings-leak/)
Yet, this is still breaking news. When I first read this story, I felt
bad for the people who were contacted for comment by the news reporting agency
who broke this story. It's not hard to imagine that they were surprised that the
device was recording their conversation, especially given that they didn't even
say the keyword. I'd bet it was even more surprising that it contained enough
information for a reporter to find and contact them. That level of invasion of
privacy is a pretty hard hit to just absorb.

I, obviously, wasn't surprised, but even given the base technical level of most
users, they shouldn't have been surprised either. I don't think it shouldn't be
surprising because of an expectation this should be a thing that happens[^1],
nor because [privacy is dead](https://www.youtube.com/watch?v=DaYn_PkrfvQ). But
because the gold standard should be everyone
opts-in to risk with informed consent.

[^1]: [1] This kind of thing *should* never happen, don't hurt other people!

When I say informed consent, I say it from its use in medicine. Everyone "knows"
the first rule of being a doctor is "First, do no harm". Ignoring the point,
that this particular cliche isn't even a part of the Hippocratic Oath, it's also
not even a reasonable expectation in all cases. If it was, there'd never be any
experimental treatments, no high risk surgeries. Even some low risk procedures
would likely require exclusion as well. What medicine has instead is informed
consent.

Informed consent at it's minimum has 3 parts. 1) Give your recommendation, and
what your treatment plan is. 2) Describe the common/possible risks of your plan.
3) List some of the alternative options. That's really all there is, there's
some other important nuance, using language the person you're talking to can
understand, but the core is really that simple. What's the closest equivalent we
have in tech? The end user license agreement, the defining example of TL;DR[^2].
It's embarrassing.

[^2]: [2] see also: [TOS;DR](https://tosdr.org/)

I don't mean to suggest that you shouldn't build exactly what you want to build.
Every technology, just like every treatment in medicine carries with it *some*
risk. The stark difference is in healthcare, the person who decides what risk is
worth what benefit is the person who has to take on the risk. In tech, the
person making the decision about what risk worth it, is some engineer. Or more
terrifyingly some corporate manager. Generally, you should avoid taking risks
for others. You can do that, by *asking*!

The first change you can make, is making everything with an additional privacy
risk exclusively opt-in. For the more experimental features or ones with a much
higher chance of a negative outcome, add confirmation model that enumerates the
risk in an understandable way. As an example, even the most egregious privacy
violator can even get it right some times...

![location_sharing_warning.png](/assets/location_sharing_warning.png)

Notice Google Maps isn't warning about using GPS for tracking, that's because it
shouldn't. Physicians don't need to explain every single risk of each and every
single intervention. Were you told that lidocaine used to numb an area prior to
dental work and/or sutures is cardio toxic? I'd hope not, because while true,
it's not meaningful risk for the doses used. (This is also my favorite example
of why you should never hide ***anything*** from your doctors, they know and
consider these things before choosing any drugs). So, don't warn users that
their email, username/password could be stolen if you get hacked. Use a good
salted password hashing method, so it can't become a meaningful risk. But it's
probably a good idea to disclose that you're storing every single conversation
had in "ear"-shot of the ultra high gain microphone that powers your new smart
device. Because no one in their right mind would opt-in to that kind of thing...


P.S. The GPDR is a nice start, it also solves a lot of other related issues with
internet privacy, but it's not a substitute for consent.

