# Ono-Sendai

A terminal retro-look theme for [Obsidian](https://obsidian.md).

Dark-mode by default, with a secondary light mode. Designed for immersive, distraction-free note-taking with a phosphor-CRT aesthetic: deep blacks, vivid punctuation accents (electric cyan, terminal green, hot pink), and a dense information layout that keeps structure visible rather than hidden.

---

## Features

- Anti-distraction focus — visible structure instead of hidden chrome
- Tab icons replaced by text
- High-density layout with more content displayed at a glance
- Images scaled down with hover zoom
- File explorer: compact 12 px font, full filenames wrap (no truncation)
- Cascading heading indent (H3–H6 step 10 px per level)
- Aligned footnotes offset for consistent leading
- WCAG AA contrast compliant for all body text
- Supports both **dark mode** and **light mode**

---

## Installation

### Manual (recommended for personal use)

1. Download or clone this repository.
2. Open your vault's folder and navigate to `.obsidian/themes/`.
3. Create a subfolder named `Ono-Sendai` and copy these files into it:
   - `theme.css`
   - `variables.css`
4. In Obsidian, open **Settings → Appearance → Themes** and select **Ono-Sendai**.

> **Note:** `theme.css` uses `@import "variables.css"` — both files must live in the same folder.

### Optional: manifest.json

For the theme to appear in the community theme browser it needs a `manifest.json`. For local use no manifest is required. If you want to create one, place this in the theme folder:

```json
{
  "name": "Ono-Sendai",
  "version": "1.0.0",
  "minAppVersion": "1.6.0",
  "author": "your-name",
  "authorUrl": "",
  "isDesktopOnly": false
}
```

---

## Fonts

The theme is designed with **Cairo** as the primary UI font (geometric sans-serif, available on [Google Fonts](https://fonts.google.com/specimen/Cairo)). It falls back gracefully to Roboto → Inter → Segoe UI.

For monospace, **Fira Code** is recommended (fallback: Source Code Pro → system monospace).

To install Cairo on Linux:
```bash
# Download from Google Fonts or via your package manager
# e.g. on Arch: yay -S ttf-cairo
```

---

## Customisation

All design tokens live in `variables.css`. Edit the `.theme-dark` or `.theme-light` block to change colours, type sizes, or spacing without touching component code.

Key tokens:

| Token | Purpose |
|---|---|
| `--os-bg-10` | Primary content background |
| `--os-bg-panel` | Sidebar teal background |
| `--os-cyan` | Accent / link colour |
| `--os-green` | H2 heading colour |
| `--os-hot-pink` | Error / inline code accent |
| `--os-amber` | Mild accent / indicators |

---

## Compatibility

- Obsidian **v1.6+** (CM6 editor, CSS variable API)
- Desktop and mobile (no desktop-only features)
- Tested with core plugins: File Explorer, Graph View, Search, Outline, Tags

---

## Attribution

Design system derived from visual reference screenshots and style notes in `style-specs/`. Clean-room CSS implementation.
