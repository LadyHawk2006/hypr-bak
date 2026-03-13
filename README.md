# 🐧 Hyprland Config Backup

<div align="center">
  <img src="https://commons.wikimedia.org/wiki/File:Hyprland_Logo_Icon.svg" width="150" height="150" alt="Hyprland Logo">
  <br>
  <img src="https://img.shields.io/badge/Distro-CachyOS-orange?style=for-the-badge&logo=arch-linux" alt="Distro">
  <img src="https://img.shields.io/badge/WM-Hyprland-blue?style=for-the-badge&logo=hyprland" alt="Window Manager">
  <img src="https://img.shields.io/badge/Automation-Inotify--Tools-green?style=for-the-badge" alt="Automation">
</div>

---

## 🚀 Overview
This repository contains my personal **Hyprland** configuration files. It is powered by a custom **automated backup system** that syncs changes to GitHub in real-time.

### ✨ Key Features
* **Auto-Sync:** Powered by `inotify-tools` and `systemd`.
* **Real-time Backups:** Every file modification, creation, or deletion is tracked.
* **Version History:** Entire "rice" history is preserved via Git commits.

## 🛠️ Automated Backup Workflow
The system is managed by a background service that watches the `~/.config/hypr` directory.



1. **Modify:** Edit any config file (e.g., `hyprland.conf`).
2. **Detect:** `inotifywait` catches the file system event.
3. **Wait:** A 60-second "cooldown" allows for multiple quick saves.
4. **Push:** Changes are automatically committed and pushed to this repo.

## 📂 Structure
| Directory/File | Description |
| :--- | :--- |
| `hyprland.conf` | Core Window Manager settings |
| `custom/` | User-specific overrides and tweaks |
| `scripts/` | Utility scripts for UI/UX |
| `hyprlock.conf` | Lockscreen configuration |

---

## 👤 Maintainer
**LadyHawk2006**
- GitHub: [@LadyHawk2006](https://github.com/LadyHawk2006)
- Email: [shadrackburuna@gmail.com](mailto:shadrackburuna@gmail.com)

---
<div align="center">
  <sub>Built with ❤️ on CachyOS</sub>
</div>
