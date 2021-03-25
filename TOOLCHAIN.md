# Toolchain

This document describes the collection of tools used for the different activities related with the lifecycle of libraries governed by the CSW C++ task force.


## Communication

Make use of the "CSW-TF C++" team on Microsoft Teams to announce or discuss anything related with the C++ task force. 


## Source control management (SCM)

C++ task force works with 2 types of [git](https://git-scm.com/) platforms:
* *GitHub*: For open source repositories (i.e foundation, adapters, ...)
* *Bitbucket*: For private repositories (i.e core business code, cybersecurity, ...)

Both cloud platforms integrate issue trackers on each repository that will be used for change & defect management. Similarly, code reviews will be performed by the built-in pull request mechanism.


## Continuous integration

There are different CI tools involved on the platform used on each repository:
* [Travis CI](https://travis-ci.org/github/systelab): Used for Linux & MacOS configurations (only open source)
* [AppVeyor](https://ci.appveyor.com/): Used for Windows configurations (only open source)
* [GitHub Actions](https://github.com/features/actions): Used to generate automated documentation (only open source)
* [Jenkins](https://www.jenkins.io/): Used for complete CI of private repositories


## Cross platform

Whenever possible, repositories are configured to be cross-platform by making use of [cmake](https://cmake.org/).

See [configurations matrix](CONFIGURATIONS_MATRIX.md) for details about the environment used on each project.


## Package manager

Conan is the package manager to be used under the scope of this task force. It can be used with the following purposes:

* Dependency management: dependencies 

* Deploy


 Every library should be prepared to be deployed as a Conan package







## Automated testing

[GoogleTest](https://google.github.io/googletest/) is the reference test automation framework. Thanks to the mocking feature, it is ideal for test automation. 

 


## Documentation

All repositories should contain a README.md file describing:
* Purpose of the repository/library
* List of features provided
* How to setup (i.e conan, build from sources, ...)
* Usage instructions (i.e code snippets are usually very helpful)

