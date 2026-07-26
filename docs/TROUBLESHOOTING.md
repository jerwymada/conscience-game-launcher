# Troubleshooting

## The application does not start

- Confirm that Windows is x64.
- Install [.NET 10 Desktop Runtime, x64](https://aka.ms/dotnet/10.0/windowsdesktop-runtime-win-x64.exe).
- Install [Microsoft Edge WebView2 Evergreen Runtime](https://go.microsoft.com/fwlink/p/?LinkId=2124703).
- For Portable, extract the complete ZIP before starting the EXE.
- Verify the download checksum.

## Windows SmartScreen displays a warning

Version 1.2.1 is not code-signed. Compare the file's SHA-256 checksum with
`downloads/SHA256SUMS.txt`. Continue only when the checksum matches a file
downloaded from this repository.

## The application says another instance is open

Restore the existing window from the notification area and close it normally.
The application allows one UI instance and one restricted elevated helper.

## The application refuses to run as administrator

This is intentional. Close the elevated instance and start the application from
its normal shortcut. The UI, games, and mod tools must run with standard rights.

## A launch is blocked after UAC consent

Read the failed session step. UAC consent only starts the restricted helper; a
later verification can still fail. Open Diagnostics and restore the environment
before retrying.

## The game process is not detected

Official launchers may take several minutes to transition from their launcher
process to the game process. Solo isolation remains active during this wait.
For a manually added game, confirm that the selected executable is the real game
executable rather than an updater or bootstrapper.

## A mod launch button is disabled

Mod tools can launch only when:

- A Solo session is active
- The real game process has been detected
- Cleanup has not started
- The configured mod executable still exists
- The mod tool is not already running

Use **Add > Add Mod** when automatic detection found a product but could not
resolve a launchable executable.

## Environment restoration needs attention

Keep the application open, go to Diagnostics, and use the corresponding restore
action. Do not start an Online game until hosts, firewall, network, and
anti-cheat recovery checks are clear.

## Log locations

- Installed: `%LocalAppData%\ConscienceGameLauncher\Logs`
- Portable: `Data\Logs` beside the executable

Review logs before sharing because they can contain local paths and process
names.
