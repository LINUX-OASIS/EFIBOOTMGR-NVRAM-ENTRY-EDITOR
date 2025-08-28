# 📦 AppImage Manager

<div align="center">

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](https://www.gnu.org/licenses/gpl-3.0)
[![Made with Bash](https://img.shields.io/badge/Made%20with-Bash-1f425f.svg?style=for-the-badge&logo=gnu-bash)](https://www.gnu.org/software/bash/)
[![Open Issues](https://img.shields.io/github/issues/LINUX-OASIS/appimage-manager?style=for-the-badge&logo=github)](https://github.com/LINUX-OASIS/appimage-manager/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/LINUX-OASIS/appimage-manager?style=for-the-badge&logo=github)](https://github.com/LINUX-OASIS/appimage-manager/pulls)
[![Forks](https://img.shields.io/github/forks/LINUX-OASIS/appimage-manager?style=for-the-badge&logo=github)](https://github.com/LINUX-OASIS/appimage-manager/network/members)
[![Stars](https://img.shields.io/github/stars/LINUX-OASIS/appimage-manager?style=for-the-badge&logo=github)](https://github.com/LINUX-OASIS/appimage-manager/stargazers)

</div>

A simple, yet powerful, command-line tool to download, integrate, update, and manage your [AppImages](https://appimage.org/).

This script automates the process of handling AppImages, integrating them into your system's application menu for a seamless desktop experience.

<br>

## 📚 Table of Contents
- [✨ Key Features](#-key-features)
- [🖥️ Compatibility](#️-compatibility)
- [⚙️ Dependencies](#️-dependencies)
- [🚀 Getting Started](#-getting-started)
  - [🔩 Installation](#-installation)
  - [💡 Usage](#-usage)
- [💬 Contributing](#-contributing)
- [📜 License](#-license)
- [🧙‍♂️ Maintainer](#️-maintainer)
- [🌐 Links](#-links)

## ✨ Key Features

- **Install:** Download the latest AppImage from a GitHub repository and integrate it.
- **Desktop Integration:** Automatically creates a `.desktop` file and extracts the icon.
- **Update:** Check for and install the latest version of an AppImage.
- **Manage:** List all installed AppImages or remove them cleanly.
- **Run:** Launch your AppImages directly from the terminal.
- **Dependency-Aware:** Checks for required tools and offers to install them for you.

---

## 🖥️ Compatibility

This script is designed for Linux distributions that use the `apt` package manager. It has been tested and is known to be compatible with:

- ✅ **Debian**
- ✅ **Ubuntu**
- ✅ **Linux Mint**
- ✅ **Other Debian/Ubuntu derivatives**

While it may work on other systems, automatic dependency installation is only supported on `apt`-based distros.

## ⚙️ Dependencies

The script requires the following command-line tools to function correctly:

- `curl`
- `jq`
- `fuse`

Don't worry if you don't have them! The script will check for missing dependencies and prompt you to install them automatically.

---

## 🚀 Getting Started

### 🔩 Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/LINUX-OASIS/appimage-manager.git
    cd appimage-manager
    ```

2.  **Make the script executable:**
    ```sh
    chmod +x appimage-manager
    ```

3.  **(Optional) Move to your PATH for global access:**
    ```sh
    sudo mv appimage-manager /usr/local/bin/appimage-manager
    ```

### 💡 Usage

The script is controlled by simple commands.

**1. Install an AppImage**

Provide the GitHub repository in `USER/REPO` format. The script will find the latest release and install the AppImage.

```sh
appimage-manager install AppImage/AppImageKit
```

**2. List Installed AppImages**

See all the applications you've installed with the manager.

```sh
appimage-manager list
```

**3. Update an AppImage**

Check for a new version and update if available. Use the application name from the `list` command.

```sh
appimage-manager update AppImageKit
```

**4. Run an AppImage**

Launch the application directly.

```sh
appimage-manager run AppImageKit
```

**5. Remove an AppImage**

Completely remove the AppImage, its desktop file, and its icon from your system.

```sh
appimage-manager remove AppImageKit
```

**6. Get Help**

Display the help message with all available commands.

```sh
appimage-manager help
```

---

## 💬 Contributing

Pull requests, issues, and suggestions are warmly welcomed! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 📜 License

This project is distributed under the **GNU General Public License v3.0**. See the `LICENSE` file for more information.

## 🧙‍♂️ Maintainer

- **LINUX-OASIS**

## 🌐 Links

- **Issues**
- **Pull Requests**
- **Releases**
- **Wiki**
