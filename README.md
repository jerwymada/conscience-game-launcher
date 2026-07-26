# Conscience Game Launcher

[![Version](https://img.shields.io/badge/version-1.2.1-4edea3)](CHANGELOG.md)
[![Platform](https://img.shields.io/badge/platform-Windows%20x64-0078d4)](docs/INSTALLATION.md)
[![Runtime](https://img.shields.io/badge/runtime-.NET%2010-512bd4)](docs/INSTALLATION.md)

**Conscience Game Launcher** prepares, monitors, and restores safer Solo and
Online game sessions on Windows. It combines game launching, mod-tool
management, network isolation, diagnostics, and local recovery in one compact
application.

> [Lire en français](README.fr.md)

## Download

| Edition | Recommended for | Download |
|---|---|---|
| Setup | Most users. One-click installation and automatic prerequisite installation. | [Download Setup 1.2.1](downloads/ConscienceGameLauncher-Setup-v1.2.1.exe) |
| Portable | Users who prefer a removable, self-contained application folder. Microsoft runtimes must already be installed. | [Download Portable 1.2.1](downloads/ConscienceGameLauncher-v1.2.1-portable-win-x64.zip) |

Both editions are lightweight and require:

- Windows 10 or Windows 11, x64
- [.NET 10 Desktop Runtime, x64](https://aka.ms/dotnet/10.0/windowsdesktop-runtime-win-x64.exe)
- [Microsoft Edge WebView2 Evergreen Runtime](https://go.microsoft.com/fwlink/p/?LinkId=2124703)

The Setup edition downloads missing Microsoft prerequisites automatically.

## Highlights

- Detects games installed through supported official launchers and standard
  Windows executables.
- Keeps Solo isolation active while official launchers finish starting a game.
- Verifies and restores managed firewall, hosts, and network-adapter state.
- Identifies supported mod managers and trainers while avoiding broad
  name-based process matching.
- Enables manual mod-tool launching only during an active Solo game session.
- Closes identified modding tools before Online launches.
- Uses a restricted UAC helper for protected Windows operations while the UI,
  games, and mod tools remain at standard user privilege.
- Stores configuration and logs locally. There is no remote update check.
- Provides built-in diagnostics and recovery actions.

## Start Here

1. Read the [installation guide](docs/INSTALLATION.md).
2. Follow the [user guide](docs/USER-GUIDE.md).
3. Verify the download with the [checksum guide](docs/VERIFY-DOWNLOADS.md).
4. Review [troubleshooting](docs/TROUBLESHOOTING.md) if a launcher, game, or mod
   tool is not detected.

## Important Safety Note

This application reduces accidental crossover between Solo modding and Online
play, but it cannot guarantee compatibility with every game, launcher,
anti-cheat system, mod, or publisher policy. Always follow the rules of the
game and platform you use. Do not launch mod tools during Online play.

## Data and Privacy

The application does not upload game, mod, configuration, or diagnostic data.

- Installed edition: `%LocalAppData%\ConscienceGameLauncher`
- Portable edition: `Data` beside `ConscienceGameLauncher.exe`

See [Security and privacy](SECURITY.md) for privilege, signing, and reporting
details.

## Authenticity

Version 1.2.1 is currently **not code-signed**. Verify the SHA-256 checksum
before running a downloaded file:

- [SHA256SUMS.txt](downloads/SHA256SUMS.txt)
- [Verification guide](docs/VERIFY-DOWNLOADS.md)

Copyright © 2026 JERWY. All rights reserved.
