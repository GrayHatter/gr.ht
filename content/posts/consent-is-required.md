+++
layout = "post"
title = "Consent Is Required"
email = "consentrequired"
date = 2025-03-29
tags = ["off-topic", "ethics", "consent", "trust"]
draft = true
summary = """As I sit here trying to write this intro, I wonder how many more times someone
is going to remind me exactly how important consent is, or remind me how easy it
is to lose sight over how much influence any individual has over another."""
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
directly or indirectly though the systems they drive, ignore consent because
it's expedient. This is bad, and collectively we should be embarrassed enough to
do something.

Opinions differ[^difficulty] on what exactly counts as consent. I'd venture to
guess it gets even more complicated when it comes to software. I'm sure that
contributes to why TOS are so unparseable by the very people who are required to
agree to them, that there's even a website dedicated to explaining common
ones[^dislike]. What does consent look like when it's software in between? If
someone continues to use the software, isn't that consent? No, it's not.

[^difficulty]: Mine don't; clearly communicated agreement with disclosure. It's
    not hard, **consider the other human too!**

[^dislike]: It's [TOS;DR](https://tosdr.org/), which I elect to only link here
    because I disagree with a number of it's conclusions and assertions. I still
    applaud the attempt.

In something that I'm sure isn't a shock to those I expect to read this, I'm
gonna use an example from healthcare[^again]. For any significant procedure,
there's someone who's been assigned to collect a signature on the paper that
will make the hospital's lawyers happy. But the patient signing their agreement
on the "terms of service" for the treatment, isn't where consent ends. Consent
is more than just tick this checkbox and then tap submit. Healthcare has
learned, many times through mistakes; about what consent really means to the
humans they treat[^humans]. It's easy to put any one into a situation where
they'll "agree" to something. Only to then feel taken advantage of, or abused.
Abused by people who day job is literally to save their life, and help them
heal. One of the most common reasons cited is;

[^again]: Yes.... again! :D

[^humans]: We're talking about medicine here because they better at
    understanding what they do to humans. Their interactions with humans aren't
    abstracted away by vscode.

> I didn't understand what was going on.

That's it, no one talked to them, no one told them what to expect, patients
under a significant amount of stress, who ostensibly trusted the people taking
care of them. Would feel victimized simply because they know what was going on.
The end result from some treatment with the primary goal of improving their
health left feeling abused. This isn't the experience of patents when someone is
consistently talking to them, explaining them what's gonna happen next.
Reminding them during difficult procedures that they can ask to take a break if
they need it. Those patients leave from the exact same exchange feeling cared
about, and taken care of. Simply telling someone what to expect before it
happens, and importantly giving them the option to opt out. It might be shocking
to your average software engineer how far treating users with just a little bit
respect will go.

Serendipitously I happen to come across this photo when doing something
completely unrelated to writing this.

![How Microsoft asks for consent](/assets/ms-consent.png)

This is consent right? Permission freely given, with a fair opportunity to
decline or otherwise opt out?

Well, I'm sure Android is better though, right? Surely they....

![How Alphabet asks for consent](/assets/goog-consent.png)

This one feels especially egregious to me. Because you can't tell the only way
to decline is hitting the back button, I'm also the type that likes the on
screen buttons, where I know most people use the new swipe gestures. But hey,
when has an update ever caused any problems[^911]? Obviously a system update is
for the benefit of the user!

[^911]: https://www.engadget.com/microsoft-teams-911-call-android-bug-fix-201139753.html

## Catalyst

[this is the incomplete section]

The last medical procedure I participated in was one of my own. It was an MRI
with contrast of my shoulder.

Now's probably the place where I'm supposed to describe the catalyst for this
rant. [Discord]

> Q: Can I go back to the original mobile app layout?

> A: We understand the change might take some getting used to, and we're here to
> help make that transition as smooth as possible for you. But with this update,
> the original mobile layout is no longer available.

https://support.discord.com/hc/en-us/articles/12654190110999-New-Mobile-App-Updates-Layout

## Reason

If that was just the catalyst, what is the real reason. The real reason is from
my disappointment watching sr.ht hurt itself in it's anger.

![How source hut asks for consent](/assets/sr.ht-consent.png)

sr.ht became confused.

sr.ht used Anubis; it's not very effective...

sr.ht hurt itself in its confusion.

I'm not apathetic to this specific source of anger and frustration. If anything
you'd describe this feeling I share as empathy instead. I've spent a bit of time
trying to make it easier for others[^easier commit]. My problem is more that
sr.ht has decided that it's time for them to externalize their costs directly
into **my** face! I've not done anything wrong, but the solution they've elected
to go with, out of anger for the current state of things, is to punish[^punish]
me. Unfortunately for everyone involved, I've elected not to play this little
game. I've had to reject a few questions related to code that was hosted on
sr.ht because I couldn't view it, until it was copied to a less open
service[^srctree]. This isn't how consent is support to work!

[^easier commit]: TODO link to commit here.

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
reasonability, and does seem to be fair in requesting consent; even though I
refused. The problem with the missing consent are the bots.

[^LLM power]: Remind me again, what's one of the major complains about GenAI?
    It's a totally green technology, right?

It's important to note, while everyone loves to complain much more about the
bots from "Big LLM", I've *yet* to catch any of them ignoring, or abusing
robots.txt. Some of the complains are valid, they are needlessly aggressive, and
it's incompetence bordering on maleficence to scrape the web interface to a git
repo. Not a single one of them violates consent. While many have a deeply
ingrained disgust for them, or for the patrons funding their continued
existence. They're playing fair, by all the reasonable rules. They're not trying
to hide, they obey robots.txt, they clearly announce themselves, and most even
enumerate the IP's they'll make requests from so they can't be impersonated.
Wither you like them or not, they're being good web citizens... at least where
crawling/scraping and consent over access is concerned.

The ones violating the rules for consent are these.

```
43.128.149.102 - "GET /repo/dns/commit/43edea6e HTTP/1.1" 200 932 "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1"
34.145.110.128 - "GET /repo/srctree/tree/srcapi HTTP/2.0" 200 1650 "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36"
34.83.184.238 - "GET /repos/gak/issues HTTP/2.0" 200 494 "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36"
35.197.78.148 - "GET /repo/mqtt/diffs/new HTTP/2.0" 200 639 "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
35.203.140.140 - "GET /repo/srctree/issues/d HTTP/2.0" 200 564 "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36"
114.250.44.111 - "HEAD /repo/n_e_s.git/commit/06fc04b5 HTTP/1.1" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36"
```

I've created and now published [nft rules](https://srctree.gr.ht/repo/rules) for
IPs that I've had to ban for evading consent. The whole Hetzner ASN is banned,
as well as a few others. Tencent and AliCloud will be next I'm sure. And I've
filed an abuse report to Google Cloud already, but they only have a few more
days before I ban their whole ASN as well. GoogleBot, another normally good
citizen, one with a purpose I support (sharing information) would be
unfortunate, but acceptable collateral damage here.

***You can not obtain consent if you're lying about who you are, and what you're
doing!*** I'm happy to share my resources with well behaved bots. Ones that are
fair, and don't try to trick me. If you're lying about your user agent, you are
the problem. You're intentionally behaving to avoid consent, and to avoid the
ability for others to enforce their rules for consent.

