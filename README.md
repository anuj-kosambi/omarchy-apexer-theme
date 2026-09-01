# Omarchy Apexer Theme

A near-black theme for [Omarchy](https://omarchy.org/) — a muted olive accent
over warm sand and clay highlights, tuned for long sessions on a dark screen.

![Apexer wallpaper](backgrounds/apexer.png)

## Palette

Dark mode. Accent is olive `#7b9d53`; the terminal brights lean warm (sand,
peach, clay) so diffs and syntax stay readable without glare.

| Role        | Hex       | Role         | Hex       |
| ----------- | --------- | ------------ | --------- |
| accent      | `#7b9d53` | background   | `#040404` |
| foreground  | `#e1e7e5` | selection    | `#1d1d1d` |
| muted       | `#726a6b` | red          | `#aa6769` |
| green       | `#d5b695` | yellow       | `#fcc8ac` |
| blue        | `#7b9d53` | magenta      | `#d16078` |
| cyan        | `#f0ecac` | orange       | `#b77e80` |

Full definitions live in [`colors.toml`](colors.toml).

## Installation

Requires an Omarchy installation. Install and apply in one command:

```bash
omarchy theme install https://github.com/anuj-kosambi/omarchy-apexer-theme.git
```

The theme is applied automatically after install. To apply it manually later:

```bash
omarchy theme set apexer
```

## What gets themed

Omarchy generates configuration for every app it covers from `colors.toml`
alone, so applying the theme restyles:

- **Terminals** — Alacritty, Foot, Kitty, Ghostty
- **Editors** — Neovim, Helix, VSCode, Obsidian
- **System tools** — btop, Hyprland
- **Omarchy shell** — bar, menus, notifications, lock screen

Icons are set to the `Yaru-red` variant via [`icons.theme`](icons.theme).

## Wallpapers

- **apexer.png** — the theme's default background

Add more backgrounds to `~/.config/omarchy/backgrounds/apexer/` or to the
theme's own `backgrounds/` directory, then cycle through them:

```bash
omarchy theme bg next
```

## Theming other apps

For apps Omarchy does not cover natively, drop a template at
`~/.config/omarchy/themed/[configname].tpl` and use the palette placeholders
(`{{ background }}`, `{{ accent }}`, `{{ color0 }}`–`{{ color15 }}`). See the
[Omarchy theming manual](https://omarchy.org/manual/making-your-own-theme/).

## Credits

Palette generated with [Aether](https://omarchy.org/) for Omarchy v4 and
hand-tuned from there.
