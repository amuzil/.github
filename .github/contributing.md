# Contributing to Amuzil projects

Thanks a ton for considering contributing to an Amuzil project!
We're always looking for new contributors, and we'd love to have you on board.

In this document, we'll go over the basics of contributing to an Amuzil project.
We'll cover the following topics:

- [Contributing to Amuzil projects](#contributing-to-amuzil-projects)
  - [Code of Conduct](#code-of-conduct)
  - [Kinds of Contributions](#kinds-of-contributions)
    - [How to Report a Bug](#how-to-report-a-bug)
    - [How to Suggest a Feature](#how-to-suggest-a-feature)
    - [How to Write Documentation](#how-to-write-documentation)
    - [How to Contribute Code](#how-to-contribute-code)
  - [Conventions](#conventions)
    - [Git](#git)
      - [Commits](#commits)
      - [Pull Requests](#pull-requests)
      - [Branches](#branches)
    - [Code](#code)
      - [Naming things](#naming-things)
      - [Formatting](#formatting)
  - [License](#license)

## Code of Conduct

We expect all contributors to abide by our [Code of Conduct](code-of-conduct.md).

## Kinds of Contributions

There are many ways to contribute to an Amuzil project.
Here are some of the most common ways:

- [Reporting a bug](#how-to-report-a-bug)
- [Suggesting a feature](#how-to-suggest-a-feature)
- [Writing documentation](#how-to-write-documentation)
- [Contributing code](#how-to-contribute-code)

### How to Report a Bug

> **IMPORTANT**: if you want to report a security vulnerability that could
> potentially affect the security of our users, please contact us following the
> instructions in the [Security Policy][security-url].

If you find a bug in an Amuzil project, please report it!
We use [GitHub Issues][issues-docs-url] to track bugs.
To report a bug, open a new issue in the project's repository.
If you're not sure how to do that, check out [this guide][creating-an-issue-docs-url].

When you open a new issue, please follow the issue template.

### How to Suggest a Feature

If you have an idea for a new feature, please suggest it!
We use [GitHub Issues][issues-docs-url] to track feature requests.
To suggest a feature, open a new issue in the project's repository.
If you're not sure how to do that, check out [this guide][creating-an-issue-docs-url].

When you open a new issue, please follow the issue template.

Are you unsure if your idea is a good fit for the project?
Feel free to [start a discussion][discussions-docs-url], and we'll talk it over!

### How to Write Documentation

All documentation for our projects lives in the [Amuzil Docs][amuzil-docs-url] repository.
We use [GitHub Pull Requests][pull-requests-docs-url] to track documentation contributions.
If you'd like to contribute to our documentation, please open a pull request there.

When you open a new pull request, please copy-paste the relevant
[pull request template][pull-request-templates-url].
In addition to the template, please follow our [conventions](#conventions).

### How to Contribute Code

If you'd like to contribute code to an Amuzil project, please open a pull request!
We use [GitHub Pull Requests][pull-requests-docs-url] to track code contributions.

When you open a new pull request, please copy-paste the relevant
[pull request template][pull-request-templates-url].
In addition to the template, please follow our [conventions](#conventions).

## Conventions

We have a few conventions that we follow when contributing to Amuzil projects.
These conventions help us keep our projects consistent and easy to work with.
We'll go over the conventions for each of the following topics:

- [Git](#git)
  - [Commits](#commits)
  - [Pull Requests](#pull-requests)
  - [Branches](#branches)
- [Code](#code)
  - [Naming things](#naming-things)
  - [Formatting](#formatting)

### Git

We use [Git][git-url] through [GitHub][github-url] to track changes to our projects.
We follow the [GitHub Flow][github-flow-url] when contributing to our projects.

#### Commits

Commits must be atomic, and should be as small as possible.
Commit messages should be clear and concise.
You must follow the following format:

```text
<gitmoji> <subject> [(#issue)]

<description>
```

Note in particular the spaces between the gitmoji, the subject and the issue,
and the blank line between the subject and the description.

If possible, [sign your commits][signing-commits-url].

##### Gitmoji

We use [Gitmoji][gitmoji-url] to add meaningful emojis to our commit messages.
This helps us keep our commit messages consistent and easy to read.
You should use the unicode emoji rather than the text version of the gitmoji.
So, `📝`, not `:memo:`.

> To make things easier,
> there are tools that integrate Gitmoji into your IDE of choice.
>
> For JetBrains IDEs, there is
> [Gitmoji Plus: Commit Button][jetbrains-gitmoji-url],
> and for Visual Studio Code, there is
> [Gitmoji][vscode-gitmoji-url].
> Both of these tools can be configured to use unicode emojis instead of text versions.
>
> If your IDE of choice does not have a Gitmoji plugin,
> or you prefer to use a Git client,
> you can use the [Gitmoji Cheat Sheet][gitmoji-url].

##### Subject

The subject of your commit message should be clear and concise.
It should be around 50 characters, and must no longer than 72 characters.
It must be written in the imperative mood, must start with a capital letter,
and must not end with a period.

Good examples:

```text
Add tomato sauce to pizza
Fix kitchen light
```

Bad examples:

```text
Added tomato sauce to pizza
fix kitchen light
```

##### Issue

If your commit is related to a specific commit, you should reference it within parentheses.
For example, for a commit that adresses issue 42, `(#123)`

##### Description

The description of your commit message can be as long as you need it to be.
It is free form, and can be used to explain the changes you made in more detail.
Be sure to use proper grammar and punctuation, and to keep your lines under 72 characters.
Also, try to use a semi-professional tone.

#### Pull Requests

Pull requests should be clear and concise. They should be as small as possible.
Pull request titles should be clear and concise.
They should start with a Gitmoji, then a space, then the title of the pull request.
The title must be written in the imperative mood, start with a capital letter,
must not end with a period, and must be no longer than 72 characters.
Aim for around 50 characters.

In general, a pull request title should look quite similar to a commit message.
However, it should summarise the changes made by all of the commits in the pull request.

##### Merge commits

Merge commits follow the same format, except for the fact that they reference the pull request, not the issue

```text
🔀 <summary> <#pull-request>

<description>
```

The `summary` should be equal to the pull request title, except if there is a good reason it should not be.

A good examples:

```text
🔀 Add form usage descriptions (#6)

Added VR & multikey usage descriptions for all forms,
as well as a small note to the Block description.
```

#### Branches

When contributing to an Amuzil project, you should create a new branch for your changes.
You must follow the following format:

```text
<type>/<name>
```

You should not use capital letters in your branch name.

Some good examples:

```text
feature/tomato-sauce-on-pizza
bug/kitchen-light
```

Some bad examples:

```text
JohnDoe/TomatoSauceOnPizza
michael/kitchen-light
tomato-sauce-on-pizza
```

##### Type

What the type of your branch is depends on the project and the changes you're making.
For example, some common types are:

- `feature`, for new features
- `bug`, for bug fixes
- `ci`, for changes to the CI/CD pipeline

Some projects may have more specific types, look for them in that project's `readme.md`.

##### Name

The name of your branch should be clear and concise.
It should be written in the imperative mood and kebab-case.

### Code

We use some quite opinionated code conventions. We'll go over them here.
These conventions help us keep our projects consistent and easy to work with.
Failure to follow these conventions may result in your pull request being rejected.

The best way to learn these conventions is to look at
the code in the project you're contributing to.
You'll learn them quick enough!

#### Naming things

When naming general folders or files, unless if otherwise specified
or impossible due to technical limitations, use kebab-case.

When naming packages/modules, code files, classes, functions, variables, etc.,
follow the conventions of the language you're using
as recommended by the [Naming Convention Project][naming-convention-project-url].

Additionally, follow the following conventions, taken from
[CodeAesthetics's "Naming Things in Code"][naming-things-in-code-url]:

- Don't abbreviate names
  - Wrong: `bpos`, `istack`
  - Correct: `blockPosition`, `itemStack`
- Don't put types in variable names
  - Wrong: `bIsValid`, `iCount`
  - Correct: `isValid`, `count`
- Add units to variable names unless if the type tells you
  - Wrong: `delay`, `length`
  - Correct: `delayMilliseconds`, `lengthMeters`
- Don't put types in your types
  - Wrong: `IDataTrait`, `IFlowControl`
  - Correct: `DataTrait`, `FlowControl`
- Refactor if you find yourself naming code `Utils`
  - Wrong: `InventoryUtils`
  - Correct: `InventoryWatcher`, `InventoryToJSONConverter`

Additionally, watching
[Povilas Korop's "One Rule to Name Methods/Variables Clearly"][one-rule-to-name-methods-variables-clearly-url]
is well worth your time. To summarise:

Bad:

```php
public function report($from, $to, $type);
```

Good:

```php
public function getFinancialReportData(
  string $fromDate,
  string $toDate,
  int $transactionType
): array;
```

It should be clear what the function does, what the parameters are, and what it returns.
Without having to read comments or the function's body.

> A comment is a failure to express yourself in code.
> If you fail, then write a comment;
> but try not to fail.
>
> ~ Uncle Bob Martin

#### Formatting

We use automated code formatting tools such as [Prettier][prettier-url]
to keep our code consistent and easy to read.
You must use these tools when contributing to an Amuzil project.

## License

By contributing to an Amuzil project, you agree that your contributions
will be licensed under its license, whatever it may be.
Look for a `license.md` at the root of the project's repository.

[security-url]: security.md
[issues-docs-url]: https://docs.github.com/en/issues/tracking-your-work-with-issues
[creating-an-issue-docs-url]: https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-issues/creating-an-issue
[pull-requests-docs-url]: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests
[pull-request-templates-url]: https://github.com/amuzil/.github/tree/main/.github/PULL_REQUEST_TEMPLATE
[discussions-docs-url]: https://docs.github.com/en/discussions
[amuzil-docs-url]: https://github.com/amuzil/docs
[git-url]: https://git-scm.com
[github-url]: https://github.com
[github-flow-url]: https://guides.github.com/introduction/flow
[signing-commits-url]: https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits
[gitmoji-url]: https://gitmoji.dev
[jetbrains-gitmoji-url]: https://plugins.jetbrains.com/plugin/12383-gitmoji-plus-commit-button
[vscode-gitmoji-url]: https://marketplace.visualstudio.com/items?itemName=seatonjiang.gitmoji-vscode
[naming-convention-project-url]: https://namingconvention.org
[naming-things-in-code-url]: https://www.youtube.com/watch?v=-J3wNP6u5YU
[one-rule-to-name-methods-variables-clearly-url]: https://www.youtube.com/watch?v=ptZKTMBR7Hw
[prettier-url]: https://prettier.io
