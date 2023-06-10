## Style and Specification

We divide the problem into security and general problems:

#### Reporting security issues

Security issues are always treated seriously. As our usual principle, we discourage anyone to spread security issues. If you find a security issue of kubecub, please do not discuss it in public and even do not open a public issue.

Instead we encourage you to send us a private email to [3293172751nss@gmail.com](mailto:3293172751nss@gmail.com) to report this.

#### Reporting general issues

To be honest, we regard every user of kubecubas a very kind contributor. After experiencing kubecub, you may have some feedback for the project. Then feel free to open an issue via [NEW ISSUE](https://github.com/kubecub/kubecub/issues/new/choose).

Since we collaborate project kubecub in a distributed way, we appreciate **WELL-WRITTEN**, **DETAILED**, **EXPLICIT** issue reports. To make the communication more efficient, we wish everyone could search if your issue is an existing one in the searching list. If you find it existing, please add your details in comments under the existing issue instead of opening a brand new one.

To make the issue details as standard as possible, we setup an [ISSUE TEMPLATE](https://github.com/kubecub/kubecub/tree/main/.github/ISSUE_TEMPLATE) for issue reporters. You can find three kinds of issue templates there: question, bug report and feature request. Please **BE SURE** to follow the instructions to fill fields in template.

**There are a lot of cases when you could open an issue:**

+ bug report
+ feature request
+ kubecub performance issues 
+ feature proposal
+ feature design
+ help wanted
+ doc incomplete
+ test improvement
+ any questions on kubecub project 
+ and so on 

Also, we must be reminded when submitting a new question about kubecub, please remember to remove the sensitive data from your post. Sensitive data could be password, secret key, network locations, private business data and so on.

#### Commit Rules

Actually in kubecub, we take two rules serious when committing:

**🥇 Commit Message:**

Commit message could help reviewers better understand what the purpose of submitted PR is. It could help accelerate the code review procedure as well. We encourage contributors to use **EXPLICIT** commit message rather than ambiguous message. In general, we advocate the following commit message type:

We use [Semantic Commits](https://www.conventionalcommits.org/en/v1.0.0/) to make it easier to understand what a commit does and to build pretty change kubecub. Please use the following prefixes for your commits:

+ `docs: xxxx`. For example, "docs: add docs about storage installation".
+ `feature: xxxx`.For example, "feature: make result show in sorted order".
+ `bugfix: xxxx`. For example, "bugfix: fix panic when input nil parameter".
+ `style: xxxx`. For example, "style: format the code style of Constants.java".
+ `refactor: xxxx.` For example, "refactor: simplify to make codes more readable".
+ `test: xxx`. For example, "test: add unit test case for func InsertIntoArray".
+ `chore: xxx.` For example, "chore: integrate travis-ci". It's the type of mantainance change.
+ other readable and explicit expression ways.

On the other side, we discourage contributors from committing message like the following ways:

+ ~~fix bug~~
+ ~~update~~
+ ~~add doc~~

**🥈 Commit Content:**

Commit content represents all content changes included in one commit. We had better include things in one single commit which could support reviewer's complete review without any other commits' help.

In another word, contents in one single commit can pass the CI to avoid code mess. In brief, there are two minor rules for us to keep in mind:

1. avoid very large change in a commit.
2. complete and reviewable for each commit.
3. words are written in lowercase English, not uppercase English or other languages such as Chinese.

No matter what the commit message, or commit content is, we do take more emphasis on code review.

An example for this could be:

```bash
❯ git commit -a -s -m "docs: add a new section to the README"
```

#### PR Description

PR is the only way to make change to kubecub project files. To help reviewers better get your purpose, PR description could not be too detailed. We encourage contributors to follow the [PR template](https://github.com/kubecub) to finish the pull request.

You can find some very formal PR in [RFC](https://github.com/kubecub/kubecub/issues) issues and learn about them.

**📖 Opening PRs:**

+ As long as you are working on your PR, please mark it as a draft
+ Please make sure that your PR is up-to-date with the latest changes in `main`
+ Mention the issue that your PR is addressing (Fix: #{ID_1}, #{ID_2})
+ Make sure that your PR passes all checks

**🈴 Reviewing PRs:**

+ Be respectful and constructive 
+ Assign yourself to the PR 
+ Check if all checks are passing
+ Suggest changes instead of simply commenting on found issues
+ If you are unsure about something, ask the author
+ If you are not sure if the changes work, try them out
+ Reach out to other reviewers if you are unsure about something
+ If you are happy with the changes, approve the PR
+ Merge the PR once it has all approvals and the checks are passing

**⚠️ DCO check:**

We have a DCO check that runs on every pull request to ensure code quality and maintainability. This check verifies that the commit has been signed off, indicating that you have read and agreed to the provisions of the Developer Certificate of Origin. If you have not yet signed off on the commit, you can use the following command to sign off on the last commit you made:

```bash
❯ git commit --amend --signoff
```

Please note that signing off on a commit is a commitment that you have read and agreed to the provisions of the Developer Certificate of Origin. If you have not yet read this document, we strongly recommend that you take some time to read it carefully. If you have any questions about the content of this document, or if you need further assistance, please contact an administrator or relevant personnel.

You can also automate signing off your commits by adding the following to your `.zshrc` or `.bashrc`:

```go
git() {
  if [ $# -gt 0 ] && [[ "$1" == "commit" ]] ; then
     shift
     command git commit --signoff "$@"
  else
     command git "$@"
  fi
}
```

#### Docs Contribution

The documentation for kubecub includes:

+ [README.md](https://github.com/kubecub/community/blob/main/README.md): This file includes the basic information and instructions for getting started with kubecub.
+ [CONTRIBUTING.md](https://github.com/kubecub/community/blob/main/CONTRIBUTING.md): This file contains guidelines for contributing to kubecub's codebase, such as how to submit issues, pull requests, and code reviews.
+ [DEVELOPGUIDE.md](https://github.com/kubecub/community/blob/main/DEVELOPGUIDE.md): This file provides a more in-depth guide to developing kubecub, including information on the project's architecture, coding conventions, and testing practices.
+ [Official Documentation](nsddd.top): This is the official documentation for kubecub, which includes comprehensive information on all of its features, configuration options, and troubleshooting tips.

Please obey the following rules to better format the docs, which would greatly improve the reading experience.

1. Please do not use Chinese punctuations in English docs, and vice versa.
2. Please use upper case letters where applicable, like the first letter of sentences / headings, etc.
3. Please specify a language for each Markdown code blocks, unless there's no associated languages.
4. Please insert a whitespace between Chinese and English words.
5. Please use the correct case for technical terms, such as using `HTTP` instead of http, `MySQL` rather than mysql, `Kubernetes` instead of kubernetes, etc.
6. Please check if there's any typos in the docs before submitting PRs.

## Engage to help anything

We choose GitHub as the primary place for kubecub to collaborate. So the latest updates of kubecub are always here. Although contributions via PR is an explicit way to help, we still call for any other ways.

+ reply to other's [issues](https://github.com/search?q=org%3Akubecub++&type=issues&s=comments&o=desc) if you could;
+ help solve other user's problems;
+ help review other's [PR](https://github.com/search?q=org%3Akubecub++&type=pullrequests&s=comments&o=desc) design; 
+ discuss about kubecub to make things clearer;
+ advocate [kubecub](google.com/search?q=kubecub) technokubecuby beyond GitHub;
+ write kubecubs on kubecub and so on.

In a word, **ANY HELP IS CONTRIBUTION.**

## Release version

Releases of kubecub are done using [Release Please](https://github.com/googleapis/release-please) and [GoReleaser](https://goreleaser.com/). The workflow looks like this:

🎯 A PR is merged to the `main` branch:

+ Release please is triggered, creates or updates a new release PR
+ This is done with every merge to main, the current release PR is updated every time

🎯 Merging the 'release please' PR to `main`:

+ Release please is triggered, creates a new release and updates the change kubecub based on the commit messages
+ GoReleaser is triggered, builds the binaries and attaches them to the release
+ Containers are created and pushed to the container registry

With the next relevant merge, a new release PR will be created and the process starts again

**👀 Manually setting the version:**

If you want to manually set the version, you can create a PR with an empty commit message that contains the version number in the commit message. For example:

Such a commit can get produced as follows: 

````bash
❯ git commit --allow-empty -m "chore: release 0.0.3" -m "Release-As: 0.0.3
````
