---
layout: post
title:  "Passwords Considered Harmful"
date:   2019-09-16
lastmod: 2023-02-18
tags: security, privacy, passwords, harmful, on-topic
---

Passwords, plainly, are not only bad at their intended purpose, but nearly
everyone is incapable of using them correctly. That includes both developers,
and users. Meanwhile they're a constant security risk, not only because
individual passwords can be broken, stolen, guessed, or given away. But also
because, if you have no other data than email and password pairs you do have
something worth stealing. Painting an even larger target on your back. It's time
to stop using password for authentication. Passwords are now considered harmful,
and you shouldn't use them anymore.

First, consider what problem passwords solve. User authentication. No, really!
That's it, that's all they're good for[^1] [^2]. Passwords are shared secret
between the server and the client. I have to start with this because I've had to
dispel the notion that they have something to do with authorization. But that's
different problem entirely. A user account may be authorized to do many things,
but each only has a single password.

[^1]: [1] Ok, that's not the only thing, passwords are also useful as a [Duress
  Code](https://en.wikipedia.org/wiki/Duress_code)

[^2]: [2] Passwords are also used as a seed for a key, but why that's a bad
  thing is a topic for another day.

Security professionals have known passwords are bad for a long time. If you
don't believe me, watch me predict the future. When you're ready, ask your
nearest information security person what's the gold standard for account
security, then come back. (I promise not to change the text while you're gone)
They said Two Factor Authentication[^3]. Now, I know what you're thinking, and
no, it's not magic. It's that passwords are so broken that a password and
literally anything else is current best practices.

[^3]: [3] If you think *that's* something, I knew they also said something about
  using a One Time Passcode (OTP). Bonus points for your security person if they
  said TOTP (Time based OTP).

Passwords make the user experience suck too. Think back, whens the last time
you were trying to use a site, perhaps an online shopping site. You've added
everything you want to the cart, ready to check out, when you forgot your
password? If you can actually remember a time, I'm sorry. Not just for you, but
for the site as well -- frustration is the memory you have of using their
software. How many friends are you gonna refer to them now? Is it less than it
could be?

Say what you will about Facebook's privacy/security. They've built a good UX.
They've even gone so far as to try to *"fix"*[^4] passwords. If the password you
enter isn't correct, Facebook will jitter your password a bit, trying different
letters, or capitalization trying to "guess" your password for you. As much as
learning that hurt me as a security geek, It's a good idea.

[^4]: [4] There's not air quotes large enough to contain the use of the work fix
  in relation to facebook.

That brings us back to the start. How many accounts to you have easy access to
that you don't know the password to off the top of your head? Even if you don't
have a password manager, I'm willing to bet the number is >= 1. So for that
account, requiring a password isn't authenticating you, it's authenticating what
ever thing is actually storing that password[^5]. Which means passwords aren't
even doing the single thing they're supposed to be doing: Authenticating users.
They're authenticating devices, and there's already plenty of better ways to go
about that. It time to stop using passwords.

[^5]: [5] Please don't let it be a post-it note!

I've already put my money where my mouth is[^6]. [MechMark] is a webapp I wrote
in a weekend to track who has mechnical keyboard parts they can sell to fellow
makers/builders. It doesn't use passwords at all, instead it'll log you in via
token sent to your email. (If you're first instinct is to complain that's not
secure, be honest, you were going to let anyone with access to the users email
reset the password anyways.) The [source] is on GitHub if you want to take a
look.

[^6]: [6] "HEY... This isn't really a considered harmful, it's shameless self
  promotion!" -- [Why not both](/assets/both.gif)?

[MechMark]: https://mechmark.bsdev.net

[source]: https://github.com/GrayHatter/MechMark/

