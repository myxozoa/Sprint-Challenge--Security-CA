The security challenge is a little different - you won't be writing code.
Instead, you'll be thinking about security, practicing your professional
communication skills by writing about a threat model as if you were emailing a
coworker. Then you'll apply what you've learned by improving your own practical
personal security, and again write up what you've done (just to document it, but
a good stretch goal is to make your writing even more polished and publish it as
a blog post).

For both of these, turn it in by commiting a Markdown file with your writing to
your fork of this repository. If you publish elsewhere, please share the link as
well.


# Part 1 - Understand and Communicate a Threat Model

Think of a threat model - a situation with a user (or type of user) and a
context that frames their personal security preferences and situation. Concepts
you should consider (and a few examples of each) include:

- Attack surface (what tech/situation exposes them, e.g. systems they use, places they go)
- Adversaries (who may be interested in compromising their security, e.g. criminals, pranksters)
- Attack vectors (specifically how they may be compromised, e.g. password theft/cracking, surveillance)
- Mitigations (what can be done to reduce the risk, e.g. 2-factor auth, encryption)

Write a summary of the overall situation as if you were going to send it as a
professional email to explain it to a coworker. Please turn in a file
`ThreatModel.md` with 1-2 paragraphs addressing the above concepts in a concise
fashion.


# Part 2 - Practical Security

Do something to improve your personal security setup - if you’re not using a
password manager, set one up. If you’re doing that, then set up two factor for
some of your accounts. If you’re doing that, then set up proper SSH keypairs for
services that support it (e.g. GitHub). And you can keep going - set up a GPG
keypair, consider simple dedicated hardware for second factor, set up a trusted
computer/VM running only open source software, set up a "sandboxed" environment
for web browsing that doesn't save state, etc.

Use the practices and approaches we learned about this week - this means pick
a suitably long *passphrase* to protect your password manager, and think about
what your threat model is and what services you want to trust with what
information. Some general tips:

- You are a software developer, which means you're a high value target (you are
a potential attack vector to anyone who runs your code)
- Unless you're working on something controversial for the political regime you
reside in, the NSA/Mossad/KGB/MI5/etc. are probably not your adversaries
- The sorts of threats you *should* worry about - common criminals/organized
crime, botnets, malware, extortion (stealing your files, DDoS-ing your service)
- For deciding whether or not to trust a service, consider history, reputation,
and incentives, as well as what countries it operates in (which will impact the
laws it is subject to, both in terms of disclosure and potential damages)

Some resources/goals:
- [KeePass](https://en.wikipedia.org/wiki/KeePass) - open-source password manager
- [Alternatives to KeePass](https://alternativeto.net/software/keepass/) - cloud, desktop, etc., consider your personal security/convenience tradeoff
- [Two Factor Auth](https://twofactorauth.org/) - list of services that support 2 factor authentication
- [Connecting to GitHub with SSH](https://help.github.com/articles/connecting-to-github-with-ssh/) - more convenient (for command line) *and* secure than passwords
- [Adding GPG to your GitHub account](https://help.github.com/articles/generating-a-new-gpg-key/) - simple GPG setup that will let you sign commits
- [Creating the perfect GPG keypair](https://alexcabal.com/creating-the-perfect-gpg-keypair/) - more complicated, for those who want finer control
- [Keybase](https://keybase.io/) - a way to share/certify public keys (also offers encrypted chat, file storage, etc.)
- [Yubico](https://www.yubico.com/) - affordable hardware security devices for two-factor/crypto
- [How to install Ubuntu in VirtualBox](https://linus.nci.nih.gov/bdge/installUbuntu.html) - usable secure popular distribution of Linux
- [Kali Linux](https://www.kali.org/) - security-specific (penetration testing) distribution of Linux, includes VM images for download
- [Information about Sandboxes](https://en.wikipedia.org/wiki/Sandbox_(computer_security)) - general starting point for learning about sandboxes to contain an application

After you do some of the above, turn in a file `PracticalSecurity.md` with 1-2
paragraphs summarizing what you did (remember, a good security setup doesn't
depend on security through obscurity, so it should be safe to talk about it as
long as you don't share actual passwords/secrets). As a stretch goal, write a
blog post about your security setup describing what you’ve learned and tips you
have for others.
