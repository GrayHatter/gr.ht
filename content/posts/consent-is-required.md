+++
layout = "post"
title = "Consent Is Required"
email = "consentrequired"
date = 2025-04-12
tags = ["off-topic", "ethics", "consent", "trust"]
draft = false
trunc = 262
+++

As I sit here attempting to decide what exactly belongs in this intro, I wonder
how many more times someone is going to remind me exactly how important consent
is, or remind me how easy it is to lose sight over how much influence any
individual has over another. In addition to how easy it is to miss the
connections between some action and it's outcome; the more layers of indirection
required as any system increase in size, the harder it becomes to even describe
how, or who plays which part. The ease at which anyone might forget, or how the
difficulty grows as the system becomes more complex, doesn't seem to be the part
that irks me. Sadly, the more I look for it, the more I see software engineers
directly, or indirectly though the systems they drive, ignore consent when it's
expedient: This is bad! The behavior of these systems come from decisions that
an engineer made. Engineers can, and should make the best decision, that also
does what's right by the people who uses these systems. While admittedly, they
don't often feel like it; the ethical decisions are easy decisions to make. As
engineers, collectively, we should take pride in what we build such that we want
to make the best decision. Enough pride, that we all also feel embarrassed when
we fail to do so.

Opinions differ on what exactly counts as consent, often it depends on the
context[^difficulty]. I'd venture to guess it gets even more complicated when it
comes to software. I'm sure that contributes to why TOS are so unparseable by
the very people who are required to agree to them, that there's even a website
dedicated to explaining common ones[^dislike]. What does consent look like when
it's software they're interacting with? Clearly, If someone is choosing to
continue using the software, that must count as consent! Except, no, it's not.

[^difficulty]: Mine don't; clearly communicated agreement with disclosure. It's
    not hard to **consider the other human!**

[^dislike]: It's [TOS;DR](https://tosdr.org/), which I elect to only link here
    because I disagree with a number of it's conclusions and assertions. I still
    applaud the attempt.

In something that I'm sure isn't a shock to those I expect to read this, I'm
gonna use an example from healthcare[^again]. For any significant procedure,
there's someone who's been assigned to collect a signature on the paper that
will make the hospital's lawyers happy. But the patient signing their agreement
on the "terms of service" for the treatment, isn't where consent ends. Consent
is more than the simple tick this checkbox and then tap submit. Healthcare has
learned, many times through mistakes; about what consent really means to the
humans they treat[^humans]. It's easy to put any one into a situation where
they'll "agree" to something. Only to then feel taken advantage of, or abused.
Abused by people who day job is literally to save their life, and help them
heal. When medicine trys to understand the why, patients often explain it as
simply as:

[^again]: Yes... again! :D [Informed Consent]( {{< ref
    "2019-07-14-informed-consent.md" >}} ) is probably required reading as well.

[^humans]: We're talking about medicine here because they better at
    understanding what they do to humans. Their interactions with humans aren't
    abstracted away by vscode.

> I didn't understand what was going on, or what was about to happen.

That's it, no one talked to them, no one told them what to expect, patients
under a significant amount of stress, who ostensibly trusted the people taking
care of them. Would feel victimized simply because *they* didn't know what was
going on. This is something that still happens quite often. The people
preforming whatever that procedure is have become such experts, they've done it
**so** many times, they'll forget that for the patient, this is brand new. The
end result from this interaction, the one with the primary goal of improving
their health left feeling abused or violated.

Contrast that with the experience of patients when someone is consistently
talking to them, and explaining to them what's gonna happen next, each step of
the way. Reminding them during difficult procedures, or ones that might be
painful that they can ask to take a break if they need it. Those patients leave
from the exact same exchange feeling cared about, and taken care of. Simply
telling someone what to expect before it happens, and importantly giving them
they have the option to opt out. Changes the experience from something
traumatic, and violating, into one where they feel like someone cares about
them. I suspect it might be shocking to your average ~~software engineer~~
human, how far treating users with just a little bit respect will go.

## What does respect look like?

Serendipitously I happen to come across this photo when doing something
completely unrelated to writing this.

![How Microsoft asks for consent](/assets/ms-consent.png)

This is consent right? Permission freely given, with a fair opportunity to
decline or otherwise opt out? Well, I'm sure Android is better though, right?
Surely they...

![How Alphabet asks for consent](/assets/goog-consent.png)

This one feels especially egregious to me. Because you can't tell the only way
to decline is hitting the back button, I'm also the type that likes the on
screen buttons, where I know most people use the new swipe gestures. But hey,
when has an update ever caused any problems[^911]? Obviously a system update is
for the benefit of the user!

[^911]: https://www.engadget.com/microsoft-teams-911-call-android-bug-fix-201139753.html

It's easy to forget, so this is where I'll remind you. I'm a security engineer.
I both deeply understand the specifics, as well as what goes into creating a
robust holistic security system. I know exactly how significant the thing that
I'm clearly suggesting is, and how catastrophic in would be. Allowing
***users*** to opt out of a security update? Clearly I've lost my mind, it's
safe for you to stop reading here, and leave a comment saying I'm dumb!

But that's not actually what I'm suggesting[^maybe a little]. I'm not brave
enough to earnestly suggest putting end users in direct control of security
updates. But, in my ideal world; security teams wouldn't use the same dark
patterns everyone admits are harmful, and toxic, and bad, and no one should use
them... up until they want to use them. [Because surely **my** reason is the one
time where the ends actually justify the means!] I’ll even go one step further,
and ask, why aren't users clamoring to install security updates? Why don’t your
users trust you? Why do they ignore security updates when security is what
everyone is always talking about? Which engineers get to fix that trust problem?

[^maybe a little]: I do think everyone should be permitted to make their own bad
    decisions, when they are solely responsible for the inevitable outcomes.

## Catalyst

Now's probably the place where I'm supposed to describe the catalyst for this
rant. Now, this has happened to me twice, and I wanna try to be clear here, the
newest UI layout is objectively better, for a number of reasons. But exactly
when I was already having a seriously awful day[^bots], my wifi network crashed
and I had reload most browser tabs. *It was at this moment I knew, discord
fucked up*. I was already pissed, and an update I normally would be excited
about, turned into a "surprise update[^suprise]" that pissed me off even more. Truth be
told, I knew I was gonna write something like this once I read one of the Q&A
answers from the most recent (to me) discord **mobile** layout update. For you
see, discord understands!

[^suprise]: There's a 4chan meme that this is as far as I'll explain here, but
    it's not about updates. Still about consent though...

[^bots]: and frustrated by the LLM bots I'm gonna rant about next.

> Q: Can I go back to the original mobile app layout?
>
> A: We understand the change might take some getting used to, and we're here to
> help make that transition as smooth as possible for you. But with this update,
> the original mobile layout is no longer available[^understands].

[^understands]: https://support.discord.com/hc/en-us/articles/12654190110999-New-Mobile-App-Updates-Layout

Remember how earlier I mentioned how you talk to people changes how they
experience consent, both implied and explicit? Yeah, I know I'm not alone when I
say this, because more than a few friends have shared the same aversion to
"surprise updates", but I really **do not appreciate people changing things for
me!** So when I wanted the old UI, and the first words I read was how discord
"understands", and how they're "here to help" *[sigh]*... The whole thing really
felt like a middle finger[^understood].

[^understood]: If you really understood, and wanted to help. You would have
    provided a "best effort" old version, at least for a few versions.

I'm someone who likes living on the bleeding edge of software. I'm better than
average when it comes to tolerating bugs that don't involve data loss. I'd be
one of the first to opt into a new layout. But you'll notice how I said opt in,
because with any changes you're making "for" someone... well Daniel Sloss
conveys exactly what I mean to express much better, when he request you to
*[nsfw video]* [ASK FIRST](https://youtu.be/1Y5AS3M9Vlo?t=73)!

By now, I'd be unconvinced, because I meant it when I said I like new updates.
"So what, you said the UI is better, why are we still talking about this?"
Because I'm still using the old discord mobile layout, (mostly out of spite from
that Q&A at this point.) I've chosen to pin myself, someone who often pretends
to be a security engineer, to an out of date version. I'm willingly using an
old, out of date apk of Discord, because it turns out, I will cut off my nose to
spite my face. And [there are dozens of us](/assets/dozens.mp4)!

I'm *sure* their security team is thrilled about this. I can confidently guess,
because of exactly how times, we at `$OLD_JOB` wanted to make a significant
improvement to security, or abuse detection/prevention, but we were thwarted by
our unwillingness to outright block support of old devices. I begrudgingly
assert this was and still is the correct decision. I refuse to punish users who
can't update for whatever reason, because more often than not, it was our fault
they aren't able to update.

It turns out, if you ignore consent, that makes your users stop trusting you,
and once users stop trusting you, that harms security of the whole system too.

## Reason

If that was just the catalyst for starting this essay, what is the real reason
it's actually getting published[^hawt]? The real reason is from my disappointment
watching sr.ht hurt itself in it's anger. For the next few lines, play the 8bit
pokemon battle music in your head!

[^hawt]: ![LLM scraping so hot right now!](/assets/scraping-so-hot.png)

![How source hut asks for consent](/assets/sr.ht-consent.png)

sr.ht became confused.

sr.ht used Anubis; it's not very effective...

sr.ht hurt itself in its confusion.

I'm not apathetic to this specific source of anger and frustration. If anything
you'd describe this feeling I share as empathy instead. I've spent a bit of time
trying to make it easier for others[^easier]. My problem is more that sr.ht has
decided that it's time for them to externalize their costs directly into **my**
face! I've not done anything wrong, but the solution they've elected to go with,
out of anger for the current state of things, is to punish[^punish] me.
Unfortunately for everyone involved, I've elected not to play this little game.
I've had to reject a few questions related to code that was hosted on sr.ht
because I couldn't view it, until it was copied to a less open
service[^srctree]. This isn't how consent is support to work!

[^easier]: TODO link to commit here.

[^punish]: Calling this a punishment to me is stretching the definition a bit
    far. If anything it's more of a punishment to sr.ht's users. Who now I
    refuse to support.

[^srctree]: Here, seems like an important place to disclose I'm building srctree
    in part because of the other issues I have with github, and to a much lesser
    extent, with source hut.

## Consent

I almost feel bad for the above. It does seem to imply I'm blaming sr.ht here
for failing to obtain consent. But that's entirely inaccurate. Source hut is
playing fair. Showing the splash screen while my computer wastes energy and cpu
cycles for no other reason than "why not[^LLM power]", is totally within the
realm of reasonability, and does seem to be fair in requesting consent; even
though I refused. The problem with the missing consent are the bots.

[^LLM power]: Remind me again, what's one of the major complaints about GenAI?
    It's a totally green technology, right?

It's important to note, while everyone loves to complain much more often about
the bots from "Big LLM", I've *yet* to catch any of them ignoring, or abusing
robots.txt. Some of the complaints are valid, they are needlessly aggressive,
and I'm in full agreement that it's incompetence bordering on maleficence to
scrape the web interface to a git repo. Not a single one of them violates
consent. While many have a deeply ingrained disgust for them, or distrust for
the patrons funding their existence. They're playing fair, by all the reasonable
rules. They're not trying to hide, they try very hard to respect robots.txt,
they clearly announce themselves, and most even enumerate and publish the IP's
they make requests from, to help prevent others from being able to impersonate
their bot. Really,whether you like them or not, they're being good web
citizens... at least where crawling/scraping and consent over *access* is
concerned.

<!--
The ones violating the rules for consent are these bots.

```
43.128.149.102 - "GET /repo/dns/commit/43edea6e HTTP/1.1" 200 932 "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1"
34.145.110.128 - "GET /repo/srctree/tree/srcapi HTTP/2.0" 200 1650 "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36"
34.83.184.238 - "GET /repos/gak/issues HTTP/2.0" 200 494 "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36"
35.197.78.148 - "GET /repo/mqtt/diffs/new HTTP/2.0" 200 639 "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
35.203.140.140 - "GET /repo/srctree/issues/d HTTP/2.0" 200 564 "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36"
114.250.44.111 - "HEAD /repo/n_e_s.git/commit/06fc04b5 HTTP/1.1" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36"
```
-->

Not a single one of these are real users, even though each claim to be one. And
there are a lot more than just these. These are just the ones in front of me as
I write this. I didn't even *try* to go looking.

I've created and now published [nft rules](https://srctree.gr.ht/repo/rules)[^nftrules]
for IPs that I've had to ban for evading consent. The whole Hetzner ASN is
banned, as well as a few others. Tencent and AliCloud will be next I'm sure. And
I've filed an abuse report to Google Cloud already, but they only have a few
more days before I ban their whole ASN as well. GoogleBot, another normally good
citizen, one with a purpose I support (sharing information) would be
unfortunate, but acceptable collateral damage here.

[^nftrules]: If anyone decides to use them, let me know I'll start annotating
    them as well.

***You can not obtain consent if you're lying about who you are, and what you're
doing!*** I'm happy to share my resources with well behaved bots. Ones that are
fair, and don't try to trick me. If you're lying about your user agent, you are
the problem. You're intentionally behaving to avoid consent, and to avoid the
ability for others to enforce their rules for consent.

## TL;DR

Unfortunately, I find I've run out of ribbon. Otherwise I'd make an attempt to
tie this whole thing together. So instead, I'll go with one last story:

I remember doing a security review for a new account access and password change
flow at `$OLD_JOB`. We'd finished discussing all of the security implications,
and approved the implementation in code. The last remaining question was that of
the default behavior. The specific question asked, was "If there were any entry
flows where we wouldn't want to give the user the option to keep or invalidate
any or all existing sessions?" The answer was no, none of the privacy or
security teams had any entries into this flow where the user shouldn't be the
one to make that decision about their sessions. But I did make the request that
default option should be to invalidate the sessions, so if I user didn't have
the confidence in which decision they should go with, they'd default to the one
that was safer for their account. The software engineer who was building this
flow objected, only by default rather than intention. The standard operating
procedure at `$OLD_JOB` was *never* destroy sessions if you could help it[^dau].
I probably only remember my response to her objection because I remember her
face light up to my response.

[^dau]: because the line on the graph must always go up... :/

> Yeah, that's true. But for all the users entering this section of the flow, we
> already know that they're able to login with the user and password they just
> set, but also know that they have a valid backup contact they could use to log
> back in if they really needed. As a bonus doing it this way protects users who
> might have been confused about the "new login" email and aren't sure what to
> do. It's safer for them if we leave just the new session we know is good. But
> this is your user flow right? You, [and your team], are the one who get's to
> make the final recommendation and decision here. So really it's up to you to
> decide if you want the default to be protecting users, or trying to increase
> [the number of daily active users] with sessions we don't know are real. But
> whatever you decide, [Team Name] Security will be there to back your decision,
> which ever you want to go with. If you want to invalidate sessions, but you
> get any pushback [from your team], let us know and we'd be happy to make it a
> security requirement for you, and then we'd be the ones to handle any
> arguments.

I will remember that conversation, and her reaction, for a long time. It's rare
you get to see someone surprised for the better about being "allowed" to do the
right thing. The expectation that I got to dispel was; a made up rule about what
you're "allowed" to do. I have no idea what the current state is today. There's
a non-zero chance someone else changed it because maybe it might have a DAU win.
This was years ago by now, so it's even more likely that flow was replaced with
the latest and greatest in 'account center technology'. But that flow did
launch, and when it launched; the default **was** protecting users. I also never
did have to argue with anyone. Because it turns out, quite often, it **is** as
simple as one person deciding that they are going to do the right thing.
