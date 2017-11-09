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
4. Sustainable code shall undergo [code review](REVIEW.md);
no direct commits to master; any commit shall come in the form of
a PR, commit after review.
5. Sustainable code shall be written in a [Test-driven manner](TESTS.md), and repositories shall ath the top of their `README.md` give indication of the degree to which code is covered by tests.
6. [Continuous integration](CI.md) shall be used to indicate code currently passes its test on CI platforms
7. A [Code of conduct](CONDUCT.md) describes the rules and constraints to developers and contributors.


## Sofware quality guidelines

* software shall be written in such a way that another person can understand its intention
* comment lines shall be used sparsely, but effectively
* reuse of unstable or esoteric libraries shall be avoided

## Software documentation guidelines

Software documentation shall include:
* installation instructions
* usages instructions
* explain in detail the intention of the software
* each repository's `README.md` shall point to the documentation


