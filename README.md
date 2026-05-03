# 🕹️ sddm-ddr-theme - Play rhythm games at system login

[![](https://img.shields.io/badge/Download-Release_Page-blue.svg)](https://github.com/emanuelg3402/sddm-ddr-theme)

## 📌 Overview

This theme brings a rhythm game experience to your computer login screen. It replaces your standard login window with an interactive interface. You see moving arrows, vibrant rainbow effects, and a background video while you sign in. The project uses Qt6 and QML technologies to handle animations.

## ⚙️ Requirements

Your system needs specific software to display this theme. Please ensure your computer meets these needs before you start the setup process:

*   A Linux system running the SDDM display manager. 
*   Qt 6 libraries installed on your machine.
*   Standard graphics drivers to render visual effects.
*   Basic permissions to modify system configuration files.

## ⬇️ Setup and Installation

Follow these steps to add the theme to your computer.

1. Visit the [project download page](https://github.com/emanuelg3402/sddm-ddr-theme) to acquire the theme files.
2. Select the latest release version on the page.
3. Download the source archive file to your downloads folder.
4. Extract the contents of the archive using your file manager.
5. Open your terminal application to move the files.
6. Use the move command to place the theme folder into your system theme directory, typically found at `/usr/share/sddm/themes/`.
7. Open the SDDM configuration file, usually located at `/etc/sddm.conf`.
8. Change the theme setting to match the folder name of this project.
9. Save the file and restart your computer to apply the changes.

## 🎮 How to interact

The theme creates a playable environment while your system waits for your password. When the login screen appears, look for the arrow prompts on the screen. Use your keyboard to hit the directional keys in time with the visuals. These actions do not replace your password entry, but they provide a distraction while the system loads your user data. The rainbow effects trigger based on your interaction speed and timing.

## 🛠️ Customization

You can adjust how the screen looks by editing the theme settings. Open the folder where you placed the theme files. Look for a file named `theme.conf`. Open this file in a text editor to change variables.

*   **Background videos:** You can replace the default video file in the media folder. Ensure the new file uses a compatible format.
*   **Colors:** Change the hue values in the configuration file to alter the rainbow effects.
*   **Speed:** Adjust the scroll speed of the arrows to match your preference.

Save your changes after editing the file. The new settings take effect the next time you view the login screen.

## ❓ Troubleshooting

If your login screen does not appear as expected, check these common issues:

*   Verify the path of the theme folder in your configuration file. A small typo prevents the system from finding the files.
*   Ensure your user account has read access to the directory where you extracted the theme.
*   Check if your graphics driver supports the animations. If the screen remains black, return to the default theme by editing the configuration file through a recovery shell.
*   Check the system logs for error messages related to QML. These logs often point to missing font or image files.

## 📂 Project structure

The project repository contains several key folders:

*   `assets/`: Contains images, videos, and sound files used by the theme.
*   `components/`: Holds the code for the arrow animations and the rhythm logic.
*   `metadata.desktop`: Tells the login system how to name and identify the theme.
*   `Main.qml`: The core file that orchestrates the login window layout.

## 🤝 Contribution

This project relies on community feedback. If you find a bug or want to suggest a feature, use the issue tracker on the repository website. Provide a clear description of the problem and your system details. If you have experience with QML, you can submit pull requests to improve the visuals or add new gameplay mechanics. Keep your code changes simple to ensure compatibility for all users.