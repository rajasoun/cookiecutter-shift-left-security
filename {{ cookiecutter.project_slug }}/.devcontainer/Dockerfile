# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.163.1/containers/python-3/.devcontainer/base.Dockerfile

# [Choice] Python version: 3, 3.9, 3.8, 3.7, 3.6
ARG VARIANT="3"
FROM mcr.microsoft.com/vscode/devcontainers/python:0-${VARIANT} AS builder

# secerts management using chamber
FROM segment/chamber:2.9.1 as chamber-builder

FROM builder
# COPY files

COPY dotfiles /root/dotfiles
COPY --from=chamber-builder /chamber /usr/bin/chamber

# pip3 packages
RUN set -ex \
    && pip3 --disable-pip-version-check --no-cache-dir install pipenv ggshield pre-commit commitizen cruft

# OS packages.
RUN set -ex \
    && apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends git-flow bash-completion
