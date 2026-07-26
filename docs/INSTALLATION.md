# Installation Guide

## Choose an Edition

### Setup edition

Recommended for most users. It installs the application under Program Files,
creates Start menu and desktop shortcuts, and downloads missing Microsoft
prerequisites.

1. Download `ConscienceGameLauncher-Setup-v1.2.1.exe`.
2. Verify its SHA-256 checksum.
3. Close any running Conscience Game Launcher instance.
4. Start the Setup and accept the Windows administrator prompt.
5. Wait while the installer checks .NET 10 Desktop and WebView2.
6. Start the application afterward from the desktop or Start menu shortcut.

The Setup intentionally does not launch the application from its elevated
installer process. The installed application runs with standard user rights.

### Portable edition

Recommended for a removable or manually managed folder.

1. Install the official [.NET 10 Desktop Runtime, x64](https://aka.ms/dotnet/10.0/windowsdesktop-runtime-win-x64.exe).
2. Install the official [Microsoft Edge WebView2 Evergreen Runtime](https://go.microsoft.com/fwlink/p/?LinkId=2124703).
3. Download and verify
   `ConscienceGameLauncher-v1.2.1-portable-win-x64.zip`.
4. Extract the entire ZIP to a writable folder.
5. Start `ConscienceGameLauncher.exe` from the extracted folder.

Do not run the executable directly from inside the ZIP. The portable edition
creates a `Data` directory beside the executable.

## Updating

### Setup

Close active game sessions and the application, then run the newer Setup. The
installer reuses the existing installation directory. User data under
`%LocalAppData%\ConscienceGameLauncher` is preserved.

### Portable

1. Close active sessions and exit the application from the notification area.
2. Keep the existing `Data` directory.
3. Replace `ConscienceGameLauncher.exe` and `readme.txt` with the files from the
   newer portable archive.

## Uninstalling

For the installed edition, use **Settings > Apps > Installed apps** in Windows.
User configuration and backups under `%LocalAppData%\ConscienceGameLauncher`
are retained unless you delete that directory manually.

For the portable edition, keep any backups you need and remove the extracted
application folder.

## French Summary

Le Setup est recommandé : il installe l'application en un clic et télécharge
les prérequis Microsoft manquants. La version portable doit être entièrement
extraite dans un dossier accessible en écriture et nécessite l'installation
manuelle de .NET 10 Desktop x64 et de WebView2. Ne lance jamais l'EXE directement
depuis l'archive ZIP.
