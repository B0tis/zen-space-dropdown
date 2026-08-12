# Space Dropdown

Compact Spaces dropdown for Zen Browser’s **expanded sidebar**. Turns the crowded Space icon strip into a single current-Space chip that expands into a scrollable vertical list on hover or keyboard focus.

> **Limitation:** Zen Mods are CSS-only. This cannot rebind left-click on the Space name indicator to open a native popup. Switching uses the real Space buttons in the footer strip (and the right-click menu).

## Features

- Collapsed chip showing the active Space (optional name + chevron)
- Hover / `:focus-within` expands a vertical, scrollable Space list
- Space names via `tooltiptext` when enabled
- Matching polish for `#zenWorkspaceMoreActions` (right-click Space list)
- Preferences for max height, names, radius, and active background

## Install (Mods Registry)

1. Open Zen → Mods / Themes marketplace
2. Install **Space Dropdown**
3. Enable it and adjust preferences under Zen Settings → Mods

## Local / development install

1. Open `about:support` → **Profile Directory**
2. Ensure `chrome/zen-themes/<mod-id>/` exists with:
   - `chrome.css`
   - `preferences.json`
3. Register the mod in `zen-themes.json` (folder name must match `id`, and `preferences` must be truthy)
4. Restart Zen, or disable/enable the mod in Settings → Mods

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
