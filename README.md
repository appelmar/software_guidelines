# [openeo](http://openeo.org/) software development guidelines

Edzer Pebesma, openeo team

This document describes the guidelines for software developers,
written for the [openeo](http://openeo.org) project.  Since the
openeo encompasses several programming languages and environments,
this document does not prescribe particular tools or platforms but
instead the general principles and methods behind them.

1. License: all software developed in the openeo project and published on the [openeo github](http://github.com/open-eo/) organisation shall be licensed under the [Apache 2.0 license](LICENSE). If software repositories deviate from this, or contain code or other artifacts that deviates from this, this shall be described in the first paragraph of the `README.md` file.
2. Proof-of-concept versus sustainable: each repository shall indicate whether it contains proof-of-concept code or sustainable code. Proof-of-concept code is meant to work but comes without any quality assurance whatsever. 
3. Sustainable code should undergo standard [quality checks](#software-quality-guidelines), and point out its [documentation](#software-documentation-guidelines)
4. Sustainable code shall undergo [code review](#software-review);
no direct commits to master; any commit shall come in the form of
a PR, commit after review.
5. Sustainable code shall be written in a [Test-driven manner](test-driven-development), and repositories shall ath the top of their `README.md` give indication of the degree to which code is covered by tests.
6. [Continuous integration](#continuous-integration) shall be used to indicate code currently passes its test on CI platforms
7. A [Code of conduct](#contributor-code-of-conduct) describes the rules and constraints to developers and contributors.


## Software quality guidelines

* software shall be written in such a way that another person can understand its intention
* comment lines shall be used sparsely, but effectively
* reuse of unstable or esoteric libraries shall be avoided

## Software documentation guidelines

Software documentation shall include:
* installation instructions
* usages instructions
* explain in detail the intention of the software
* each repository's `README.md` shall point to the documentation


## Software review

* sustainable software development shall take place by always having two persons involved in a change: one person makes a pull request, another person reviews the pull requests and merges it into the master branch.
* software review discussions shall be intelligible for external developers, and serve as implicit documentation for development decisions taken

## Test-driven development


## Continuous integration

Repositories containing running software shall use
an appropriate continuous integration platform, such as
[travis](https://travis-ci.org/) or similar, to show whether the
current build passes all checks. This helps understand contributors
that the software passes tests on an independent platform, and
may give insights in the way the software is compiled, deployed
and tested.

## Contributor Code of Conduct

As contributors and maintainers of this project, we pledge to respect all people who 
contribute through reporting issues, posting feature requests, updating documentation,
submitting pull requests or patches, and other activities.

We are committed to making participation in this project a harassment-free experience for
everyone, regardless of level of experience, gender, gender identity and expression,
sexual orientation, disability, personal appearance, body size, race, ethnicity, age, or religion.

Examples of unacceptable behavior by participants include the use of sexual language or
imagery, derogatory comments or personal attacks, trolling, public or private harassment,
insults, or other unprofessional conduct.

Project maintainers have the right and responsibility to remove, edit, or reject comments,
commits, code, wiki edits, issues, and other contributions that are not aligned to this 
Code of Conduct. Project maintainers who do not follow the Code of Conduct may be removed 
from the project team.

Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by 
opening an issue or contacting one or more of the project maintainers.

This Code of Conduct is adapted from the Contributor Covenant 
(http:contributor-covenant.org), version 1.0.0, available at 
http://contributor-covenant.org/version/1/0/0/
