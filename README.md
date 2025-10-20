# Arch Post-install Tool (v3.0.1)

An intelligent, modular, and interactive TUI (Terminal User Interface) script designed to simplify the post-installation configuration of Arch Linux, with a primary focus on setting up modern Wayland environments like **Hyprland**.

The tool guides the user through essential steps, including:
* GPU driver selection (NVIDIA, AMD, Intel).
* Installation of an AUR helper (`yay`).
* Intelligent selection of hardware-specific patches (e.g., microcode, iGPU fixes).
* Installation of packages, shell configuration (Zsh, Fastfetch), and dotfiles.

## 🚀 Key Features

* **Modular Architecture:** The script is now split into six functional components inside the `modules/` directory for dramatically improved maintainability and scalability (Version 3.0.1).
* **Essential Patching:** Automatically applies critical kernel parameters and configuration patches based on detected hardware (CPU microcode, i915 PSR fix, etc.).
* **User Privilege Safety:** Safely executes user-specific actions (dotfile installs, shell configuration) as the non-root user via the `execute_as_user` utility.
* **Customization Menus:** Dedicated TUI menus for advanced configuration of popular tools like **Zsh** and **Fastfetch**.

## ⚙️ How to Run

1.  **Prerequisites:** Ensure your base Arch installation is complete and you have a user account set up with `sudo` privileges.
2.  **Download/Clone:**

Go to releases and download the leatest version of the .tar.gz file and ecstract the file

3. now ```bash
   cd Arch-postinstall-Tool
   chmod +x Arch-Postinstall-Tool.sh 
    ```
4.  **Execute the Script:** Run the main script with `sudo`. It will safely drop privileges for user-level actions.
    ```bash
    sudo ./Arch-Postinstall-Tool.sh
    ```
5.  **Follow the TUI:** Use the interactive menu to define your system configuration, drivers, packages, and theme.
