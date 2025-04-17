# Schedule 1 Basic Teleport Mod

A simple, lightweight mod for Schedule 1 that provides teleportation keybinds and utility functions without a GUI overlay.

## Features

- Teleport instantly to key locations using simple key presses
- Save game progress with a single key
- Change game time between day and night
- Works only when the game window is in focus
- Minimal performance impact

## Keybinds

### Teleportation
- `B` - Teleport to Bungalow
- `N` - Teleport to Barn
- `R` - Teleport to Laundromat
- `I` - Teleport to Docks
- `H` - Teleport to Sweatshop

### Utilities
- `Q` - Save game progress
- `O` - Set time to 07:00 (morning)
- `P` - Set time to 23:00 (night)

## Installation

1. Install [MelonLoader](https://melonwiki.xyz/#/) for Schedule 1 if you haven't already
2. Download the `BasicTeleportMod.dll` file
3. Place the DLL in the `Mods` folder in your Schedule 1 installation directory
   - Typically located at `Steam\steamapps\common\Schedule 1\Mods`
4. Launch the game
5. The mod will automatically initialize and all keybinds will be ready to use

## How It Works

This mod uses reflection to find and execute game commands directly, without any UI elements or console visibility. When you press a hotkey while the game is in focus, the corresponding command is executed in the background.

The mod also includes a window focus check to ensure that hotkeys only work when the game window is active, preventing accidental inputs in other applications.

## Requirements

- Schedule 1 game
- MelonLoader v0.5.3 or newer
- .NET Framework 4.7.2 or newer

## Troubleshooting

If the mod doesn't work:
- Make sure MelonLoader is properly installed
- Check the MelonLoader logs for any error messages
- Verify that the mod DLL is in the correct Mods folder
- Make sure you have the correct permissions to run the mod
- Update to the latest version of Schedule 1 and MelonLoader

Common errors:
- "Console instance or executeCommandMethod is null": The mod couldn't find the game's command system. This can happen if the game updates or changes its internal structure.
- "Error executing command": The command was found but couldn't be executed properly.

## Compatibility

This mod was tested with Schedule 1 and MelonLoader v0.5.3+.