# Getting Started

For institutionalizing Shift Left Security tools for 
1. Secrets Detection
2. Static Application Security Testing (SAST) Scan

### Prerequisites
1. [Docker](https://www.docker.com/)

```sh
docker run --rm --name cruft python:3.9.2-alpine3.13  \
  pip3  install cruft \
  && cruft create https://github.com/rajasoun/cookiecutter-shift-left-security
```

Once finished, navigate to your new project folder :

```sh
cd <project_name>
```

Refer SLS.md

SLS - Shift Left Security

