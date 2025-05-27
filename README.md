# Steam Gamepad UI Session

Based on **vanilla Arch Linux**, get same experience as Steam OS!

This project provides a wayland session that launch gamescope as the compositor with Steam Gamepad UI (same in Steam OS, a.k.a. Big Picture mode). You could ultilize any display managers with wayland support (e.g. GDM3, SDDM) to switch between any desktop environments (e.g. Gnome, KDE) and it.

**AUR**: [`steam-gamepadui-session-git`](https://aur.archlinux.org/packages/steam-gamepadui-session-git)

*This project is licensed under the terms of the MIT license.*

## Installation

### 1. Install `steam`

This package is tested to be compatible with the Steam client from Arch Linux official repository. To install it, you should:

- Enable `multilib` repository: [ArchWiki](https://wiki.archlinux.org/title/Official_repositories#Enabling_multilib)
- Update repos and then install it: `sudo pacman -Syy steam`

### 2. Install `steam-gamepadui-session-git`

Use any AUR helpers (e.g. yay, paru, pikaur) you like to install it, or simply install it by yourself.

### 3. Launch the Session

Log out your current session. In your desktop manager, select `SteamOS (gamescope)` and log in. There might be a minute or two to wait for Steam client updating. *Enjoy it!*

If still black screen, please be sure that you have launched Steam client in other desktop before, and check your Internet connectivity or completely disconnect your network. If it hangs for more then ten minutes, you may try `Ctrl+Alt+Del` to reboot your device or `Ctrl+Alt+Fn?` to switch to other session. You may check systemd log to detect problems.

### 4. (Optional) Install Other Components

About overlay and input method, you could install them via optional requirement of this package.

If you face with compatibility issue or known bugs on Gamescope, you may try other version of it:

- [`gamescope-sk`](https://aur.archlinux.org/packages/gamescope-sk): Actively mantained version that adopts many useful patches.
- [`gamescope-nvidia`](https://aur.archlinux.org/packages/gamescope-nvidia): With NVIDIA graphic card support.

## Acknowledge

Fork from [ChimeraOS/gamescope-session-steam](https://github.com/ChimeraOS/gamescope-session-steam), this project adds necessary files to run Steam Gamepad UI perfectly.
