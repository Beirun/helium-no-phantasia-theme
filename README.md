# Helium no Phantasia

A minimal dark theme for [Helium Browser](https://helium.computer). Soft slate blues — no eye-searing purple, no compromises.

## Preview

| Element | Color |
|---|---|
| Frame / Tab Strip | `#16181d` — blue-black |
| New Tab Page | `#12151c` — wallpaper-matched field |
| Toolbar / Active Tab / NTP Sections / Omnibox | `#1c1f26` — slate |
| Inactive Tabs | `#23272f` — lighter slate |
| Text | `#edf0f8` — soft white |
| Links | `#58bed5` — soft blue |

New Tab wallpaper: [`images/ntp-background.png`](images/ntp-background.png) — white line-art on a `#12151c` field. The `ntp_background` color is matched to that field so the wallpaper blends into the window edges. Swap in your own PNG using the same filename, or point `theme.images.theme_ntp_background` at a different file. Alignment and tiling are set via `ntp_background_alignment` and `ntp_background_repeat`.

> Sizing: Chromium renders a theme's New Tab background at its natural pixel size — it does not scale to fit. The wallpaper is therefore exported at 1920px wide to match a 1080p screen 1:1; a larger image looks zoomed in and cropped. On a HiDPI display, export at 2× (3840px wide).

## Installation

1. Download or clone this repo
2. Open `chrome://extensions` in Helium
3. Enable **Developer mode** (top-right toggle)
4. Click **Load unpacked** → select this folder
5. Done

> Heads up: Helium doesn't always apply theme changes on extension refresh. If colors aren't updating, remove the theme and re-add it via Load unpacked. If it still won't load, fully quit and relaunch Helium first.

## Notes

- Incognito windows are not affected — this is a Helium limitation, not a theme issue.
- Built on Manifest V2 — Chrome's theme API does not support the `theme` key in MV3.

## License

Do whatever you want with it.
