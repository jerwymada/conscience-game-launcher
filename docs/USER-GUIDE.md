# User Guide

## Library

The Dashboard opens on **Games** by default. Use the Games/Mods selector below
the search field to change the visible library.

- **Refresh** rescans installed game launchers and known mod tools.
- **Add > Add Game** registers a game executable manually.
- **Add > Add Mod** registers a mod, trainer, or mod manager executable.
- The kebab menu on a manually added item contains its **Remove** action.
  Removing an entry never deletes the underlying program files.

Automatically detected entries cannot be removed from the inventory. Games can
be hidden from their kebab menu.

## Solo Session

1. Select a game.
2. Choose **Play Solo**.
3. Accept the UAC prompt when a protected Windows operation is required.
4. Wait for every preflight step and for the real game process to be detected.
5. Launch identified mod tools from the **Solo Mods** area.
6. Close the game normally or use **Abort Session & Restore**.

The launcher keeps Solo isolation active while an official launcher is still
starting the game. Closing Conscience Game Launcher during a protected session
first requests cancellation and waits for cleanup.

## Online Session

1. Close mod tools that are not managed by the application.
2. Select the game and choose **Play Online**.
3. The launcher closes identified mod tools, clears managed traces, removes Solo
   isolation, and verifies network access before starting the game.

Mod-tool launching is unavailable during Online sessions. Do not manually
start trainers or mod tools while playing Online.

## Settings

- **Hosts blocking:** adds the managed Solo hosts block.
- **Killswitch:** disables all targeted physical network adapters during Solo
  isolation and rolls back if any adapter cannot be disabled.
- **Save backup:** creates a local save backup before the selected session.
- **Auto Close:** keeps monitoring until the detected game process exits.
- **Block mod tool Internet access:** maintains outbound Windows Firewall rules
  for registered mod-tool executables.
- **Start with Windows:** disabled by default.
- **Minimize to notification area:** disabled by default.

Settings are stored locally and saved automatically.

## Diagnostics

Diagnostics reports the state of:

- Managed hosts entries
- Session firewall rules
- Network-adapter recovery
- Anti-cheat service recovery
- Persistent mod-tool network rules

Use the focused recovery actions when a check reports that restoration is
required. Export logs before reporting a reproducible problem, then review them
for personal file paths.
