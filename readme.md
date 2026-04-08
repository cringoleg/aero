# AeroSpace Tiling WM Setup

Keyboard-driven tiling window manager for macOS with instant workspace switching. No animations, no SIP disabling.

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
