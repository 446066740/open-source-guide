---
title: Leadership and Governance
description: Cupcake ipsum dolor sit amet powder sesame snaps croissant dragée. Cake chocolate cake gummi bears topping chocolate bar. I love carrot cake sesame snaps cake pie. Gummies chupa chups cupcake gummi bears ice cream lemon drops cake dessert. Powder pie macaroon chocolate cake I love. Caramels pastry donut I love I love donut. Biscuit cake soufflé. Wafer cake fruitcake pudding bonbon.
---

Your project is growing, people are engaged, and you're committed to keeping this thing going. At this stage, you may be wondering how to incorporate regular project contributors into your workflow.

Maybe you want to give commit access to someone who's made significant contributions. Maybe you got into a debate with a community member and realized you didn't know how to resolve it.

If you have questions about leadership and governance for open source projects, we've got answers.

## What are examples of formal roles used in open source projects?

Here are some common roles that you might have heard of for open source projects. What these roles actually mean, though, is entirely up to you.

* Maintainer

* Contributor

* Committer

For some projects, "maintainers" are the only people in a project with commit access. In other projects, they're simply the people who are listed in the README as maintainers.

A maintainer doesn't necessarily have to be someone who writes code for your project. It could be someone who's done a lot of work evangelizing your project (like @janl did for [CouchDB](https://github.com/apache/couchdb)) or written documentation that made the project more accessible to others (like @orta [did for CocoaPods](https://realm.io/news/orta-therox-moving-to-oss-by-default/)). Regardless of what they do day-to-day, a maintainer is probably someone who feels responsibility over the direction of the project and is committed to improving it.

A "contributor" could be defined as anyone who comments on an issue or pull request, as [Node.js](https://github.com/nodejs) [defines it](https://medium.com/the-javascript-collection/healthy-open-source-967fa8be7951), whereas other projects would define a contributor as somebody whose pull request was accepted. The term "committer" might be used to distinguish commit access from other forms of contribution.

Use leadership roles to formally recognize people who have made outstanding contributions to your project, regardless of their technical skill. @jacobian, one of [Django](https://github.com/django/django)'s former BDFLs, [once told a crowd at PyCon](https://www.youtube.com/watch?v=hIJdFxYlEKE#t=5m0s) that he is actually a mediocre programmer who joined the project a year after it started, though he's often mistaken as the "inventor" of Django.

## How do I formalize these leadership roles?

Formalizing your leadership roles helps people feel ownership and tells other community members who to look to for help. For a smaller project, designating leaders can be as simple as adding their names to your README or a CONTRIBUTORS text file.

For a bigger project, if you have a website, create a team page or list your project leaders there. For inspiration, [PostgreSQL](https://github.com/postgres/postgres/) has a [comprehensive team page](https://www.postgresql.org/community/contributors/) with short profiles for each contributor.

If your project has a very active contributor community, you might form a "core team" of maintainers, or even subcommittees of people who take ownership of different issue areas. For example, you could have subcommittees focused on security, issue triaging, or community conduct. [Rust](https://github.com/rust-lang/rust) is an example of a project that [moved from having one core team](https://github.com/rust-lang/rfcs/blob/master/text/1068-rust-governance.md) to multiple teams. Let people self-organize and volunteer for the roles they're most excited about, rather than assigning them.

Leadership teams may want to create a designated channel (like on IRC) or meet regularly to discuss the project (like on Gitter or Google Hangout). You can even make those meetings public so other people can listen. [Cucumber-ruby](https://github.com/cucumber/cucumber-ruby), for example, [hosts office hours every week](https://github.com/cucumber/cucumber-ruby/blob/master/CONTRIBUTING.md#talking-with-other-devs).

Once you've established leadership roles, don't forget to document how people can attain them! Establish a clear process for how someone can become a maintainer or join a subcommittee in your project, and write it into your GOVERNANCE.md. Tools like [Vossibility](https://github.com/icecrime/vossibility-stack) can help you publicly track who is (or isn't) making contributions to the project. Documenting this information avoids the community perception that maintainers are a clique that makes its decisions privately.

Finally, if your project is on GitHub, consider moving your project from your personal account to an Organization. [GitHub Organizations](https://github.com/blog/674-introducing-organizations) make it easier to manage permissions and protect your project's legacy.

## When should I give someone commit access?

Some people think you should give commit access to [everybody who makes a contribution](http://felixge.de/2013/03/11/the-pull-request-hack.html). Doing so could encourage more people to feel ownership of your project. On the other hand, especially for big community projects, you may want to only give commit access to people who have demonstrated their commitment. There's no one right way of doing it - do what makes you most comfortable!

If your project is on GitHub, you can use [protected branches](https://help.github.com/articles/about-protected-branches/) to manage who can push to a particular branch, and under which circumstances.

## What are some of the common governance structures for open source projects?

There are three common governance structures associated with open source projects:

* **BDFL:** BDFL stands for "Benevolent Dictator for Life". Under this structure, one person (usually the initial author of the project) has final say on all major project decisions. [Python](https://github.com/python) is a classic example. Smaller projects are probably BDFL by default, because there are only one or two maintainers. A project that originated at a company might also fall into the BDFL category.

* **Meritocracy:** **(Note: the term "meritocracy" carries negative connotations for some communities and has a [complex social and political history](http://geekfeminism.wikia.com/wiki/Meritocracy).)** Under a meritocracy, active project contributors (those who demonstrate "merit") are given a formal decision making role. Decisions are usually made based on pure voting consensus. The meritocracy concept was pioneered by the [Apache Foundation](http://www.apache.org/); [all Apache projects](http://www.apache.org/index.html#projects-list) are meritocracies. Contributions can only be made by individuals representing themselves, not by a company.

* **Liberal contribution:** Under a liberal contribution model, the people who do the most work are recognized as most influential, but this is based on current work and not historic contributions. Major project decisions are made based on a consensus seeking process (discuss major grievances) rather than pure vote, and strive to include as many community perspectives as possible. Popular examples of projects that use a liberal contribution model include [Node.js](https://nodejs.org/en/foundation/) and [Rust](https://www.rust-lang.org/en-US/).

Which one should you use? It's up to you! Every model has advantages and tradeoffs. And although they may seem quite different at first, all three models have more in common than they seem. If you're interested in adopting one of these models, check out these templates:

* [BDFL model template](http://oss-watch.ac.uk/resources/benevolentdictatorgovernancemodel)
* [Meritocracy model template](http://oss-watch.ac.uk/resources/meritocraticgovernancemodel)
* [Node.js's liberal contribution policy](https://medium.com/the-javascript-collection/healthy-open-source-967fa8be7951#.m9ht26e79)

## Do I need governance docs when I launch my project?

There is no right time to write down your project's governance, but it's much easier to define once you've seen your community dynamics play out. The best (and hardest) part about open source governance is that it is shaped by the community!

Some early documentation will inevitably contribute to your project's governance, however, so start writing down what you can. For example, you can define clear expectations for behavior, or how your contributor process works, even at your project's launch.

If you're part of a company launching an open source project, it's worth having an internal discussion before launch about how your company expects to maintain and make decisions about the project moving forward. You may also want to publicly explain anything particular to how your company will (or won't!) be involved with the project.

## Do I need a legal entity to support my project?

You don't need a legal entity to support your open source project unless you're handling money. For example, if you want to create a commercial business, you'll want to set up a C Corp or LLC (if you're based in the US). If you're just doing contract work related to your open source project, you can accept money as a sole proprietor, or set up an LLC (if you're based in the US).

If you want to accept donations for your open source project, you can set up a donation button (using PayPal or Stripe, for example), but the money won't be tax-deductible unless you are a qualifying nonprofit (a 501c3, if you're in the US). Many projects don't wish to go through the trouble of setting up a nonprofit, so they find a nonprofit fiscal sponsor instead. A fiscal sponsor accepts donations on your behalf, usually in exchange for a percentage of the donation. [Software Freedom Conservancy](https://sfconservancy.org/), [Apache Foundation](http://www.apache.org/), [Eclipse Foundation](https://eclipse.org/org/foundation/), and [Open Collective](https://opencollective.com/opensource) are examples of organizations that serve as fiscal sponsors for open source projects.

If your project is closely associated with a certain language or ecosystem, there may also be a related software foundation you can work with. For example, the [Python Software Foundation](https://www.python.org/psf/) helps support [PyPI](https://pypi.python.org/pypi), the Python package manager, and the [Node.js Foundation](https://nodejs.org/en/foundation/) helps support [Express.js](http://expressjs.com/), a Node-based framework.
