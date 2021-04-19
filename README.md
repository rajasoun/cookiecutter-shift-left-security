# Getting Started

For institutionalizing Shift Left Security tools for

1. Secrets Detection
2. Static Application Security Testing (SAST) Scan

### Prerequisites

1. [Docker](https://www.docker.com/)

```sh
docker run --rm --name cruft python:3.9.3-alpine3.13  \
  pip3  install cruft \
  && cruft create https://github.com/rajasoun/cookiecutter-shift-left-security
```

Once finished, navigate to your new project folder :

```sh
cd <project_name>
```

Refer [SLS - Shift Left Security](SLS.md)



# Tool Radar
🚀 Collection of tools that performs git hooks management for linting, code formating, commit message standardization, sutomated versioning and package publishing

### Adopt:
-   [commitizen](https://github.com/commitizen/cz-cli): Tool that guides the developer through the writing of the commit message
-   [commitlint](https://github.com/conventional-changelog/commitlint): Tool that validates the commit message following a set of rules and good practices
-   [pre-commit](https://pre-commit.com/): A framework for managing and maintaining multi-language pre-commit hooks

### Assess:
-   [lint-staged](https://github.com/okonet/lint-staged): Run linters against staged git files and don't let :poop: slip into your code base!
-   [prettier](https://prettier.io/): An opinionated code formatter
-   [husky](https://github.com/typicode/husky): Tool that adds scripts (hooks) trigged before (pre-commit) and after (post-commit) your commit.
-   [release-it](https://github.com/release-it/release-it): CLI tool to automate versioning and package publishing related tasks
