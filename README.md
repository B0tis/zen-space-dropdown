# Space Dropdown

Compact Spaces dropdown for Zen Browser’s **expanded sidebar**. Turns the crowded Space icon strip into a single current-Space chip that expands into a readable list on hover or keyboard focus.

> **Limitation:** Zen Mods are CSS-only. This cannot rebind left-click on the Space name indicator to open a native popup. Switching uses the real Space buttons in the footer strip (and the right-click menu).

## Features

- Collapsed chip showing the active Space (optional name + chevron)
- Hover / `:focus-within` expands a vertical Space list that grows with the list (capped at ~80vh)
- Past that cap, extra columns wrap instead of a tall scrollport, so Zen's hover auto-scroll cannot jump
- Space names via `tooltiptext` when enabled
- Matching polish for `#zenWorkspaceMoreActions` (right-click Space list)
- Preferences for names, radius, and active background

## Install (Windows)

Zen’s **Mods → Import** only installs mods that exist in the **official store**. It ignores the asset URLs in a local JSON file and looks up the mod ID online — so custom mods like this one cannot be imported that way.

Use the installer instead:

```powershell
cd path\to\zen-space-dropdown
powershell -ExecutionPolicy Bypass -File .\install.ps1
```

Then restart Zen, or open **Settings → Mods** and toggle **Space Dropdown** off/on.

### Manual install

1. Open `about:support` → **Profile Directory**
2. Copy files into `chrome/zen-themes/a1c8e4f2-9b3d-4e7a-8f1c-2d6b5a9e0c44/`:
   - `chrome.css`
   - `preferences.json`
3. Add the mod entry from `space-dropdown.zen.json` into `zen-themes.json` (folder name must match `id`)
4. Restart Zen, or disable/enable the mod in Settings → Mods

## Preferences

| Preference | Type | Default | Purpose |
|---|---|---|---|
| `mod.space-dropdown.enabled` | checkbox | `true` | Master toggle |
| `mod.space-dropdown.show_names` | checkbox | `true` | Show Space names |
| `mod.space-dropdown.chip_radius` | string | `8px` | Corner radius |
| `mod.space-dropdown.active_bg` | string | Accent mix | Active Space background |

## Usage

1. Use Zen with an **expanded sidebar** (not single-toolbar).
2. Look at the Space strip in the sidebar footer — it should show one chip.
3. Hover (or Tab-focus) the chip to expand the full Space list; click a row to switch.
4. Right-click the Space indicator / switcher for the native manage menu (also restyled).

## License

MIT



