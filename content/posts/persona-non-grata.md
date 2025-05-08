+++
layout = "post"
title = "Persona Non Grata"
email = "non-grata"
date = 2025-04-23
tags = ["infosec", "security", "drama", "llm", "abuse"]
draft = false
#trunc = 300
summary = """I had to stop myself from giving this article it's previous working title: Stop
Externalizing The Costs Of Your Service Directly Into Your Users Face. This is
the follow up I promised to write, when I omitted the longer complaint I had
about Anubis"""
+++

I had to stop myself from giving this article it's previous working title:

> Stop Externalizing The Costs Of Your Service Directly Into Your Users
> Face[^cmpwn].

[^cmpwn]: [Please stop externalizing your costs directly into my
    face](https://drewdevault.com/2025/03/17/2025-03-17-Stop-externalizing-your-costs-on-me.html)

This is the follow up I promised to write, when I omitted the longer complaint I
had about [Anubis](https://anubis.techaro.lol/) from my last post [about
consent]({{< ref consent-is-required.md >}}). Seeing people use Anubis makes me
feel sad! But you should in no way take as a critique against Anubis itself. If
I wanted to be shallow, there's plenty of cheap shots I could take against it's
[source code](https://github.com/TecharoHQ/anubis) I could only do so because
I'm still able to find humor in being a troll, the pedant in me dictates that I
claim the code has some issue, but there's nothing egregiously wrong with it.
It's good (enough) code! I'm even happen to double down, and I'm happy to link
to the creator, and to their blog which you can find....

![ https\://xeiaso.net/blog ](/assets/xeiaso-blog-down.png)

... oh, sorry, nevermind I can't reach their blog anymore. That's a shame I have
to admit that I didn't always agree with all of their takes[^never], but I've yet
to come across anything that's been flat out wrong. I've happily linked their
blog to others, and if it was still up, I'd still link to it. They've published
a number of articles that were better than what I wanted to write.

[^never]: I never do, for anyone, but such is the life of a pedant!

Oh, I know, surely the internet archive has it!

![ https\://xeiaso.net/blog ](/assets/xeiaso-blog-down-archive.png)

Fuck!

Well, I guess the internet just got a lot worse. The worst part; it's made this
way by people who purport to care about an open internet. I almost decided not
to include the source for the original title. But I eventually broke down,
because... well I haven't completely figured that out yet, but I feel I need to
explain exactly why this proof of work captcha feels like the right solution to
so many people, and then hopefully convince you why you should still shun
it[^shun].

[^shun]: Not the project, I'm glad it exists, and I'm hopeful I'll find a use
    for it. Or at the very least, learn from it's implementation. It's just not
    the solution to crawlers/bots for most cases.

I don't object to the idea, nor the concept of proof of work captcha. I've
advocated for trying it a number of times at `$OLD_JOB`, but was never invested
enough to charge up that hill. It's a good solution to consider when you're
unable to isolate scripted, from organic traffic. It's infinitely better than
visual human captchas. The part I object to, is serving it to **me**, or your
users who may or may not know better, or to the internet archive. Yes yes, it's
very cute you have an exclusion for curl, but that's still only in the security
through obscurity category, so you're welcome to claim the negative credit for
that!

I know exactly why, Xe is doing it, it's their new toy[^cool]. But I also know
why SourceHut is doing it, and it's not because it's the best solution. It's
because the owner of sourcehut is angry, and he's again, taking out his anger on
other people, in this case the users of SourceHut[^support].

[^cool]: and it **is** a cool toy!

[^support]: I've been unable to help someone asking for help with code a number
    of times because I can't, [wont?] load pages from git.sr.ht when they've
    linked to their source code hosted on sr.ht. Some have been happy to push to
    codeberg, others I simply couldn't answer their question.

> If you personally work on developing LLMs et al, know this: I will never work
> with you again, and I will remember which side you picked when the bubble
> bursts.

*sigh*

> I miss the old Drew.
    -- *e0ff*

That's a quote from a friend, I remember it, because a few weeks before that, I
said literally, the exact same thing, to a completely different friend. I said
about a year ago, and I said it again this past month. The new drew is more
interested in punishing people than build cool stuff that improves the world,
and watching that change has been very disheartening. I miss the sircmpwn that
wasn't exclusively angry.

The old ddvault understood that you don't punish users, you punish the people
directly responsible for the bad behavior[^go]. The irony here being the article
about blocking only the abusive behavior, is linked within the article
explaining how they're "forced" to serve this captcha to users. I run
[srctree.gr.ht](https://srctree.gr.ht), and I can attest, the new breed of AI
crawlers love git hosts. I've spent plenty of time watching logs scroll by that
I would classify as abusive. But **none** of them are subtle. The argument that
these are advanced persistent threats, that are impossible to identify, and are
constantly rotating identifiers, but have also chosen to spend this obfuscation
time on crawling webpages, instead of a simple git clone, doesn't pass the sniff
test[^tor]. I don't buy it. I'm sure some of you have already picked your side, so
I'll gladly fill in your objection for you. srctree is infinitesimally smaller
than sr.ht, so obviously I've just never seen the real abuse! Perhaps, anyone
with access to a host logs that's willing to share multiple KB of "raw" logs
showing mostly residential ASNs, maybe I can help you out. Until then it seems
unlikely, and doesn't match the traffic I've seen.

[^go]: [ SourceHut will (not) blacklist the Go module
    mirror](https://sourcehut.org/blog/2023-01-09-gomodulemirror/)

[^tor]: every time someone complains about abuse from a "residential" network, I
    can't not hear: TOR exit node.

### The solution on srctree[^joke]

[^joke]: There was a joke there, but I had to change it because I'm afraid of the C++
committee.

Ban them. No, seriously. Shoot the messenger! If you notice abuse from a given
ASN, ban the subnet. [I've published my
rules](https://github.com/GrayHatter/rules/)[^update] Some note worthy entries,
just tonight I banned the FB ASN[^fbasn], I'm sure that'll cause some problems
in the future, but that's future me's responsibility. As I mentioned previously,
I'm sure I'm gonna ban Alibaba's subnet next. Hetnzer is currently persona non
grata[^hetznerasn], GCP almost got the same treatment, but I filed an abuse
report, and it stopped[^shocked].

[^update]: I totally promise to update it soon... promise!

[^shocked]: I know, I didn't expect it to work either. But the timing seemed to
    match well.

That's it, it takes banning a new ASN every other week[^prove]. But the problem
is manageable. Without forcing browsers to complete a POW, or trust your
scripts. The problem is that the http traffic across the internet has suddenly
become a lot less human. The solution to hostile traffic isn't to make browsers
prove they're browsers. The solution to hostile traffic, is to block the hostile
traffic. You get bonus points if you report the abuse to the registered abuse
contact for the network, and tell them you've banned them for malicious traffic
sending fraudulent requests.

[^prove]: Please, prove me wrong. But bring published logs to show for it. I
    find most of the existing articles unconvincing. Claims of some experience
    that dosen't match mine, and no evidence other than. Just trust me bro.

If you really wanna have an impact: publish the IPs you've banned. I'm hopeful
the conversation goes something like:

> Hey, why can't I connect to [some service] from [some ISP]?

Oh, yeah, [ISP] is banned because they host too much abusive LLM/GenAI traffic.
You need to use a different ISP try, [other suggestion].

If you feel so strongly about how "fancy auto complete" is ruining the world, and
how there's no chance we'll survive this new *revolutionary technology*, and
everyone who works with it, is the devil, and you're gonna remember which side
they picked[^sigh]! Then target that vitriol at the service providers willing to
host this traffic, instead of targeting users! If you want to take a stand,
punish the people hosting the abuse!

[^sigh]: This toxic Us vs Them bullshit needs to stop. Please! I get that so
    many people are angry, I'm angry too. But the Us vs Them, where idle
    curiosity makes someone a "them" is a much bigger part of the problem than
    whatever the newest techno fad is, that you happen to dislike for whatever
    reason the "us group" has picked today.

Yes, large scale scraping is rough, and hard to maintain, but we are FOSS
hackers dammit, we've been building dope shit, and raising the bar of all
software for longer than anyone ever thought was going to be possible. We've
replaced bad user-hostile systems, with free, open, hackable code that does
exactly what we want. Hackers don't punish users, or ruin **their** code because
some VC startup doesn't know how to run a crawler, or clone a git repo, or wants
to lie about what it's doing.

### Other Options

#### Firewall

So you've decided to block the abuse? Everyone still seems to like iptables
still, but I use nftables these days. Below is a minimal example that you can
*probably* drop in if you're using nftables.
```
table inet filter {
    set abuse {
        type ipv4_addr
            flags interval
            auto-merge
            elements = { }
    }
    chain input {
        type filter hook input priority 0; policy accept
        ip saddr @abuse tcp dport { 80, 443 } counter
        ip saddr @abuse tcp dport { 80, 443 } reject with icmpx 3
        tcp dport { 80, 443 } accept
    }
    chain output {
        type filter hook output priority 0; policy accept
    }
}
```

I recently switched[^yesllm] because I wanted an easier to configure grouping.
Normally, I'd go with a scorched earth policy, and flat out drop everything that
I consider abusive. But in this case, I've started banning whole subnets; so I'd
feel bad if they didn't have a way to contact and ask for an
exception/correction. This way, if your main server is also your name server, or
email server, you can still receive a reply to that email you sent to the abuse
contact.

[^yesllm]: Yes... I wanted to group because of LLMs...

Arguably, the most important part of the above, is `reject with icmpx 3` when
you reject abusive crawler traffic, tell the sender why! Don't just drop the
traffic! Here, we reject with icmp type 3, code 13 (administratively
prohibited). The default, icmp reject `network unreachable` is misleading. It is
reachable, but the admin has prohibited this communication, for non-technical
reasons.

If you'd like to detect if you're banned from srctree, `tcpdump -n icmp` and try
to connect with your browser. You probably need to prefix with `doas` because
the raw socket required to listen for icmp packets requires elevated network
caps. If you see anything like `22:24:34.138261 IP 144.126.209.12 > 10.0.0.174:
ICMP host 144.126.209.12 unreachable - admin prohibited filter, length 68` Your
network host also hosts abuse. You should consider switching to a better ISP!

#### Firewall v2

Part of the original plan for this article was to submit a few patches to a
browser or two, to show a different screen when a connection is admin prohibited
instead of just "filtered" Unfortunately, these patches have proven themselves
to be more work than my current headspace allows for[^nmap]. This makes it very
hard for users to understand why they're blocked. If you'd rather not outright
block this traffic, but send it to your PoW gateway, or serve a custom notice,
or redirect to a separate instance on another port, that returns mostly 429 if
CPU usage is ever >50% or whatever other metric/resource you find is being
abused.

[^nmap]: I still have the idea to send a patch to nmap, but getting my brain to
    play along has proven harder than expected.

```
table inet raw {
    chain prerouting {
        type filter hook prerouting priority raw;
        ip saddr @abuse tcp dport 443 tcp dport set [custom server port]
    }
}
```

Setting up `nat` + `masquerade` in nft is outside the scope of this rant but
if you want to be really fancy, you could offload the abusive traffic to a
different system.

#### Verse Bot Detection

I've been playing with building bot detection in
[Verse](https://srctree.gr.ht/repo/verse) There's a number of ideas that you're
welcome to pick through if you're not ready to rewrite your whole codebase in
verse yet. As of the moment I write this, it's covers about 40% of the
detections I want to write. There's another high sensitivity rule that I need to
add, but then I suspect it'll catch 90% of all the crawlers lying about who they
are. If you do decide you'd like to try it out, or want to talk about how it
works. Send me an email, I'm happy to help you reuse what I've learned in your
detection system.

[^fbasn]: https://rdap.db.ripe.net/ip/57.141.0.0
[^hetznerasn]: https://bgp.he.net/AS24940#_prefixes

