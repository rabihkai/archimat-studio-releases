# Archimat Studio

Archimat Studio is a Windows app for Archimat that turns a short description of a room
(and, if you like, a few reference photos and catalog products) into photorealistic images
of kitchens, bathrooms, bedrooms and hotel rooms. Every image is kept with its history and
can be changed later.

This page only holds the installers. There is no source code here.

## Install

1. Open the [latest release](https://github.com/rabihkai/archimat-studio-releases/releases/latest)
   and download `ArchimatStudio-Setup-x.y.z.exe` (under **Assets**).
2. Run it. Windows may show "Windows protected your PC" because the installer is not signed yet:
   click **More info**, then **Run anyway**.
3. Archimat Studio opens in your web browser. The first time, it opens **Settings**, where you
   paste the two API keys you were given.

The app installs for your Windows account only (no administrator rights needed). It needs
Windows 10 or 11, 64-bit, and an internet connection to make images.

## Updates

Archimat Studio checks each time it starts and once a day whether a newer version is published here. When there is one,
a notice at the top of its page shows what is new and a **Download and install** button: Studio
closes, installs the update and opens again. You can also download the newest installer from the
[latest release](https://github.com/rabihkai/archimat-studio-releases/releases/latest) and run it
over the installed app. The daily check can be turned off in Settings.

Your projects, settings and API keys are not in the program folder, so updating or uninstalling
never removes them:

- projects and images: `Documents\Archimat Studio Library`
- settings and logs: `%LOCALAPPDATA%\Archimat Studio`

## Check a download (optional)

Each release also has a `.sha256` file. In PowerShell:

```powershell
Get-FileHash .\ArchimatStudio-Setup-x.y.z.exe -Algorithm SHA256
```

The hash shown must be the one in the `.sha256` file and in the release notes.

## Uninstall

Windows Settings > Apps > Installed apps > Archimat Studio > Uninstall. Your projects and
settings stay where they are.
