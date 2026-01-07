# Daemon Labs - Workshop Prerequisites

We try to keep prerequisites to a minimum, but please run through these items before attending the workshop to ensure a smooth start.

## 1. Create a GitHub Account
If you don't already have one, please [sign up for GitHub](https://github.com/signup). You will need this to access the workshop code.

---

## 2. System Setup (Select Your OS)

Please follow the instructions for your specific operating system below.

### 🍎 macOS Users
1.  **Install Command Line Tools (Git)**
    * Open your terminal (Command+Space, type "Terminal").
    * Run the command: `git --version`
    * **If a pop-up appears:** Click **"Install"**. This automatically sets up Git and necessary system tools.
        * *Note: The pop-up might open **behind** your terminal window. Move your window to check!*
    * **If you see a version number:** You are already set.

2.  **Install Container Engine (Docker)**
    * **Option A (Standard):** Download and install [Docker Desktop for Mac](https://docs.docker.com/desktop/install/mac-install/).
    * **Option B (License Friendly):** If you cannot use Docker Desktop due to licensing, install [Rancher Desktop](https://rancherdesktop.io/).
        * *Important:* During setup, ensure you select **"dockerd (moby)"** as the container engine.

### 🪟 Windows Users
**Important:** We require **WSL2** (Windows Subsystem for Linux) for this workshop to ensure everything runs correctly.

1.  **Install WSL2**
    * Open PowerShell as Administrator.
    * Run: `wsl --install`
    * Restart your computer if prompted. This will install the Ubuntu Linux environment.

2.  **Install Container Engine (Docker)**
    * **Option A (Standard):** Download [Docker Desktop for Windows](https://docs.docker.com/desktop/install/windows-install/).
        * In Settings > General, ensure **"Use the WSL 2 based engine"** is checked.
        * In Settings > Resources > WSL Integration, ensure "Ubuntu" is toggled **ON**.
    * **Option B (License Friendly):** Install [Rancher Desktop](https://rancherdesktop.io/).
        * *Important:* During setup, select **"dockerd (moby)"** as the engine and enable **WSL** access for your Ubuntu distribution.

3.  **Verify Git**
    * Open your **Ubuntu** terminal (search "Ubuntu" in the Start menu).
    * Run `git --version`. (Git is usually pre-installed on WSL. If missing, run `sudo apt update && sudo apt install git`).

### 🐧 Linux Users
1.  **Install Git:** Run `sudo apt install git` (or your distro equivalent).
2.  **Install Docker:** Follow the instructions for [Docker Engine](https://docs.docker.com/engine/install/).

---

## 3. Code Editor

We recommend **Visual Studio Code** for its strong Docker integration, but **Cursor** is a fully compatible alternative.

### Option A: Visual Studio Code (Recommended)
1.  **Download & Install:** [Visual Studio Code](https://code.visualstudio.com/).
2.  **Install Extensions:** Open VS Code, click the "Extensions" icon (square grid on the left), and install:
    * **Docker** (by Microsoft) - *For container management.*
    * **WSL** (by Microsoft) - *Required for Windows users to edit files inside Linux.*

### Option B: Cursor (AI-Powered)
If you prefer [Cursor](https://cursor.com/), it works perfectly for this workshop.
* **Note:** You must still install the **Docker** and **WSL** extensions mentioned above inside Cursor.

---

## 4. Final Verification (Run This!)

Before the workshop starts, please open your terminal (**Windows users: use your Ubuntu terminal**) and run these commands to confirm everything is ready.

You should see version numbers for both:

```bash
git --version
docker --version
