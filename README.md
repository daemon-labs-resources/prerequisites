# Daemon Labs - Workshop Prerequisites

We try to keep prerequisites to a minimum, but please run through these items before attending any of our workshops to ensure a smooth start.

---

## 1. GitHub Account

**Goal:** Ensure you have access to the workshop code repositories.

If you don't already have one, please [sign up for GitHub](https://github.com/signup).

> [!NOTE]
> We will be cloning repositories directly from GitHub during the workshop, so a valid account is required.

---

## 2. System Setup (Select Your OS)

**Goal:** Configure your operating system with the correct Container Engine and Git tools.

Please follow the instructions for your specific operating system below.

### 🍎 macOS Users

#### 1. Install Command Line Tools (Git)

Open your terminal (Command+Space, type "Terminal") and run the following command:

```bash
git --version
```

- **If a pop-up appears:** Click **"Install"**. This automatically sets up Git and necessary system tools.
- **If you see a version number:** You are already set.

> [!TIP]
> The installation pop-up might open **behind** your terminal window. Move your window to check if it's hiding there!

#### 2. Install Container Engine (Docker)

- **Option A (Standard):** Download and install [Docker Desktop for Mac](https://docs.docker.com/desktop/install/mac-install/).
- **Option B (License Friendly):** If you cannot use Docker Desktop due to licensing, install [Rancher Desktop](https://rancherdesktop.io/).

> [!IMPORTANT]
> If you choose **Rancher Desktop**, ensure you select **"dockerd (moby)"** as the container engine during setup.

---

### 🪟 Windows Users

> [!WARNING]
> We require **WSL2** (Windows Subsystem for Linux) for this workshop.  
> PowerShell alone will **not** work for the exercises.

#### 1. Install WSL2

Open PowerShell as Administrator and run:

```powershell
wsl --install
```

Restart your computer if prompted.  
This will install the Ubuntu Linux environment.

#### 2. Install Container Engine (Docker)

- **Option A (Standard):** Download [Docker Desktop for Windows](https://docs.docker.com/desktop/install/windows-install/).
  - In Settings > General, ensure **"Use the WSL 2 based engine"** is checked.
  - In Settings > Resources > WSL Integration, ensure "Ubuntu" is toggled **ON**.
- **Option B (License Friendly):** Install [Rancher Desktop](https://rancherdesktop.io/).
  - During setup, select **"dockerd (moby)"** as the engine.
  - Enable **WSL** access for your Ubuntu distribution in the settings.

#### 3. Verify Git

Open your **Ubuntu** terminal (search "Ubuntu" in the Start menu) and run:

```bash
git --version
```

> [!NOTE]
> Git is usually pre-installed on WSL. If it is missing, run `sudo apt update && sudo apt install git`.

---

### 🐧 Linux Users

#### 1. Install Git

Run the following command (or your distro equivalent):

```bash
sudo apt install git
```

#### 2. Install Docker

Follow the official instructions for [Docker Engine](https://docs.docker.com/engine/install/).

---

## 3. Code Editor

**Goal:** Set up an IDE that can communicate with Docker and your WSL environment.

We recommend **Visual Studio Code** for its strong Docker integration, but **Cursor** is a fully compatible alternative.

### Option A: Visual Studio Code (Recommended)

1.  **Download & Install:** [Visual Studio Code](https://code.visualstudio.com/).
2.  **Install Extensions:** Open VS Code, click the "Extensions" icon (square grid on the left), and install:
    - **Docker** (by Microsoft) - _For container management._
    - **WSL** (by Microsoft) - _Required for Windows users to edit files inside Linux._

### Option B: Cursor (AI-Powered)

If you prefer [Cursor](https://cursor.com/), it works perfectly for this workshop.

> [!IMPORTANT]
> You must still install the **Docker** and **WSL** extensions mentioned above inside Cursor.

---

## 4. Final Verification

**Goal:** Confirm all tools are installed and accessible from your terminal.

Before the workshop starts, please open your terminal (**Windows users: use your Ubuntu terminal**) and run these commands.

```bash
git --version
docker --version
```

You should see version numbers for both commands.

> [!WARNING]
> If `docker --version` fails, ensure your application (Docker Desktop or Rancher) is actually running!
>
> **Windows Users:** If it fails inside Ubuntu, check your "WSL Integration" settings in Docker/Rancher to ensure Ubuntu is authorized.

---

## 🎉 Ready to go!

Your environment is now prepared for the workshop. See you there!
