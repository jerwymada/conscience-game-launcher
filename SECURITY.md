# Security and Privacy

## Supported Version

Only the latest published version is supported:

| Version | Supported |
|---|---|
| 1.2.1 | Yes |
| Older versions | No |

## Windows Privileges

The main application runs with standard user rights. Games and mod tools
started by the application therefore also run with standard rights.

Protected operations such as firewall changes, hosts-file changes,
network-adapter state, and anti-cheat service control use a restricted helper.
Windows displays a UAC prompt before that helper starts. Rejecting the prompt
blocks the affected safety step.

The Setup executable requests administrator permission because it installs
under Program Files and may install official Microsoft prerequisites. The
installer does not launch the application from its elevated process.

## Code Signing

Version 1.2.1 is not digitally signed. Windows SmartScreen may display a
reputation warning. Verify the SHA-256 checksum from
[`downloads/SHA256SUMS.txt`](downloads/SHA256SUMS.txt) before running either
download.

## Local Data

Conscience Game Launcher does not include telemetry, cloud synchronization, or
a remote update service. Configuration, backups, and diagnostic logs remain on
the local computer.

Logs may contain local file paths, process names, game names, or launcher
details. Review exported logs before attaching them to a public issue.

## Reporting a Security Issue

Open a GitHub issue only for non-sensitive reports. Do not include personal
paths, tokens, private logs, or proof-of-concept material that could put users
at risk. For a sensitive report, contact the repository owner privately through
their GitHub profile and provide a minimal description first.

## Scope

The application helps maintain separation between Solo modding and Online
play. It is not an anti-cheat bypass and does not guarantee protection from
publisher enforcement. Users remain responsible for following game and
platform rules.
