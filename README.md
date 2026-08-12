# Space Dropdown

Compact Spaces dropdown for Zen Browser’s **expanded sidebar**. Turns the crowded Space icon strip into a single current-Space chip that expands into a scrollable vertical list on hover or keyboard focus.

> **Limitation:** Zen Mods are CSS-only. This cannot rebind left-click on the Space name indicator to open a native popup. Switching uses the real Space buttons in the footer strip (and the right-click menu).

## Features

- Collapsed chip showing the active Space (optional name + chevron)
- Hover / `:focus-within` expands a vertical, scrollable Space list
- Space names via `tooltiptext` when enabled
- Matching polish for `#zenWorkspaceMoreActions` (right-click Space list)
- Preferences for max height, names, radius, and active background

## Install

### Import (recommended)

1. Download [`space-dropdown.zen.json`](https://github.com/B0tis/zen-space-dropdown/blob/master/space-dropdown.zen.json)
2. Open Zen → Settings → Mods
3. Use **Import** and select the JSON file
4. Enable **Space Dropdown** and adjust preferences

### Local / development install

1. Open `about:support` → **Profile Directory**
2. Copy files into `chrome/zen-themes/a1c8e4f2-9b3d-4e7a-8f1c-2d6b5a9e0c44/`:
   - `chrome.css`
   - `preferences.json`
3. Register the mod in `zen-themes.json` (folder name must match `id`, and `preferences` must be truthy)
4. Restart Zen, or disable/enable the mod in Settings → Mods

> The official Mods Registry / theme-store is currently archived. This mod is distributed from GitHub until submissions reopen.

## Preferences

| Preference | Type | Default | Purpose |
|---|---|---|---|
| `mod.space-dropdown.enabled` | checkbox | `true` | Master toggle |
| `mod.space-dropdown.max_height` | string | `240px` | Max height of expanded list |
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

