# Hyprland Config — Minimal-Functional

Ported from `ubuntu-dots/i3/config` to Hyprland. Style: Catppuccin Mocha + JetBrainsMono Nerd Font.

## Layout

- `hypr/hyprland.conf` — main config: 105 keybinds, workspace pinning, window rules
- `hypr/hyprpaper.conf` — wallpaper daemon
- `waybar/config.jsonc` — minimal-functional bar: workspaces | window | clock | tray·net·vol·power
- `waybar/style.css` — Catppuccin Mocha theme

## Pinned workspaces

| WS | App |
|----|-----|
| 1 | Terminal (kitty) |
| 2 | Browser (Zen + Firefox) |
| 3 | Editor (VSCode) |
| 4 | Slack |
| 5 | Email (Thunderbird) |
| 6 | Discord |
| 7 | Notes (Obsidian) |
| 8 | Music/Media |
| 9-10 | Free |

## Dependencies

Required:
- `hyprland` `waybar` `hyprpaper` `hyprlock` `hypridle` `hyprpolkitagent`
- `kitty` `rofi` `dunst` `wl-clipboard` `cliphist`
- `grim` `slurp` (screenshots)
- `jq` `pactl` `playerctl` `nm-applet` `udiskie`

Companion repo for rofi scripts: [shaiknoorullah/rofi](https://github.com/shaiknoorullah/rofi)

## Install

```bash
git clone https://github.com/shaiknoorullah/hyprland-config.git ~/.config/hyprland-config-src
ln -sf ~/.config/hyprland-config-src/hypr/hyprland.conf  ~/.config/hypr/hyprland.conf
ln -sf ~/.config/hyprland-config-src/hypr/hyprpaper.conf ~/.config/hypr/hyprpaper.conf
ln -sf ~/.config/hyprland-config-src/waybar/config.jsonc ~/.config/waybar/config.jsonc
ln -sf ~/.config/hyprland-config-src/waybar/style.css    ~/.config/waybar/style.css
```

You also need `monitors.conf` and `nvidia.conf` in `~/.config/hypr/` (machine-specific).
