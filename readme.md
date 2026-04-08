# AeroSpace Tiling WM Setup

This is my own config for aerospace - keyboard-driven tiling window manager for macOS with instant workspace switching. No animations, no SIP disabling.

It is configured to use capslock key changed to work as hyper-key (shift + option + ctrl + cmd) which enables collision free shortcut usage - macos does not use hyper combinations. You also don't have wait for the focus to catch app to your switching - which was the main headache for me. 


## Install

```bash
brew install --cask nikitabobko/tap/aerospace
brew install --cask hyperkey
cp aerospace.toml ~/.aerospace.toml
```

## Hyperkey Setup

1. Open Hyperkey, grant Accessibility permissions when prompted.
2. Set **Caps Lock** as the Hyper key.

## Keybindings

**Hyper** = Caps Lock (held) = Ctrl + Shift + Cmd + Alt

### Workspaces

| Action | Binding |
|--------|---------|
| Switch to workspace | Hyper + key |
| Send window to workspace | Ctrl + Cmd + key |
| Toggle last two workspaces | Hyper + Tab |
| Move workspace to next monitor | Hyper + ` |

Available workspaces: `1-4`, `Q W E R T`, `A S D G`, `Z X C V B`

### Windows

| Action | Binding |
|--------|---------|
| Focus | Hyper + H/J/K/L |
| Move/swap | Hyper + [ ] ; ' |
| Resize | Hyper + - / = |
| Fullscreen | Hyper + F |
| Balance sizes | Hyper + B |
| Layout toggle (tiles) | Hyper + / |
| Layout toggle (accordion) | Hyper + , |

### Service Mode (Hyper + .)

| Action | Key |
|--------|-----|
| Reload config & exit | Esc |
| Reset layout | R |
| Toggle float/tile | F |
| Close other windows | Backspace |
| Join with neighbor | Hyper + H/J/K/L |

## Uninstall

```bash
brew uninstall --cask nikitabobko/tap/aerospace
brew uninstall --cask hyperkey
rm ~/.aerospace.toml
```
