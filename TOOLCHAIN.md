# Toolchain

This document describes the collection of tools used for the different activities related with the lifecycle of libraries governed by the CSW C++ task force.


## Communication

Make use of the "CSW-TF C++" team on Microsoft Teams to announce or discuss anything related with the C++ task force. 


## Source Control Management

C++ task force works with 2 types of [git](https://git-scm.com/) platforms:
* *GitHub*: For open source repositories (i.e foundation, adapters, ...)
* *Bitbucket*: For private repositories (i.e core business code, cybersecurity, ...)

Both cloud platforms integrate issue trackers on each repository that will be used for change & defect management. Similarly, code reviews will be performed by the built-in pull request mechanism.


## Continuous integration

There are different tools involved on the continuous integration used on each repository:
* [Travis CI](https://travis-ci.org/github/systelab): Used for Linux & MacOS configurations (only open source)
* [AppVeyor](https://ci.appveyor.com/): Used for Windows configurations (only open source)
* [GitHub Actions](https://github.com/features/actions): Used to generate automated documentation (only open source)
* [Jenkins](https://www.jenkins.io/): Used for complete CI of private repositories

> Pending to evaluate if it's worth to move all CI to GitHub Actions, thus the toolchain will be simplified.


## Cross platform

Whenever possible, repositories are configured to be cross-platform by making use of [cmake](https://cmake.org/).

See [configurations matrix](CONFIGURATIONS_MATRIX.md) for details about the different environments used on CSW projects.


## Package manager & artifacts

[Conan](https://conan.io/) is "de facto" standard package manager for C++. It should be used in task force libraries to:
* Manage and retrieve dependencies
* Pack binaries and deploy them to an artifacts repository

Thus, every library should contain a conan recipe and be prepared for deployment as a Conan package. However, the artifacts repository will vary depending on the type of repo. While binaries of private libraries will be uploaded to [CSW Artifactory](https://artifactory.systelab.net/), for open source repositories the binaries should go to [JFrogPlatform](http://systelab.jfrog.io/)


## Automated testing

[GoogleTest](https://google.github.io/googletest/) is the reference test automation framework of this task force. Thanks to its mocking feature (GMock), it is ideal for creating unit tests. Nevertheless, it can be used also to build tests that have a wider scope such as component tests or integration tests.

It is not possible to define a general rule for the amount of automated test required, so this will be evaluated for each particular case. However, the philosophy should be about testing as much as possible in an automated manner.

Thanks to [Codecov](https://app.codecov.io/), line code coverage will be measured for GitHub projects. Despite not having an specific target value, reports from this tool can be used on pull requests to detect missing scenarios on the created test suites. Moreover, when a library has a coverage below 80%, it is a smell that probably there are some tests missing.


## Code quality

In order to find bugs as soon as possible, code of task force repositories will be statically analyzed on every build. This will be achieved by means of CppCheck. However, different tools will be used to display the output reports of this type of analysis:

* [Codacy](https://app.codacy.com/organizations/gh/systelab/repositories) will be used for open source libraries
* [SonaQube](https://sonarq.systelab.net/) will be the tool to monitor private repositories

> Still pending to define quality gates for this type of analysis


## Documentation

All repositories should contain a `README.md` file describing:
* Purpose of the repository/library
* List of features provided
* How to setup (i.e conan, build from sources, ...)
* Usage instructions (i.e code snippets are usually very helpful)

