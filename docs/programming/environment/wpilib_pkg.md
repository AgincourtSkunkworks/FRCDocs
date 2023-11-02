---
title: WPILib Software Package
weight: 100
---

# Installing WPILib Software Package
[Official Documentation](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-2/wpilib-setup.html)

If you are not *running* the code, and are only planning on editing it, then this package will install additional programs that you won't ever be using. You can follow the standard [onboarding](index.md#onboarding) process instead.

You can also choose to use this package instead to install Java & VS Code in one step, if you don't mind the additional software bloat, just remember to follow the [Git & GitHub](git.md) guide as well.

## Requirements
- 64-bit Operating System
- `glibc>=2.34` for Linux

## Download + Extract
1. Download the [latest release](https://github.com/wpilibsuite/allwpilib/releases/latest)
    - Select the correct binary for your operating system.
2. Extract the downloaded file
    
    === "Windows"
        1. Mount the `.iso` image by right-clicking it, then clicking `Mount`.
            - If you have 7-Zip, you can also extract directly with right-click → `7-Zip` → `Extract to X`.
        2. Open the mounted/extracted location, and run `WPILibInstaller.exe`

        !!!note

            If prompted by Window's Defender, click `More Info`, then `Run Anyway`.

    === "Linux"
        1. Extract the `.tar.gz` archive
            - `#!bash tar -xf WPILib_Linux-<version>.tar.gz`
        2. Open the extracted folder, and run `WPILibInstaller`
            - `#!bash cd WPILib_Linux-<version>`
            - You may need to make it executable with:  
            `#!bash sudo chmod +x WPILibInstaller`

    === "MacOS"
        1. Install the `Xcode Command Line Tools`
            - `#!bash xcode-select --install`
        2. Double-click the downloaded `dmg` and launch `WPILibInstaller`

## Running
1. Once the installer is run (see previous tabs), go through the installer
2. Once you reach the prompt for the install mode, it is recommended you select `Everything`, otherwise you will need to install and configure [VS Code](vs_code.md) manually.
    - `Tools Only` installs only the WPILib tools (Pathweaver, Shuffleboard, RobotBuilder, SysID, Glass, and OutlineViewer), as well as the Java JDK.
    - `Everything` installs VS Code, extensions, WPILib tools (see above), the Java JDK, and all dependencies
3. If prompted to select a VS Code install method, choosing `Download for this computer only` is recommended

## Reboot
You may be asked to reboot your computer after the installation is complete. If so, do so.
