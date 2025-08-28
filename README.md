#  UEFI NVRAM Boot Entry Editor  UEFI-TUI  UEFI-TUI  UEFI-TUI

<p align="center">
  <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Desktop%20Computer.png" alt="Desktop Computer" width="120" height="120" />
</p>

<h1 align="center">UEFI NVRAM Boot Entry Editor</h1>

<p align="center">
  A user-friendly, terminal-based UI (TUI) for managing UEFI boot entries with <code>efibootmgr</code>.
</p>

<p align="center">
    <!-- License -->
    <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">
        <img src="https://img.shields.io/badge/License-GPLv3-blue.svg" alt="License: GPLv3">
    </a>
    <!-- Language -->
    <img src="https://img.shields.io/badge/Language-Bash-blueviolet" alt="Language: Bash">
    <!-- PRs Welcome -->
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome">
    <!-- OS -->
    <img src="https://img.shields.io/badge/OS-Linux%20(UEFI)-yellow.svg" alt="OS: Linux (UEFI)">
    <!-- Distros -->
    <img src="https://img.shields.io/badge/Distros-Debian%20%7C%20Ubuntu%20%7C%20Mint-orange" alt="Distros">
</p>

<p align="center">
    <!-- GitHub Repo specific badges - will work once repo is public -->
    <a href="https://github.com/LINUX-OASIS/custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR/issues">
        <img src="https://img.shields.io/github/issues/LINUX-OASIS/custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR" alt="GitHub issues">
    </a>
    <a href="https://github.com/LINUX-OASIS/custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR/stargazers">
        <img src="https://img.shields.io/github/stars/LINUX-OASIS/custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR" alt="GitHub stars">
    </a>
    <a href="https://github.com/LINUX-OASIS/custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR/network/members">
        <img src="https://img.shields.io/github/forks/LINUX-OASIS/custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR" alt="GitHub forks">
    </a>
</p>

---

## ✨ Features

This script simplifies the often-complex task of managing UEFI boot entries by providing a guided, interactive `whiptail` interface.

-   **Create Boot Entries**: Interactively scan for partitions (`vfat`, `iso9660`) and `.efi` files to create new, custom boot entries.
## 🖥️ Compatibility

This script is designed for **Linux distributions running on UEFI-based systems**. It uses the `apt` package manager for dependency installation.

**Officially Compatible With:**
*   Debian
*   Ubuntu
*   Linux Mint
*   ...and other Debian/Ubuntu derivatives.

## ⚙️ Dependencies

The script requires the following tools to be installed:

-   `efibootmgr`: The core command-line tool for managing UEFI boot entries.
-   `whiptail` (from the `newt` library): Used to create the dialog boxes for the TUI.

> **Note:** The script will automatically check if `efibootmgr` is installed and will attempt to install it using `sudo apt install -y efibootmgr` if it is not found.

## 🚀 Usage

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/LINUX-OASIS/custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR.git
    cd custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR
    ```

2.  **Make the script executable:**
    ```bash
    chmod +x custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR.sh
    ```

3.  **Run the script with `sudo`:**
    `efibootmgr` requires root privileges to modify NVRAM variables. The script will prompt you to re-run with `sudo` if you forget.
    ```bash
    sudo ./custom-EFIBOOTMGR-NVRAM-ENTRY-EDITOR.sh
    ```

4.  Follow the on-screen menus to manage your boot entries!

---

## 📜 License

This project is licensed under the **GNU General Public License v3.0**. See the LICENSE file for details.

## 💬 Contributing

Pull requests, issues, and suggestions are warmly welcomed! For major changes, please open an issue first to discuss what you would like to change.

See CONTRIBUTING.md for guidelines.

## 🌐 Links

*   Issues
*   Pull Requests
*   Releases
*   Wiki

## 🧙‍♂️ Maintainer

This project is maintained by **LINUX-OASIS**.

