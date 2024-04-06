# Filippo's open source maintenance policy
Link: https://filippo.io/maintenance  
Updated: April 2024

This policy explains how I work on my open source projects, what you should expect from me as a maintainer, and how to contribute.

### I work in cycles

I work on a number of codebases, and the way to apportion attention that works best with my brain is to batch up work, focus on a project for one to four weeks, and then move to a different project. This reduces context switching overhead and gives me time to consider overall trends.

This means there might be extended periods during which I am not actively working on a specific project. This does NOT mean the project is unmaintained: I still _read_ every issue filed, and would react promptly to urgent issues, such as security reports or any breakage that makes a project not work anymore for its _current_ users.

If a project is unmaintained, it will be either archived or moved to [FiloSottile/mostly-harmless](https://github.com/FiloSottile/mostly-harmless).

### Projects have a precise scope

Most of my projects are meant to be simple solutions to a specific problem, and I generally try to resist scope creep.

I understand that might make them not a good fit for you, and that’s ok. Feel free to open a discussion or a feature request, but please understand if we conclude that the issue is out of scope. Forks are welcome!

This is critical both to keep the UX simple, and to keep the maintenance burden manageable.

### Well researched issues are gold

The most useful contributions are detailed issue reports. The more you can tell us about environment and expectations the better. I truly appreciate when users investigate further, or do the work of checking how other implementations behave, or what the relevant specifications say.

Even if you can’t do the extra work, feel free to open an issue. I don’t resent any issue, they’re all gifts (but as gifts they don’t entitle you to a response).

### Experience reports are gems

Even if something might look like it’s working as intended, or if you’re encountering a non-technical issue, I invite you to file an experience report.

It can be as simple as “this error was confusing, even if I figured it out” or as high-level as “getting started was a mess, here are all the things I tried” or as specific as “when I try to use this for this workflow it’s very clunky”.

Focus on your experience, not on the solution. Oftentimes the solution will need to take into account the needs of other stakeholders, or solve multiple issues at once, but having a clear idea of a problem is the first step.

Maybe we will conclude there’s nothing we can do within the project’s scope (see above), but every experience report informs how I think about the project.

If you want to contribute but don’t know where to start, try to use the project from scratch keeping a friction log of all the things that you found confusing or difficult or unclear, and then share that.

### PRs might get reimplemented

Unlike some projects, I *do not* prefer PRs to issues, for a number of reasons.

* Working in batches (see above) means you might have to wait a while before I review a PR, and you might have moved on to other work by then.
* I don’t have the bandwidth for long review cycles, but I am also very particular about the code I accept into a project, since it will be on me to maintain it.
* Cryptography and security projects require an unusually high degree of code review.
* Contributors naturally focus on their use case and circumstances when writing patches, which might need to be adapted to serve other project users.
* I am generally not trying to build large contributor communities around most of my projects, as they are small scoped tools (see above).

All together, this means that detailed issues are usually more useful to me than PRs, and while you’re welcome to open a PR as a way to demonstrate an issue, **you should expect it to be reimplemented rather than merged**. Please don’t take this personally. I try to use `Co-authored-by` lines liberally to share credit where possible.

There are some exceptions, like support for operating systems I am not familiar with, or features I am not well-equipped to implement. We can discuss those cases in the issue tracker. I am also usually happy to merge trivial/short changes.

### Funding

I’m a [professional Open Source maintainer](https://words.filippo.io/professional-maintainers/). If your company might be interested in enabling my work, in the [reciprocal value of a direct line to a maintainer](https://words.filippo.io/dispatches/reciprocal/), and in unlimited access to my expertise, reach out to discuss a retainer! 📨

_I believe the critical role of open source maintainer can develop into a real profession, commanding compensation in line with that of a senior software engineer, charging companies that rely on open source projects and wish to get access to the maintainer's unique and extensive expertise._

**I don't rely on crowdfunding for sustainability, so I generally don't solicit donations from individuals**. If you wish to express gratitude or encourage my work, send me a postcard! 📮

> Filippo Valsorda  
> 9450 SW Gemini Dr #52960  
> Beaverton, Oregon 97008-7105  
> USA

### Conduct

Most of my projects don’t have a formal code of conduct, but I uphold the values of the [Go Community Code of Conduct](https://go.dev/conduct) and I have a zero-tolerance policy for toxic behavior.

Comments that create an unwelcoming environment will lead to a ban. This is my garden, you can go be a jerk elsewhere.

### Security

Please email me privately at security@filippo.io to report a potential security issue. If you’re not sure if something is a security issue, reach out! You should expect a reply within a week, usually much quicker.

I am happy with standard ninety days disclosure timelines, or with embargoes no longer than nine months. I will produce security advisories and file CVEs for any issue I consider a security issue.

I know projects are not entitled to free security research or coordinated disclosure, and I appreciate the contribution of reporters. I do not offer bug bounties at this time.
