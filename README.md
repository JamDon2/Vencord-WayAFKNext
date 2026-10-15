# Vencord-WayAFKNext

Automated builds of [Vencord](https://github.com/Vendicated/Vencord) with the [WayAFKNext](https://github.com/MuffinTastic/WayAFKNext) plugin included.

## What is this?

WayAFKNext makes AFK timeout (idle detection) work on Wayland compositors (Hyprland, Sway, etc). This repo automatically builds Vencord with the plugin every 6 hours and publishes releases.

## Installation (Arch Linux)

```bash
yay -S vesktop-wayafknext-bin
```

**[AUR Package →](https://aur.archlinux.org/packages/vesktop-wayafknext-bin)**

## How it works

1. GitHub Actions checks for new Vencord commits every 6 hours
2. If there's a new commit, it builds Vencord with WayAFKNext
3. The AUR package patches Vesktop to download from this repo instead of upstream

## Credits

- [Vencord](https://github.com/Vendicated/Vencord) - The Discord client mod
- [Vesktop](https://github.com/Vencord/Vesktop) - Standalone Vencord desktop app  
- [WayAFKNext](https://github.com/MuffinTastic/WayAFKNext) - Wayland idle detection plugin by MuffinTastic
