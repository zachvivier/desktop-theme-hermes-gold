# Hermes Gold

![Hermes Gold palette preview](assets/hermes-gold-preview.png)

A warm gold-on-charcoal theme for [Hermes Agent](https://github.com/NousResearch/hermes-agent). It is based on the visual palette of the Hermes Agent website and applies across the **desktop app, TUI, and CLI**.

## Palette

| Role | Color |
| --- | --- |
| Canvas | `#141414` |
| Elevated surface | `#1B1B1D` |
| Header and code background | `#09090D` |
| Primary gold | `#FFD800` |
| Secondary amber | `#FFBE00` |
| Bronze | `#CD8032` |
| Primary text | `#E9E4DC` |
| Muted text | `#8C8C8D` |
| Borders | `#484122` |

## Install

Hermes Agent must already be installed.

```bash
mkdir -p "${HERMES_HOME:-$HOME/.hermes}/skins"
curl -fsSL \
  https://raw.githubusercontent.com/zachvivier/desktop-theme-hermes-gold/main/hermes-gold.yaml \
  -o "${HERMES_HOME:-$HOME/.hermes}/skins/hermes-gold.yaml"
hermes config set display.skin hermes-gold
```

Hermes should repaint automatically within a second. The theme also appears in the Appearance picker and `/skin` menu.

## Update

Run the download command again, then reselect the theme if needed:

```bash
curl -fsSL \
  https://raw.githubusercontent.com/zachvivier/desktop-theme-hermes-gold/main/hermes-gold.yaml \
  -o "${HERMES_HOME:-$HOME/.hermes}/skins/hermes-gold.yaml"
hermes config set display.skin hermes-gold
```

## Revert or uninstall

```bash
hermes config set display.skin default
rm "${HERMES_HOME:-$HOME/.hermes}/skins/hermes-gold.yaml"
```

## Customize

With `hermes-gold` active, change one token without replacing the rest of the palette:

```bash
hermes skin set ui_accent "#FFD800"
```

The complete theme is contained in [`hermes-gold.yaml`](hermes-gold.yaml).

## License

MIT
