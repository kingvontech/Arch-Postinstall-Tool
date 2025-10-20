Arch Post-install Tool (v3.0.1)

An intelligent, modular, and interactive TUI (Terminal User Interface) script designed to simplify the post-installation configuration of Arch Linux, with a primary focus on setting up modern Wayland environments like Hyprland.

The tool guides the user through essential steps, including:

GPU driver selection (NVIDIA, AMD, Intel).

Installation of an AUR helper (yay).

Intelligent selection of hardware-specific patches (e.g., microcode, iGPU fixes).

Installation of packages, shell configuration (Zsh, Fastfetch), and dotfiles.

🚀 Key Features

Modular Architecture: The script is now split into six functional components inside the modules/ directory for dramatically improved maintainability and scalability (Version 3.0.1).

Essential Patching: Automatically applies critical kernel parameters and configuration patches based on detected hardware (CPU microcode, i915 PSR fix, etc.).

User Privilege Safety: Safely executes user-specific actions (dotfile installs, shell configuration) as the non-root user via the execute_as_user utility.

Customization Menus: Dedicated TUI menus for advanced configuration of popular tools like Zsh and Fastfetch.

⚙️ How to Run

Prerequisites: Ensure your base Arch installation is complete and you have a user account set up with sudo privileges.

Download and Extract:

Go to the releases page and download the latest .tar.gz file (e.g., Arch-Postinstall-Tool-v3.0.1.tar.gz). Then, use the following commands to extract the archive.

# Download the file (replace URL with the correct one from your releases)
wget https://github.com/kingvontech/Arch-Postinstall-Tool/releases/download/Version3.0.1/Arch-Postinstall-Tool-v3.0.1.tar.gz

# Extract the archive. This creates the tool's directory.
tar -xvzf Arch-Postinstall-Tool-v3.0.1.tar.gz


Navigate to Directory:

cd Arch-Postinstall-Tool


Set Permissions: Grant execute permission to the main script.

chmod +x Arch-Postinstall-Tool.sh


Execute the Script: Run the main script with sudo. It will safely drop privileges for user-level actions.

sudo ./Arch-Postinstall-Tool.sh


Follow the TUI: Use the interactive menu to define your system configuration, drivers, packages, and theme.
