# Contributing to Centipede Royale
:+1::tada: First off, thanks for taking the time to contribute! :tada::+1:
The following is a set of guidelines for contributing to ghProfileSearch and its packages, which are hosted in the [CentipedeRoyale](https://github.com/longttran/thegame) on GitHub. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.
#### Table Of Contents
[Code of Conduct](#)
[I don't want to read this whole thing, I just have a question!!!](#)
[What should I know before I get started?](#)
 * [ProfileSearch and Packages](#)
 * [Design Decisions](#)
[How Can I Contribute?](#)
 * [Reporting Bugs](#)
 * [Suggesting Enhancements](#)
 * [Your First Code Contribution](#)
 * [Pull Requests](#)
[Styleguides](#)
 * [Git Commit Messages](#)
 * [JavaScript Styleguide](#)
 * [CoffeeScript Styleguide](#)
 * [Specs Styleguide](#)
 * [Documentation Styleguide](#)
[Additional Notes](#)
 * [Issue and Pull Request Labels](#)
 
## Code of Conduct

This project and everyone participating in it is governed by the [Centipede Royale](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## How Can I Contribute?

### Reporting Bugs

This section guides you through submitting a bug report for CentipedeRoyale. Following these guidelines helps maintainers and the community understand your report :pencil:, reproduce the behavior :computer: :computer:, and find related reports :mag_right:.

Before creating bug reports, please check [this list](#before-submitting-a-bug-report) as you might find out that you don't need to create one. When you are creating a bug report, please [include as many details as possible](#how-do-i-submit-a-good-bug-report). Fill out [the required template](https://github.com/centipede-royale/CentipedeRoyale/blob/master/.github/ISSUE_TEMPLATE/Bug_report.md), the information it asks for helps us resolve issues faster.

> **Note:** If you find a **Closed** issue that seems like it is the same thing that you're experiencing, open a new issue and include a link to the original issue in the body of your new one.

#### Before Submitting A Bug Report

* **Check the [debugging guide](#).** You might be able to find the cause of the problem and fix things yourself. Most importantly, check if you can reproduce the problem [in the latest version of CentipedeRoyale](#), if the problem happens when you run CentipedeRoyale in [safe mode](#), and if you can get the desired behavior by changing [CentipedeRoyales or packages' config settings](#).
* **Check the [FAQs on the forum](https://github.com/centipede-royale/CentipedeRoyale)** for a list of common questions and problems.
* **Determine [which repository the problem should be reported in](#)**.
* **Perform a [cursory search](https://github.com/centipede-royale/CentipedeRoyale)** to see if the problem has already been reported. If it has **and the issue is still open**, add a comment to the existing issue instead of opening a new one.

#### How Do I Submit A (Good) Bug Report?

Bugs are tracked as [GitHub issues](https://guides.github.com/features/issues/). After you've determined [which repository](#) your bug is related to, create an issue on that repository and provide the following information by filling in [the template](https://github.com/centipede-royale/CentipedeRoyale/blob/master/.github/ISSUE_TEMPLATE/Bug_report.md).

Explain the problem and include additional details to help maintainers reproduce the problem:

* **Use a clear and descriptive title** for the issue to identify the problem.
* **Describe the exact steps which reproduce the problem** in as many details as possible. For example, start by explaining how you started CentipedeRoyale, e.g. which command exactly you used in the terminal, or how you started CentipedeRoyale otherwise. When listing steps, **don't just say what you did, but explain how you did it**. For example, if you moved the cursor to the end of a line, explain if you used the mouse, or a keyboard shortcut or an CentipedeRoyale command, and if so which one?
* **Provide specific examples to demonstrate the steps**. Include links to files or GitHub projects, or copy/pasteable snippets, which you use in those examples. If you're providing snippets in the issue, use [Markdown code blocks](https://help.github.com/articles/markdown-basics/#multiple-lines).
* **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
* **Explain which behavior you expected to see instead and why.**
* **Include screenshots and animated GIFs** which show you following the described steps and clearly demonstrate the problem. If you use the keyboard while following the steps, **record the GIF with the [Keybinding Resolver](https://centipede-royale.github.io/CentipedeRoyale/) shown**. You can use [this tool](https://www.cockos.com/licecap/) to record GIFs on macOS and Windows, and [this tool](https://github.com/colinkeenan/silentcast) or [this tool](https://github.com/GNOME/byzanz) on Linux.
* **If you're reporting that CentipedeRoyale crashed**, include a crash report with a stack trace from the operating system. On macOS, the crash report will be available in `Console.app` under "Diagnostic and usage information" > "User diagnostic reports". Include the crash report in the issue in a [code block](https://help.github.com/articles/markdown-basics/#multiple-lines), a [file attachment](https://help.github.com/articles/file-attachments-on-issues-and-pull-requests/), or put it in a [gist](https://gist.github.com/) and provide link to that gist.
* **If the problem is related to performance or memory**, include a [CPU profile capture](https://github.com/centipede-royale/CentipedeRoyale) with your report.
* **If Chrome's developer tools pane is shown without you triggering it**, that normally means that you have a syntax error in one of your themes or in your `styles.less`. Try running in [Safe Mode](#) and using a different theme or comment out the contents of your `styles.less` to see if that fixes the problem.
* **If the problem wasn't triggered by a specific action**, describe what you were doing before the problem happened and share more information using the guidelines below.

Provide more context by answering these questions:

* **Can you reproduce the problem in [safe mode](#)?**
* **Did the problem start happening recently** (e.g. after updating to a new version of CentipedeRoyale) or was this always a problem?
* If the problem started happening recently, **can you reproduce the problem in an older version of CentipedeRoyale?** What's the most recent version in which the problem doesn't happen? You can download older versions of CentipedeRoyale from [the releases page](#).
* **Can you reliably reproduce the issue?** If not, provide details about how often the problem happens and under which conditions it normally happens.
* If the problem is related to working with files (e.g. opening and editing files), **does the problem happen for all files and projects or only some?** Does the problem happen only when working with local or remote files (e.g. on network drives), with files of a specific type (e.g. only JavaScript or Python files), with large files or files with very long lines, or with files in a specific encoding? Is there anything else special about the files you are using?

Include details about your configuration and environment:

* **Which version of CentipedeRoyale are you using?** You can get the exact version by running `centipede-royale -v` in your terminal, or by starting CentipedeRoyale and running the `Application: About` command from the [Command Palette](#).
* **What's the name and version of the OS you're using**?
* **Are you running CentipedeRoyale in a virtual machine?** If so, which VM software are you using and which operating systems and versions are used for the host and the guest?
* **Which [packages](#) do you have installed?** You can get that list by running `apm list --installed`.
* **Are you using [local configuration files](#)** `config.cson`, `keymap.cson`, `snippets.cson`, `styles.less` and `init.coffee` to customize CentipedeRoyale? If so, provide the contents of those files, preferably in a [code block](https://help.github.com/articles/markdown-basics/#multiple-lines) or with a link to a [gist](https://gist.github.com/).
* **Are you using CentipedeRoyale with multiple monitors?** If so, can you reproduce the problem when you use a single monitor?
* **Which keyboard layout are you using?** Are you using a US layout or some other layout?

### Suggesting Enhancements

This section guides you through submitting an enhancement suggestion for CentipedeRoyale, including completely new features and minor improvements to existing functionality. Following these guidelines helps maintainers and the community understand your suggestion :pencil: and find related suggestions :mag_right:.

Before creating enhancement suggestions, please check [this list](#before-submitting-an-enhancement-suggestion) as you might find out that you don't need to create one. When you are creating an enhancement suggestion, please [include as many details as possible](#how-do-i-submit-a-good-enhancement-suggestion). Fill in [the template](https://github.com/centipede-royale/CentipedeRoyale/blob/master/.github/ISSUE_TEMPLATE/Feature_request.md), including the steps that you imagine you would take if the feature you're requesting existed.

#### Before Submitting An Enhancement Suggestion

* **Check the [debugging guide](https://github.com/centipede-royale/CentipedeRoyale/)** for tips — you might discover that the enhancement is already available. Most importantly, check if you're using [the latest version of CentipedeRoyale](https://github.com/centipede-royale/CentipedeRoyale) and if you can get the desired behavior by changing [CentipedeRoyale's or packages' config settings](https://github.com/centipede-royale/CentipedeRoyale).
* **Check if there's already [a package](https://github.com/centipede-royale/CentipedeRoyale) which provides that enhancement.**
* **Determine [which repository the enhancement should be suggested in](#centipede-royale).**
* **Perform a [cursory search](https://github.com/search)** to see if the enhancement has already been suggested. If it has, add a comment to the existing issue instead of opening a new one.

#### How Do I Submit A (Good) Enhancement Suggestion?

Enhancement suggestions are tracked as [GitHub issues](https://guides.github.com/features/issues/). After you've determined [which repository](#centipede-royale) your enhancement suggestion is related to, create an issue on that repository and provide the following information:

* **Use a clear and descriptive title** for the issue to identify the suggestion.
* **Provide a step-by-step description of the suggested enhancement** in as many details as possible.
* **Provide specific examples to demonstrate the steps**. Include copy/pasteable snippets which you use in those examples, as [Markdown code blocks](https://help.github.com/articles/markdown-basics/#multiple-lines).
* **Describe the current behavior** and **explain which behavior you expected to see instead** and why.
* **Include screenshots and animated GIFs** which help you demonstrate the steps or point out the part of CentipedeRoyale which the suggestion is related to. You can use [this tool](https://www.cockos.com/licecap/) to record GIFs on macOS and Windows, and [this tool](https://github.com/colinkeenan/silentcast) or [this tool](https://github.com/GNOME/byzanz) on Linux.
* **Explain why this enhancement would be useful** to most AtCentipedeRoyaleom users and isn't something that can or should be implemented as a [community package](#centipede-royale).
* **List some other text editors or applications where this enhancement exists.**
* **Specify which version of CentipedeRoyale you're using.** You can get the exact version by running `centipede-royale -v` in your terminal, or by starting CentipedeRoyale and running the `Application: About` command from the [Command Palette](https://github.com/centipede-request/command-palette).
* **Specify the name and version of the OS you're using.**

### Your First Code Contribution

Unsure where to begin contributing to CentipedeRoyale? You can start by looking through these `beginner` and `help-wanted` issues:

* [Beginner issues][beginner] - issues which should only require a few lines of code, and a test or two.
* [Help wanted issues][help-wanted] - issues which should be a bit more involved than `beginner` issues.

Both issue lists are sorted by total number of comments. While not perfect, number of comments is a reasonable proxy for impact a given change will have.

If you want to read about using CentipedeRoyale or developing packages in CentipedeRoyale, the [Centipede Royale Manual](https://centipede-royale.github.io/CentipedeRoyale/) is free and available online. You can find the source to the manual in [centipede-royale](https://centipede-royale.github.io/CentipedeRoyale/).

#### Local development

CentipedeRoyale Core and all packages can be developed locally. For instructions on how to do this, see the following sections in the [Centipede Royale Manual](https://centipede-royale.github.io/CentipedeRoyale/:

* [Hacking on CentipedeRoyale Core][hacking-on-centipede-royale-core]
* [Contributing to Official CentipedeRoyale Packages][contributing-to-official-centipede-royale-packages]

### Pull Requests

The process described here has several goals:

- Maintain CentipedeRoyale's quality
- Fix problems that are important to users
- Engage the community in working toward the best possible CentipedeRoyale
- Enable a sustainable system for CentipedeRoyale's maintainers to review contributions

Please follow these steps to have your contribution considered by the maintainers:

1. Follow all instructions in [the template](PULL_REQUEST_TEMPLATE.md)
2. Follow the [styleguides](#styleguides)
3. After you submit your pull request, verify that all [status checks](https://help.github.com/articles/about-status-checks/) are passing <details><summary>What if the status checks are failing?</summary>If a status check is failing, and you believe that the failure is unrelated to your change, please leave a comment on the pull request explaining why you believe the failure is unrelated. A maintainer will re-run the status check for you. If we conclude that the failure was a false positive, then we will open an issue to track that problem with our status check suite.</details>

While the prerequisites above must be satisfied prior to having your pull request reviewed, the reviewer(s) may ask you to complete additional design work, tests, or other changes before your pull request can be ultimately accepted.

## Styleguides

### Git Commit Messages

* Use the present tense ("Add feature" not "Added feature")
* Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
* Limit the first line to 72 characters or less
* Reference issues and pull requests liberally after the first line
* When only changing documentation, include `[ci skip]` in the commit title
* Consider starting the commit message with an applicable emoji:
    * :art: `:art:` when improving the format/structure of the code
    * :racehorse: `:racehorse:` when improving performance
    * :non-potable_water: `:non-potable_water:` when plugging memory leaks
    * :memo: `:memo:` when writing docs
    * :penguin: `:penguin:` when fixing something on Linux
    * :apple: `:apple:` when fixing something on macOS
    * :checkered_flag: `:checkered_flag:` when fixing something on Windows
    * :bug: `:bug:` when fixing a bug
    * :fire: `:fire:` when removing code or files
    * :green_heart: `:green_heart:` when fixing the CI build
    * :white_check_mark: `:white_check_mark:` when adding tests
    * :lock: `:lock:` when dealing with security
    * :arrow_up: `:arrow_up:` when upgrading dependencies
    * :arrow_down: `:arrow_down:` when downgrading dependencies
    * :shirt: `:shirt:` when removing linter warnings

### JavaScript Styleguide

All JavaScript must adhere to [JavaScript Standard Style](https://standardjs.com/).

* Prefer the object spread operator (`{...anotherObj}`) to `Object.assign()`
* Inline `export`s with expressions whenever possible
  ```js
  // Use this:
  export default class ClassName {

  }

  // Instead of:
  class ClassName {

  }
  export default ClassName
  ```
* Place requires in the following order:
    * Built in Node Modules (such as `path`)
    * Built in CentipedeRoyale and CentipedeRoyale Modules (such as `centipede-royale`, `remote`)
    * Local Modules (using relative paths)
* Place class properties in the following order:
    * Class methods and properties (methods starting with `static`)
    * Instance methods and properties
* [Avoid platform-dependent code](https://centipede-royale.github.io/CentipedeRoyale/sections/cross-platform-compatibility/)

### CoffeeScript Styleguide

* Set parameter defaults without spaces around the equal sign
    * `clear = (count=1) ->` instead of `clear = (count = 1) ->`
* Use spaces around operators
    * `count + 1` instead of `count+1`
* Use spaces after commas (unless separated by newlines)
* Use parentheses if it improves code clarity.
* Prefer alphabetic keywords to symbolic keywords:
    * `a is b` instead of `a == b`
* Avoid spaces inside the curly-braces of hash literals:
    * `{a: 1, b: 2}` instead of `{ a: 1, b: 2 }`
* Include a single line of whitespace between methods.
* Capitalize initialisms and acronyms in names, except for the first word, which
  should be lower-case:
  * `getURI` instead of `getUri`
  * `uriToOpen` instead of `URIToOpen`
* Use `slice()` to copy an array
* Add an explicit `return` when your function ends with a `for`/`while` loop and
  you don't want it to return a collected array.
* Use `this` instead of a standalone `@`
  * `return this` instead of `return @`
* Place requires in the following order:
    * Built in Node Modules (such as `path`)
    * Built in CentipedeRoyale and Electron Modules (such as `centipede-royale`, `remote`)
    * Local Modules (using relative paths)
* Place class properties in the following order:
    * Class methods and properties (methods starting with a `@`)
    * Instance methods and properties
* [Avoid platform-dependent code](https://centipede-royale.github.io/CentipedeRoyale/sections/cross-platform-compatibility/)

### Specs Styleguide

- Include thoughtfully-worded, well-structured [Jasmine](https://jasmine.github.io/) specs in the `./spec` folder.
- Treat `describe` as a noun or situation.
- Treat `it` as a statement about state or how an operation changes state.

#### Example

```coffee
describe 'a dog', ->
 it 'barks', ->
 # spec here
 describe 'when the dog is happy', ->
  it 'wags its tail', ->
  # spec here
```

### Documentation Styleguide

* Use [CentipedeRoyaleDoc](https://github.com/centipede-royale/centipede-royaledoc).
* Use [Markdown](https://daringfireball.net/projects/markdown).
* Reference methods and classes in markdown with the custom `{}` notation:
    * Reference classes with `{ClassName}`
    * Reference instance methods with `{ClassName::methodName}`
    * Reference class methods with `{ClassName.methodName}`

#### Example

```coffee
# Public: Disable the package with the given name.
#
# * `name`    The {String} name of the package to disable.
# * `options` (optional) The {Object} with disable options (default: {}):
#   * `trackTime`     A {Boolean}, `true` to track the amount of time taken.
#   * `ignoreErrors`  A {Boolean}, `true` to catch and ignore errors thrown.
# * `callback` The {Function} to call after the package has been disabled.
#
# Returns `undefined`.
disablePackage: (name, options, callback) ->
```

## Additional Notes

### Issue and Pull Request Labels

This section lists the labels we use to help us track and manage issues and pull requests. Most labels are used across all CentipedeRoyale repositories, but some are specific to `centipede-royale/centipede-royale`.

[GitHub search](https://help.github.com/articles/searching-issues/) makes it easy to use labels for finding groups of issues or pull requests you're interested in. For example, you might be interested in [open issues across `centipede-royale/centipede-royale` and all CentipedeRoyale-owned packages which are labeled as bugs, but still need to be reliably reproduced]() or perhaps [open pull requests in `centipede-royale/centipede-royale` which haven't been reviewed yet](https://github.com/search?utf8=%E2%9C%93&q=is%3Aopen+is%3Apr+repo%3Acentipederoyale%2Fcentipederoyale+comments%3A0). To help you find issues and pull requests, each label is listed with search links for finding open items with that label in `centipede-royale/centipede-royale` only and also across all CentipedeRoyale repositories. We  encourage you to read about [other search filters](https://help.github.com/articles/searching-issues/) which will help you write more focused queries.

The labels are loosely grouped by their purpose, but it's not required that every issue have a label from every group or that an issue can't have more than one label from the same group.

Please open an issue on `centipede-royale/centipede-royale` if you have suggestions for new labels, and if you notice some labels are missing on some repositories, then please open an issue on that repository.

#### Type of Issue and Issue State

| Label name | `centipede-royale/centipede-royale` :mag_right: | `centipede-royale`‑org :mag_right: | Description |
| --- | --- | --- | --- |
| `enhancement` | [search][search-centipede-royale-repo-label-enhancement] | [search][search-centipede-royale-org-label-enhancement] | Feature requests. |
| `bug` | [search][search-centipede-royale-repo-label-bug] | [search][search-centipede-royale-org-label-bug] | Confirmed bugs or reports that are very likely to be bugs. |
| `question` | [search][search-centipede-royale-repo-label-question] | [search][search-centipede-royale-org-label-question] | Questions more than bug reports or feature requests (e.g. how do I do X). |
| `feedback` | [search][search-centipede-royale-repo-label-feedback] | [search][search-centipede-royale-org-label-feedback] | General feedback more than bug reports or feature requests. |
| `help-wanted` | [search][search-centipede-royale-repo-label-help-wanted] | [search][search-centipede-royale-org-label-help-wanted] | The CentipedeRoyale core team would appreciate help from the community in resolving these issues. |
| `beginner` | [search][search-centipede-royale-repo-label-beginner] | [search][search-centipede-royale-org-label-beginner] | Less complex issues which would be good first issues to work on for users who want to contribute to CentipedeRoyale. |
| `more-information-needed` | [search][search-centipede-royale-repo-label-more-information-needed] | [search][search-centipede-royale-org-label-more-information-needed] | More information needs to be collected about these problems or feature requests (e.g. steps to reproduce). |
| `needs-reproduction` | [search][search-centipede-royale-repo-label-needs-reproduction] | [search][search-centipede-royale-org-label-needs-reproduction] | Likely bugs, but haven't been reliably reproduced. |
| `blocked` | [search][search-centipede-royale-repo-label-blocked] | [search][search-centipede-royale-org-label-blocked] | Issues blocked on other issues. |
| `duplicate` | [search][search-centipede-royale-repo-label-duplicate] | [search][search-centipede-royale-org-label-duplicate] | Issues which are duplicates of other issues, i.e. they have been reported before. |
| `wontfix` | [search][search-centipede-royale-repo-label-wontfix] | [search][search-centipede-royale-org-label-wontfix] | The CentipedeRoyale core team has decided not to fix these issues for now, either because they're working as intended or for some other reason. |
| `invalid` | [search][search-centipede-royale-repo-label-invalid] | [search][search-centipede-royale-org-label-invalid] | Issues which aren't valid (e.g. user errors). |
| `package-idea` | [search][search-centipede-royale-repo-label-package-idea] | [search][search-centipede-royale-org-label-package-idea] | Feature request which might be good candidates for new packages, instead of extending CentipedeRoyale or core CentipedeRoyale packages. |
| `wrong-repo` | [search][search-centipede-royale-repo-label-wrong-repo] | [search][search-centipede-royale-org-label-wrong-repo] | Issues reported on the wrong repository (e.g. a bug related to the [Settings View package](https://centipede-royale.github.io/CentipedeRoyale/) was reported on [CentipedeRoyale core](https://github.com/centipede-royale/centipede-royale)). |

#### Topic Categories

| Label name | `centipede-royale/centipede-royale` :mag_right: | `centipede-royale`‑org :mag_right: | Description |
| --- | --- | --- | --- |
| `windows` | [search][search-centipede-royale-repo-label-windows] | [search][search-centipede-royale-org-label-windows] | Related to CentipedeRoyale running on Windows. |
| `linux` | [search][search-centipede-royale-repo-label-linux] | [search][search-centipede-royale-org-label-linux] | Related to CentipedeRoyale running on Linux. |
| `mac` | [search][search-centipede-royale-repo-label-mac] | [search][search-centipede-royale-org-label-mac] | Related to CentipedeRoyale running on macOS. |
| `documentation` | [search][search-centipede-royale-repo-label-documentation] | [search][search-centipede-royale-org-label-documentation] | Related to any type of documentation (e.g. [API documentation](https://github.com/centipede-royale/CentipedeRoyale/) and the [manual](https://github.com/centipede-royale/CentipedeRoyale/)). |
| `performance` | [search][search-centipede-royale-repo-label-performance] | [search][search-centipede-royale-org-label-performance] | Related to performance. |
| `security` | [search][search-centipede-royale-repo-label-security] | [search][search-centipede-royale-org-label-security] | Related to security. |
| `ui` | [search][search-centipede-royale-repo-label-ui] | [search][search-centipede-royale-org-label-ui] | Related to visual design. |
| `api` | [search][search-centipede-royale-repo-label-api] | [search][search-centipede-royale-org-label-api] | Related to CentipedeRoyale's public APIs. |
| `uncaught-exception` | [search][search-centipede-royale-repo-label-uncaught-exception] | [search][search-centipede-royale-org-label-uncaught-exception] | Issues about uncaught exceptions, normally created from the [Notifications package](https://github.com/centipede-royale/CentipedeRoyale). |
| `crash` | [search][search-centipede-royale-repo-label-crash] | [search][search-centipede-royale-org-label-crash] | Reports of CentipedeRoyale completely crashing. |
| `auto-indent` | [search][search-centipede-royale-repo-label-auto-indent] | [search][search-centipede-royale-org-label-auto-indent] | Related to auto-indenting text. |
| `encoding` | [search][search-centipede-royale-repo-label-encoding] | [search][search-centipede-royale-org-label-encoding] | Related to character encoding. |
| `network` | [search][search-centipede-royale-repo-label-network] | [search][search-centipede-royale-org-label-network] | Related to network problems or working with remote files (e.g. on network drives). |
| `git` | [search][search-centipede-royale-repo-label-git] | [search][search-centipede-royale-org-label-git] | Related to Git functionality (e.g. problems with gitignore files or with showing the correct file status). |

#### `centipede-royale/centipede-royale` Topic Categories

| Label name | `centipede-royale/centipede-royale` :mag_right: | `centipede-royale`‑org :mag_right: | Description |
| --- | --- | --- | --- |
| `editor-rendering` | [search][search-centipede-royale-repo-label-editor-rendering] | [search][search-centipede-royale-org-label-editor-rendering] | Related to language-independent aspects of rendering text (e.g. scrolling, soft wrap, and font rendering). |
| `build-error` | [search][search-centipede-royale-repo-label-build-error] | [search][search-centipede-royale-org-label-build-error] | Related to problems with building CentipedeRoyale from source. |
| `error-from-pathwatcher` | [search][search-centipede-royale-repo-label-error-from-pathwatcher] | [search][search-centipede-royale-org-label-error-from-pathwatcher] | Related to errors thrown by the [pathwatcher library](https://github.com/centipede-royale/CentipedeRoyale). |
| `error-from-save` | [search][search-centipede-royale-repo-label-error-from-save] | [search][search-centipede-royale-org-label-error-from-save] | Related to errors thrown when saving files. |
| `error-from-open` | [search][search-centipede-royale-repo-label-error-from-open] | [search][search-centipede-royale-org-label-error-from-open] | Related to errors thrown when opening files. |
| `installer` | [search][search-centipede-royale-repo-label-installer] | [search][search-centipede-royale-org-label-installer] | Related to the CentipedeRoyale installers for different OSes. |
| `auto-updater` | [search][search-centipede-royale-repo-label-auto-updater] | [search][search-centipede-royale-org-label-auto-updater] | Related to the auto-updater for different OSes. |
| `deprecation-help` | [search][search-centipede-royale-repo-label-deprecation-help] | [search][search-centipede-royale-org-label-deprecation-help] | Issues for helping package authors remove usage of deprecated APIs in packages. |
| `centipede-royale` | [search][search-centipede-royale-repo-label-electron] | [search][search-centipede-royale-org-label-electron] | Issues that require changes to [CentipedeRoyale](https://centipede-royale.github.io/CentipedeRoyale/) to fix or implement. |

#### Pull Request Labels

| Label name | `centipede-royale/centipede-royale` :mag_right: | `centipede-royale`‑org :mag_right: | Description
| --- | --- | --- | --- |
| `work-in-progress` | [search][search-centipede-royale-repo-label-work-in-progress] | [search][search-centipede-royale-org-label-work-in-progress] | Pull requests which are still being worked on, more changes will follow. |
| `needs-review` | [search][search-centipede-royale-repo-label-needs-review] | [search][search-centipede-royale-org-label-needs-review] | Pull requests which need code review, and approval from maintainers or CentipedeRoyale core team. |
| `under-review` | [search][search-centipede-royale-repo-label-under-review] | [search][search-centipede-royale-org-label-under-review] | Pull requests being reviewed by maintainers or CentipedeRoyale core team. |
| `requires-changes` | [search][search-centipede-royale-repo-label-requires-changes] | [search][search-centipede-royale-org-label-requires-changes] | Pull requests which need to be updated based on review comments and then reviewed again. |
| `needs-testing` | [search][search-centipede-royale-repo-label-needs-testing] | [search][search-centipede-royale-org-label-needs-testing] | Pull requests which need manual testing. |

[search-centipede-royale-repo-label-enhancement]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aenhancement
[search-centipede-royale-org-label-enhancement]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aenhancement
[search-centipede-royale-repo-label-bug]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Abug
[search-centipede-royale-org-label-bug]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Abug
[search-centipede-royale-repo-label-question]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aquestion
[search-centipede-royale-org-label-question]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aquestion
[search-centipede-royale-repo-label-feedback]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Afeedback
[search-centipede-royale-org-label-feedback]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Afeedback
[search-centipede-royale-repo-label-help-wanted]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Ahelp-wanted
[search-centipede-royale-org-label-help-wanted]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Ahelp-wanted
[search-centipede-royale-repo-label-beginner]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Abeginner
[search-centipede-royale-org-label-beginner]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Abeginner
[search-centipede-royale-repo-label-more-information-needed]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Amore-information-needed
[search-centipede-royale-org-label-more-information-needed]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Amore-information-needed
[search-centipede-royale-repo-label-needs-reproduction]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aneeds-reproduction
[search-centipede-royale-org-label-needs-reproduction]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aneeds-reproduction
[search-centipede-royale-repo-label-triage-help-needed]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Atriage-help-needed
[search-centipede-royale-org-label-triage-help-needed]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Atriage-help-needed
[search-centipede-royale-repo-label-windows]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Awindows
[search-centipede-royale-org-label-windows]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Awindows
[search-centipede-royale-repo-label-linux]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Alinux
[search-centipede-royale-org-label-linux]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Alinux
[search-centipede-royale-repo-label-mac]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Amac
[search-centipede-royale-org-label-mac]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Amac
[search-centipede-royale-repo-label-documentation]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Adocumentation
[search-centipede-royale-org-label-documentation]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Adocumentation
[search-centipede-royale-repo-label-performance]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aperformance
[search-centipede-royale-org-label-performance]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aperformance
[search-centipede-royale-repo-label-security]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Asecurity
[search-centipede-royale-org-label-security]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Asecurity
[search-centipede-royale-repo-label-ui]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aui
[search-centipede-royale-org-label-ui]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aui
[search-centipede-royale-repo-label-api]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aapi
[search-centipede-royale-org-label-api]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aapi
[search-centipede-royale-repo-label-crash]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Acrash
[search-centipede-royale-org-label-crash]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Acrash
[search-centipede-royale-repo-label-auto-indent]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aauto-indent
[search-centipede-royale-org-label-auto-indent]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aauto-indent
[search-centipede-royale-repo-label-encoding]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aencoding
[search-centipede-royale-org-label-encoding]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aencoding
[search-centipede-royale-repo-label-network]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Anetwork
[search-centipede-royale-org-label-network]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Anetwork
[search-centipede-royale-repo-label-uncaught-exception]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Auncaught-exception
[search-centipede-royale-org-label-uncaught-exception]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Auncaught-exception
[search-centipede-royale-repo-label-git]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Agit
[search-centipede-royale-org-label-git]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Agit
[search-centipede-royale-repo-label-blocked]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Ablocked
[search-centipede-royale-org-label-blocked]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Ablocked
[search-centipede-royale-repo-label-duplicate]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aduplicate
[search-centipede-royale-org-label-duplicate]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aduplicate
[search-centipede-royale-repo-label-wontfix]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Awontfix
[search-centipede-royale-org-label-wontfix]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Awontfix
[search-centipede-royale-repo-label-invalid]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Ainvalid
[search-centipede-royale-org-label-invalid]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Ainvalid
[search-centipede-royale-repo-label-package-idea]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Apackage-idea
[search-centipede-royale-org-label-package-idea]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Apackage-idea
[search-centipede-royale-repo-label-wrong-repo]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Awrong-repo
[search-centipede-royale-org-label-wrong-repo]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Awrong-repo
[search-centipede-royale-repo-label-editor-rendering]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aeditor-rendering
[search-centipede-royale-org-label-editor-rendering]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aeditor-rendering
[search-centipede-royale-repo-label-build-error]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Abuild-error
[search-centipede-royale-org-label-build-error]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Abuild-error
[search-centipede-royale-repo-label-error-from-pathwatcher]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aerror-from-pathwatcher
[search-centipede-royale-org-label-error-from-pathwatcher]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aerror-from-pathwatcher
[search-centipede-royale-repo-label-error-from-save]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aerror-from-save
[search-centipede-royale-org-label-error-from-save]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aerror-from-save
[search-centipede-royale-repo-label-error-from-open]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aerror-from-open
[search-centipede-royale-org-label-error-from-open]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aerror-from-open
[search-centipede-royale-repo-label-installer]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Ainstaller
[search-centipede-royale-org-label-installer]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Ainstaller
[search-centipede-royale-repo-label-auto-updater]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aauto-updater
[search-centipede-royale-org-label-auto-updater]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aauto-updater
[search-centipede-royale-repo-label-deprecation-help]: https://github.com/search?q=is%3Aopen+is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+label%3Adeprecation-help
[search-centipede-royale-org-label-deprecation-help]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Adeprecation-help
[search-centipede-royale-repo-label-electron]: https://github.com/search?q=is%3Aissue+repo%3Acentipederoyale%2Fcentipederoyale+is%3Aopen+label%3Aelectron
[search-centipede-royale-org-label-electron]: https://github.com/search?q=is%3Aopen+is%3Aissue+user%3Acentipederoyale+label%3Aelectron
[search-centipede-royale-repo-label-work-in-progress]: https://github.com/search?q=is%3Aopen+is%3Apr+repo%3Acentipederoyale%2Fcentipederoyale+label%3Awork-in-progress
[search-centipede-royale-org-label-work-in-progress]: https://github.com/search?q=is%3Aopen+is%3Apr+user%3Acentipederoyale+label%3Awork-in-progress
[search-centipede-royale-repo-label-needs-review]: https://github.com/search?q=is%3Aopen+is%3Apr+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aneeds-review
[search-centipede-royale-org-label-needs-review]: https://github.com/search?q=is%3Aopen+is%3Apr+user%3Acentipederoyale+label%3Aneeds-review
[search-centipede-royale-repo-label-under-review]: https://github.com/search?q=is%3Aopen+is%3Apr+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aunder-review
[search-centipede-royale-org-label-under-review]: https://github.com/search?q=is%3Aopen+is%3Apr+user%3Acentipederoyale+label%3Aunder-review
[search-centipede-royale-repo-label-requires-changes]: https://github.com/search?q=is%3Aopen+is%3Apr+repo%3Acentipederoyale%2Fcentipederoyale+label%3Arequires-changes
[search-centipede-royale-org-label-requires-changes]: https://github.com/search?q=is%3Aopen+is%3Apr+user%3Acentipederoyale+label%3Arequires-changes
[search-centipede-royale-repo-label-needs-testing]: https://github.com/search?q=is%3Aopen+is%3Apr+repo%3Acentipederoyale%2Fcentipederoyale+label%3Aneeds-testing
[search-centipede-royale-org-label-needs-testing]: https://github.com/search?q=is%3Aopen+is%3Apr+user%3Acentipederoyale+label%3Aneeds-testing

[beginner]:https://github.com/search?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+label%3Abeginner+label%3Ahelp-wanted+user%3Acentipederoyale+sort%3Acomments-desc
[help-wanted]:https://github.com/search?q=is%3Aopen+is%3Aissue+label%3Ahelp-wanted+user%3Acentipederoyale+sort%3Acomments-desc+-label%3Abeginner
[contributing-to-official-centipede-royale-packages]:https://centipede-royale.github.io/CentipedeRoyale/sections/contributing-to-official-centipede-royale-packages/
[hacking-on-centipede-royale-core]: https://centipede-royale.github.io/CentipedeRoyale/sections/hacking-on-centipede-royale-core/