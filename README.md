# Daemon Labs - Workshop Prerequisites

We try to keep prerequisites to a minimum, but please run through these items before attending any of our workshops to ensure a smooth start.

## 1. Docker Environment

Please ensure you have [Docker Desktop](https://docs.docker.com/get-started/get-docker/) installed and running.
This provides the Docker engine required for our exercises.

To confirm successful installation, run the following command in your terminal:

```shell
docker --version
```

### Windows Users: WSL2 Requirement

To leverage Docker's best performance on Windows, you must have [WSL2 (Windows Subsystem for Linux)](https://docs.microsoft.com/en-us/windows/wsl/install) installed and set as the default engine in Docker Desktop settings.

## 2. Git Client

For cloning and managing the workshop code repository, you will need the Git command-line tool installed.

1. **Install Git:** Please install the Git client for your operating system from the official source: [Git SCM Downloads](https://git-scm.com/downloads).

2. **Verify Installation:** Confirm it's installed by running:

```shell
git --version
```

We don't mind which method you use to interact with Git, but popular options include the terminal, [GitHub Desktop](https://desktop.github.com/download/), or directly within Visual Studio Code.

## 3. Code Editor

While you can use any editor, we highly recommend using [Visual Studio Code](https://code.visualstudio.com/) due to its excellent integration capabilities.

### Recommended Visual Studio Code Extensions

- **Docker:** Installs quickly and provides great command and container management directly within the editor: [Visual Studio Code Docker Extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker).

### Windows Users: WSL Extension

If you are running Windows and using WSL2 (as recommended above), we also recommend installing the [Remote - WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl) extension for a seamless development experience inside the Linux environment.

## 4. GitHub Account

If you don't already have one, please create an account and sign in here: [GitHub Signup](https://github.com/signup).
We will be cloning repositories from GitHub during the workshop.
