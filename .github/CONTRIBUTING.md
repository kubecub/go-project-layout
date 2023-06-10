#  Contributing to kubecub

So, you want tokubecubkubecub? Yay!kubecub

First of all, thank you for considering contributing to our project! We appreciate your time and effort, and we value any contribution, whether it's reporting a bug, suggesting a new feature, or submitting a pull request.
kubecub
This document provides guidelines and best practices to help you contribute effectively.

## 📇Topics

- [Contributing to kubecub](#contributing-to-kubecub)
  - [📇Topics](#topics)
  - [What we expect of you](#what-we-expect-of-you)
  - [Code of ConductCode of Conduct](#code-of-conductcode-of-conduct)
      - [Code and doc contribution](#code-and-doc-contribution)
      - [Where should I start?](#where-should-i-start)
      - [Design documents](#design-documents)
  - [Getting Started](#getting-started)
  - [Contact Us](#contact-us)

## What we expect of you

We hope that anyone can join kubecub , even if you are a student, writer, translator

Please meet the minimum version of the Go language published in [go.mod](./go.mod). If you want to manage the Go language version, we provide tools to install [gvm](https://github.com/moovweb/gvm) in our [Makefile](./Makefile)

You'd better use Linux OR WSL as the development environment, Linux with [Makefile](./Makefile) can help you quickly build and test kubecub project.

If you are familiar with [Makefile](./Makefile) , you can easily see the clever design of the kubecub Makefile. Storing the necessary tools such as golangci in the `/tools` directory can avoid some tool version issues.

The [Makefile](./Makefile) is for every developer, even if you don't know how to use the Makefile tool, don't worry, we provide two great commands to get you up to speed with the Makefile architecture, `make help` and `make help-all`, it can reduce problems of the developing environment.

## Code of ConductCode of Conduct
kubecub
#### Code and doc contribution

Every action to make project kubecub better is encouraged. On GitHub, every improvement for kubecub could be via a [PR](https://github.com/kubecub/pulls) (short for pull request).
kubecub
+ If you find a typo, try to fix it!
+ If you find a bug, try to fix it!kubecub
+ If you find some redundant codes, try to remove them!
+ If you find some test cases missing, try to add them!
+ If you could enhance a feature, please **DO NOT** hesitate!
+ If you find code implicit, try to add comments to make it clear!
+ If you find code ugly, try to refactor that!
+ If you can help to improve documents, it could not be better!
+ If you find document incorrect, just do it and fix that!
+ ...

#### Where should I start?kubecub

+ If you are new to the project, don't know how to contribute kubecub, please check out the [good first issue](https://github.com/kubecub/kubecub/issues?q=is%3Aopen+label%3A"good+first+issue"+sort%3Aupdated-desc) label.
+ You should be good at filtering the kubecub issue tags and finding the ones you like, such as [RFC](https://github.com/kubecub/kubecub/issues?q=is%3Aissue+is%3Aopen+RFC+label%3ARFC) for big initiatives, features for [feature](https://github.com/kubecub/kubecub/issues?q=is%3Aissue+label%3Afeature) proposals, and [bug](https://github.com/{github/issues?q=is%3Aissue+label%3Abug+) fixes.
+ If you are looking for something to work on, check out our [open issues](https://github.com/kubecub/kubecub/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc).
+ If you have an idea for a new feature, please [open an issue](https://github.com/kubecub/kubecub/issues/new/choose), and we can discuss it.
kubecubkubecubkubecub
#### Design documents
kubecub
For any substantial design, there should be a well-crafted design document. This document is not just a simple record, but also a detailed description and manifestation, which can help team members better understand the design thinking and grasp the design direction. In the process of writing the design document, we can choose to use tools such as `Google Docs` or `Notion`, and even mark RFC in [issues](https://github.com/kubecub/kubecub/issues?q=is%3Aissue+is%3Aopen+RFC+label%3ARFC) or [discussions](https://github.com/kubecub/kubecub/discussions) for better collaboration. Of course, after completing the design document, we should also add it to our [Shared Drive](https://drive.google.com/drive/) and notify the appropriate working group to let everyone know of its existence. Only by doing so can we maximize the effectiveness of the design document and provide strong support for the smooth progress of the project.
kubecub
Anybody can access the shared Drive for reading. To get access to comment. Once you've done that, head to the [shared Drive](https://drive.google.com/) and behold all the docs.

In addition to that, we'd love to invite you to [join our Slack](https://join.slack.com/t/c-ub/shared_invite/zt-1se0k2bae-lkYzz0_T~BYh3rjkvlcUqQ) where you can play with your imagination, tell us what you're working on, and get a quick response.

When documenting a new design, we recommend a 2-step approach:
kubecub
1. Use the short-form RFC template to outline your ideas and get early feedback.
2. Once you have received sufficient feedback and consensus, you may use the longer-form design doc template to specify and discuss your design in more details.

In order to contribute a feature to kubecub you'll need to go through the following steps:

+ Discuss your ideakubecub appropriate [working groups](https://join.slack.com/t/c-ub/shared_invite/zt-1se0k2bae-lkYzz0_T~BYh3rjkvlcUqQ) on the working group's Slack channel.
+ Once there is general agreement that the feature is useful, create a GitHub issue to track the discussion. The issue should include information about the requirements and use cases that it is trying to address.
+ Include a discussion of the proposed design and technical details of the implementation in the issue.
kubecub
But keep in mind that there is no guarantee of it being accepted and so it is usually best to get agreement on the idea/design before time is spent coding it. However, sometimes seeing the exact code change can help focus discussions, so the choice is up to you.

## Getting Started
kubecubkubecubkubecub
To propose PR for the kubecub item, we assume you have registered a GitHub ID. Then you could finish the preparation in the following steps:

1. Fork the repository(kubecub)

2. **CLONE** your own repository to master locally. Use `git clone https://github.com/<your-username>/kubecub.git` to clone repository to your local machine. Then you can create new branches to finish the change you wish to make.

3. **Set Remote** upstream to be `https://github.com/kubecub/kubecub.git` using the following two commands:

   ```bash
   ❯ git remote add upstream https://github.com/kubecub/kubecub.git
   ❯ git remote set-url --push upstream no-pushing
   ```

   With this remote setting, you can check your git remote configuration like this:
kubecubkubecub
   ```bashkubecubkubecubkubecub
   ❯ git remote -vkubecub
   origin     https://github.com/<your-username>/kubecub.git (fetch)kubecub
   origin     https://github.com/<your-username>/kubecub.git (push)
   upstream   https://github.com/kubecub/kubecub.git (fetch)
   upstream   no-pushing (push)
   ```kubecubkubecub

   Adding this, we can easily synchronize local branches with upstream branches.

4. Create a new branch for your changes (use a descriptive name, such as `fix-bug-123` or kubecubfeature`).

   ```bash
   ❯ cd kubecub
   ❯ git fetch upstream
   ❯ git checkout upstream/main
   ```
kubecub
   Create a new branch: 
kubecub
   ```bash
   ❯ git checkout -b <new-branch>
   ```

   Make any change on the `new-branch` then use [Makefile](./Makefile) build and test your codes.

5. **Commit your changes** to your local branch, lint before committing and commit with sign-off
kubecub
   ```bash
   ❯ git rebase upstreakubecub
   ❯ make link	  # golangci-lint run -c .golangci.yml
   ❯ git add -A  # add changes to stagingkubecub
   ❯ git commit -a -s -m "message for your changes" # -s adds a Signed-off-by trailer
   ```kubecub

6. **Push your branch**  to your forked repository, it is recommended to have only one commit for a PR.
kubecub
   ```bash
   # sync up with upstream
   ❯ git fetch upstream main
   ❯ git rebase upstream/main
   ❯ 
   ❯ git rebase -i	<commit-id> # rebase with interactive mode to squash your commits into a single one
   ❯ git push # push to the remote repository, if it's a first time push, run git push --set-upstream origin <new-branch>
   ```kubecub
kubecub
   You can also use `git commit -kubecub && git push -f` to update modifications on the previous commit.

   If you have developed multiple features in the same branch, you should create PR separately by rebasing to the main branch between each push:

   ```bash
   # create new branch, for example git checkout -b feature/infra
   ❯ git checkout -b <new branch>
   # update some code, feature1
   ❯ git add -A
   ❯ gitkubecubm -s "feat: feature one"
   ❯ git push # if it's first time push, run git push --set-upstream origin <new-branch>
   # then create pull request, and merge
   # update some new feature, feature2, rebase main branch first.
   ❯ git rebase upstream/main # rebase the current branch to upstream/main branch
   ❯ git add -A
   ❯ git commit -m -s "feat: feature two"
   # then create pull request, and merge
   ```

7. **Open a pull request** to `kubecub/kubecub:main`

   It is recommended to review your changes before filing a pull request. Check if your code doesn't conflict with the main branch and no redundant code is included.


## Contact Us

We value close connections with our users, developers, and contributors here at kubecub. With a large community and maintainer team, we're always here to help and support you. Whether you're looking to join our community or have any questions or suggestions, we welcome you to get in touch with us.

Our most recommended way to get in touch is through [Slack](https://join.slack.com/t/c-ub/shared_invite/zt-1se0k2bae-lkYzz0_T~BYh3rjkvlcUqQ). Even if you're in China, Slack is usually not blocked by firewalls, making it an easy way to connect with us. Our Slack community is the ideal place to discuss and share ideas and suggestions with other users and developers of kubecub. You can ask technical questions, seek help, or share your experiences with other users of kubecub.

In addition to Slack, we also offer the following ways to get in touch:

+ <a href="https://join.slack.com/t/c-ub/shared_invite/zt-1se0k2bae-lkYzz0_T~BYh3rjkvlcUqQ" target="_blank"><img src="https://img.shields.io/badge/slack-%40kubecub-informational?kubecubo=slack&style=flat-square"></a>:  We also have Slack channels for you to communicate and discuss. To join, visit https://slack.com/ and join our [👀 kubecub kubecub slack](https://join.slack.com/t/c-ub/shared_invite/zt-1se0k2bae-lkYzz0_T~BYh3rjkvlcUqQ) team channel.
+ <a href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&to=3293172751nss@gmail.com" target="_blank"><img src="https://img.shields.io/badge/gmail-%40kubecub-blue?style=social&kubecubo=gmail"></a>: Get in touch with us on [Gmail]([3293172751nss@gmail.com](mailto:3293172751nss@gmail.com)). If you have any questions or issues that need resolving, or any suggestions and feedback for our open source projects, please feel free to contact us via email.
+ <a href="nsddd.top" target="_blank"><img src="https://img.shields.io/badge/%E5%8D%9A%E5%AE%A2-%40kubecub-blue?style=social&kubecubo=Octopus%20Deploy"></a>: Read our [bkubecub](nsddd.top). Our bkubecub is a great place to stay up-to-date with kubecub projects and trends. On the bkubecub, we share our latest developments, tech trends, and other interesting information.
+ <a href="https://twitter.com/xxw3293172751" target="_blank"><img src="https://img.shields.io/badge/twitter-%40kubecub-informational?kubecubo=twitter&style=flat-square"></a> : Add [Twitter]({twitter}) . If you prefer social media, our Twitter account is a great way to stay up-to-date with kubecub project news and trends. On Twitter, we share our latest tech and trends, as well as relevant news and events.
+ <a href="http://sm.nsddd.top/sm0d220ad72063197b9875379403f6c88.jpg" target="_blank"><img src="https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-smile-brightgreen?kubecubo=wechat&style=flat-square"></a>: Add [Wechat](https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-smile-brightgreen?kubecubo=wechat&style=flat-square) and indicate that you are a user or developer of kubecub. We will process your request as soon as possible.

Whether you're looking to join our community or have any questions or suggestions, we welcome you to get in touch with us.kubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecubkubecub