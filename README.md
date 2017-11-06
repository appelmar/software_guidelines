# [openeo](http://openeo.org/) software guidelines

Edzer Pebesma, openeo team

This document describes the guidelines for software developers,
written for the [openeo](http://openeo.org) project. This seems
somewhat premature to write before a single line of code has been
written, but this has been promised to the funder of the project.

1. License: all software developed in the openeo project and published on the [openeo github](http://github.com/open-eo/) organisation shall be licensed under the [Apache 2.0 license](LICENSE). If software repositories deviate from this, or contain code or other artifacts that deviates from this, this shall be described in the first paragraph of the `README.md` file.
2. Proof-of-concept versus sustainable: each repository shall indicate whether it contains proof-of-concept code or sustainable code. Proof-of-concept code is meant to work but comes without any quality assurance whatsever. 
3. Sustainable code should undergo standard [quality checks](SOFTWARE_QUALITY.md), and point out its [documentation](DOCUMENTATION.md).
4. Sustainable code shall undergo [code review](REVIEW.md);
no direct commits to master; any commit shall come in the form of
a PR, commit after review.
5. Sustainable code shall be written in a [Test-driven manner](TESTS.md), and repositories shall ath the top of their `README.md` give indication of the degree to which code is covered by tests.
6. [Continuous integration](CI.md) shall be used to indicate code currently passes its test on CI platforms
7. A [Code of conduct](CONDUCT.md) shall describe the rules and constraints to developers and contributors.
