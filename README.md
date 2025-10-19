# 🛠️ Arch-Postinstall-Tool (v3.0) - The Adaptive Customizer

An intelligent, interactive post-installation script for Arch Linux, designed to streamline the setup of a high-performance system, focusing on Wayland (Hyprland), stability, and deep shell customization.

## Features at a Glance (v3.0)

* **Enhanced TUI:** A responsive, color-coded menu system for intuitive navigation.
* **Adaptive Hardware Patching:** Automatic detection of CPU (Intel/AMD) and common problematic hardware (e.g., Realtek Wi-Fi) to apply crucial post-install fixes (microcode, kernel parameters, TLP).
* **Zsh Deep Customization:** Interactive setup for **Oh My Zsh**, **Powerlevel10k**, and essential plugins.
* **Fastfetch Styling:** Choose from several display configurations, including custom color palettes.
* **Modular Installation:** Select GPU drivers, window managers (Hyprland, i3), and a comprehensive set of packages and dotfile themes via a guided menu flow.
* **Wayland Focus:** Pre-selected modern packages like **PipeWire** and **XDG Portals** for a seamless Wayland experience.

## Prerequisites

This script assumes you have already:

1.  Installed a **minimal Arch Linux base system**.
2.  Set up **network connectivity**.
3.  Created a **non-root user** with `sudo` privileges.
4.  Run the script from a **TTY** or an existing terminal session.

## Usage

### 1. Download

Clone the repository or download the script directly:

```bash
git clone [https://github.com/YourUsername/Arch-Postinstall-Tool.git](https://github.com/YourUsername/Arch-Postinstall-Tool.git)
cd Arch-Postinstall-Tool
