# Releases

Installers for the apps in the suite, and `catalog.json`, the list [Hangar](https://github.com/RohithOrg/hangar) reads to install and update them. This repository holds no source code.

## Get started

Download **Hangar** from the [latest release](https://github.com/RohithOrg/releases/releases/latest), then install every other app from inside it. Hangar keeps them up to date.

| Your computer | Download |
|---|---|
| Mac with Apple silicon (M1 or newer) | `hangar-<version>-macos-aarch64.dmg` |
| Windows 10 or 11 | `hangar-<version>-windows-x86_64.exe` |
| Linux (x86-64) | `hangar-<version>-linux-x86_64.AppImage` |

## Opening it the first time

The apps aren't signed with a paid Apple or Microsoft certificate yet, so your system asks once before opening a downloaded installer. Apps installed through Hangar afterwards don't ask.

**Mac**
1. Open the `.dmg` and drag Hangar into Applications.
2. Open Hangar. macOS says *"Apple could not verify Hangar is free of malware"*. Click **Done**.
3. Go to **System Settings → Privacy & Security**, scroll down and click **Open Anyway** next to Hangar, then confirm with your password.

**Windows**
1. Run the installer. If *"Windows protected your PC"* appears, click **More info**, then **Run anyway**.
2. Hangar installs for your user account only; no administrator password is needed.

**Linux**
1. Make the file runnable: right-click → Properties → *Allow executing as program*, or `chmod +x hangar-*.AppImage`.
2. Double-click it. On Ubuntu 22.04 or newer, if nothing happens, install FUSE 2 first: `sudo apt install libfuse2`.

## Is it safe?

Every installer here is signed with the suite's release key, and Hangar checks that signature and the file's SHA-256 before installing anything. A file that doesn't match is refused.

Updates never touch your data. Each app keeps its files outside the app itself (Job Command Center uses `Documents/Job Command Center`), so updating or reinstalling keeps everything.
