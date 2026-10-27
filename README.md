# Yozora ヨゾラ — Theme

A dark, night-blue browser theme for Chromium browsers (Brave, Chrome, Edge, Vivaldi, Opera…), with matching [Dark Reader](https://darkreader.org) presets.
It pairs with the [Yozora new tab page](https://github.com/Sync-Kai/yozora-newtab).

## Palette

| Role | Color |
|---|---|
| Window frame | `#11131a` |
| Toolbar | `#1a1d27` |
| Text | `#e8eaf0` |
| Accent (lavender) | `#a99cf2` |

## Installation (developer mode)

1. Clone the repository:
   ```bash
   git clone https://github.com/Sync-Kai/yozora-theme.git
   ```
2. Open `brave://extensions` (or `chrome://extensions`, `edge://extensions`…).
3. Turn on **Developer mode**.
4. Click **Load unpacked** and select the `yozora-theme` folder (the one that contains `manifest.json`).

The theme applies immediately. To go back to the default theme, open the appearance settings and click **Reset to default**.

### Stable extension ID

`manifest.json` contains a fixed public `key`, so the theme keeps the same ID (`jbgakplacolpbmpdcchpihgnjgdolodi`) wherever the folder lives.

> Before you publish to the Chrome Web Store, remove the `key` field from the packaged manifest. The store assigns its own key.

## Dark Reader presets

The `dark-reader/` folder holds four settings files. Each one matches an accent color of the new tab page:

| File | Accent |
|---|---|
| `yozora-lavande.json` | lavender `#a99cf2` |
| `yozora-ambre.json` | amber `#f2b56b` |
| `yozora-menthe.json` | mint `#6fd3b0` |
| `yozora-corail.json` | coral `#f2877a` |

All four darken pages to the theme's background (`#11131a`) and text color (`#e8eaf0`), and use the accent as the selection color.

**Import a preset:**

1. Install [Dark Reader](https://darkreader.org).
2. Open its popup, then go to **Settings** → **Advanced** → **Import settings**.
3. Choose one of the `.json` files.

> Importing a preset replaces your current Dark Reader settings, including your site lists. Export them first if you want to keep them.

## Project structure

```
manifest.json      Theme manifest (MV3)
_locales/          Theme name and description per language (en, fr, nl, de, es)
dark-reader/       Dark Reader presets
```

## Related

- [yozora-newtab](https://github.com/Sync-Kai/yozora-newtab): the new tab page extension.
