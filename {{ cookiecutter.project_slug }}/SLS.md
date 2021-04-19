# Getting Started

Institutionalizing Shift Left Security tools for

1. Secrets Detection
1. Static Application Security Testing (SAST) Scan

### Prerequisites

1. [Visual Studio Code](https://code.visualstudio.com/)
1. [Remote-Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) ext install ms-vscode-remote.remote-containers
1. [Docker](https://www.docker.com/)

### Quick Background

Visual Studo Code [Remote Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension allow us to use docker as a full-featured development environment.

Remote Containters allows us to isolate each project’s development environment with following advantages

1. Reproducibility: Each developer has exactly the same workspace
1. Isolation: Workspaces and their dependencies are isolated from each other
1. Security: Prevents malicious dependencies from installing malware or reading your files.

Each project has a .devcontainer folder.
The .devcontainer folder contains the Dockerfile and devcontainer.json configuration for the development environment.

![Remote Container](https://code.visualstudio.com/assets/docs/remote/containers/architecture-containers.png)

### Getting Started

1. Enable help and alias

   ```
   $ source dotfiles/.alias.sh
   $ ghelp
   ```

1. Setup commitzen, commitlint and ggshield toolset as git hooks

   ```
   $ gsetup
   ```

1. Populate .env file with GITHUB_TOKEN, GITGUARDIAN_API_KEY and GITGUARDIAN_API_URL
   ```
   cp .env.sample .env
   ```

## Prerequisites - Remote development in Containers

Running Visual Studio Code in a Docker container using the Remote - Containers extension.
Goto: https://code.visualstudio.com/docs/remote/containers-tutorial

[Developing inside a Container](https://code.visualstudio.com/docs/remote/containers)
