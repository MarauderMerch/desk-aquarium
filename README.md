# Desk Aquarium

An idle aquarium game: five tanks (a coral reef, Amazon blackwater, Lake Malawi, an Iwagumi
aquascape and fancy goldfish), each stocked with real species that the hobby keeps together.
Happy fish earn coins for more fish, decor and upgrades. No fish ever dies.

**These builds are for playtesting.** This page holds only the releases; send what you find to
whoever sent you the link.

## Install

It needs **Windows 10 or 11, 64-bit**, and a graphics card with **OpenGL 3.3**, which is nearly
any PC from the last ten years.

1. Download **[DeskAquarium-Setup.zip](https://github.com/MarauderMerch/desk-aquarium/releases/latest/download/DeskAquarium-Setup.zip)** (about 50 MB).
2. Right-click it and choose **Extract All**.
3. Open `DeskAquarium\install` and double-click **Install Desk Aquarium.cmd**.
   - If Windows says "Windows protected your PC", click **More info**, then **Run anyway**.
   - If the PC has no Python 3.13, the setup installs it. Windows asks once to allow it.
4. When it says **Done**, open **Desk Aquarium** from the Desktop. The extracted folder can then
   be deleted.

## Updates

At each start the game looks at this page's newest release. When there is a newer version it
asks before installing it, and your tank and progress are kept. Nothing to download again.

## Playing

A short tutorial runs the first time. The main controls:

| Input | Does |
|---|---|
| Click a fish | its card |
| F or Space | feed |
| C | clean the glass (drag to wipe) |
| B / T / P | Shop / Tanks / Fincyclopedia |
| Wheel, right drag | zoom, pan |
| F11 | fullscreen |
| F12 / Shift+F12 | a photo, without / with the menus |
| Esc | close a panel, or the menu (settings, save and quit) |

Touch screens work too: tap, drag, pinch, and a long press for a tooltip.

## If something goes wrong

Send these:
- the setup's log, `%TEMP%\desk-aquarium-install.log`
- the game's log, `%TEMP%\desk-aquarium-game.log`
- any photos, in `Pictures\Desk Aquarium`

To open a `%TEMP%\...` path, paste it into File Explorer's address bar. If the setup says the game
could not draw with OpenGL, update the graphics driver (Windows Update) and run it again.

## What it installs, and removing it

| What | Where |
|---|---|
| The game | `%LOCALAPPDATA%\Programs\DeskAquarium` |
| Your save | `%APPDATA%\DeskAquarium` |
| The shortcut | **Desk Aquarium** on the Desktop, and its launcher in `C:\ProgramData\DeskAquarium` |
| Python 3.13, if it was missing | Settings, Apps |
| pygame, moderngl and numpy | `%APPDATA%\Python\Python313` |

To remove it, delete the shortcut and those folders. Deleting `%APPDATA%\DeskAquarium` deletes
your progress.

## Privacy

The game sends nothing about you or your PC. At each start it downloads `latest.json` from this
page's newest release to see whether there is an update, and GitHub sees that request as it sees
any download.
