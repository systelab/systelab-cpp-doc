# Contributing to CSW C++ Task Force

:+1::tada: First off, thanks for taking the time to contribute! :tada::+1:

The following is a set of guidelines for contributing to CSW C++ task force and its libraries. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.


#### Table Of Contents

[Code of Conduct](#code-of-conduct)

[I don't want to read this whole thing, I just have a question!!!](#i-dont-want-to-read-this-whole-thing-i-just-have-a-question)

[What should I know before I get started?](#what-should-i-know-before-i-get-started)
  * [Catalog of libraries](#catalog-of-libraries)
  * [Toolchain](#toolchain)
  * [Conventions and decisions](#conventions-and-decisions)
  * [Roadmap](#roadmap)

[How Can I Contribute?](#how-can-i-contribute)
  * [Reporting Bugs](#reporting-bugs)
  * [Suggesting Enhancements](#suggesting-enhancements)
  * [Pull Requests](#pull-requests)


## Code of Conduct

This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## I don't want to read this whole thing I just have a question!!!

> **Note:** Please don't file an issue to ask a question. You'll get faster results by using the resources below.

We have an official channel on Microsoft Teams and where the community chimes in with helpful advice if you have questions.


## What should I know before I get started?

### Catalog of libraries

C++ task force is a large open source project and it's made up of multiple repositories. When you initially consider contributing, you might be unsure about which repository should go the functionality you want to change or report a bug for. The [catalog of libraries](CATALOG.md) should help you with that.

### Toolchain

Check our [toolchain](TOOLCHAIN.md) document for a complete list of the set of tools we work with.

### Conventions and decisions

The following resources may help you with the conventions we are used as well as the decisions taken:
* [Coding guidelines](CODING_GUIDELINES.md)
* [Design decisions](DESIGN_DECISIONS.md)

### Roadmap

Next steps of the task force are defined and updated on the [roadmap](https://github.com/systelab/systelab-cpp-doc/projects) for the current year.


## How Can I Contribute?

### Reporting Bugs

This section guides you through submitting a bug report for a C++ library. Following these guidelines helps maintainers and the community understand your report :pencil:, reproduce the behavior :computer: :computer:, and find related reports :mag_right:.

Before creating bug reports, please check the list of open bugs of the library repository as you might find out that you don't need to create one. 

> **Note:** If you find a **Closed** issue that seems like it is the same thing that you're experiencing, open a new issue and include a link to the original issue in the body of your new one.

#### How Do I Submit A (Good) Bug Report?

Bugs are tracked as [GitHub issues](https://guides.github.com/features/issues/) or [Bitbucket issues](https://bitbucket.org/). After you've determined [which repository](#catalog-of-libraries) your bug is related to, create an issue on that repository and provide the following information by filling in the template.

Explain the problem and include additional details to help maintainers reproduce the problem:

* **Use a clear and descriptive title** for the issue to identify the problem.
* **Describe the exact steps which reproduce the problem** in as many details as possible. For example, start by explaining how you use the library, e.g. which API method you used, or how you configured it. When listing steps, **don't just say what you did, but explain how you did it**. 
* **Provide specific examples to demonstrate the steps**. Include links to files or GitHub projects, or copy/pasteable snippets, which you use in those examples. If you're providing snippets in the issue, use [Markdown code blocks](https://help.github.com/articles/markdown-basics/#multiple-lines).
* **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
* **Explain which behavior you expected to see instead and why.**
* **If you're reporting a crash**, include a crash report with a stack trace from the operating system. 
* **If the problem is related to performance or memory**, include a CPU profile capture with your report.
* **If the problem wasn't triggered by a specific action**, describe what you were doing before the problem happened and share more information using the guidelines below.

### Suggesting Enhancements

This section guides you through submitting an enhancement suggestion for Atom, including completely new features and minor improvements to existing functionality. Following these guidelines helps maintainers and the community understand your suggestion :pencil: and find related suggestions :mag_right:.

Before creating enhancement suggestions, please check the list of issues of the library repository as you might find out that you don't need to create one. 

#### How Do I Submit A (Good) Enhancement Suggestion?

Enhancement suggestions are tracked as [GitHub issues](https://guides.github.com/features/issues/). After you've determined [which repository](#catalog-of-libraries) your enhancement suggestion is related to, create an issue on that repository and provide the following information:

* **Use a clear and descriptive title** for the issue to identify the suggestion.
* **Provide a step-by-step description of the suggested enhancement** in as many details as possible.
* **Provide specific examples to demonstrate the steps**. Include copy/pasteable snippets which you use in those examples, as [Markdown code blocks](https://help.github.com/articles/markdown-basics/#multiple-lines).
* **Describe the current behavior** and **explain which behavior you expected to see instead** and why.

### Pull Requests

The process described here has several goals:

- Maintain quality of libraries
- Fix problems that are important to users
- Engage the community in working toward the best possible library
- Enable a sustainable system for libraries' maintainers to review contributions

Please follow these steps to have your contribution considered by the maintainers:

1. This task force is aligned with the feature-branch strategy. The branch naming convention is "bugfix- or feature-" plus the issue number in Github or Bitbucket.
 > For example: bugfix-200

2. Follow all instructions in [the template](PULL_REQUEST_TEMPLATE.md)

3. The changes can be tested in your local before publishing. Make sure all automated tests pass before that.

4. After you submit your pull request, verify that all [status checks](https://help.github.com/articles/about-status-checks/) are passing <details><summary>What if the status checks are failing?</summary>If a status check is failing, and you believe that the failure is unrelated to your change, please leave a comment on the pull request explaining why you believe the failure is unrelated. A maintainer will re-run the status check for you. If we conclude that the failure was a false positive, then we will open an issue to track that problem with our status check suite.</details>

5. While the prerequisites above must be satisfied prior to having your pull request reviewed, the reviewer(s) may ask you to complete additional design work, tests, or other changes before your pull request can be ultimately accepted.

6. Before merging the pull request, the master branch needs to be merged into current.

7. Once it's merged, the author must transition it to the status "Ready to test" in the [project](https://github.com/systelab/systelab-components/projects)

8. Based upon need, the library will be published into the npm repository. This process must be done by an authorized user.
