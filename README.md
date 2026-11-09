# Helium no Phantasia

A slate-toned dark theme for [Helium Browser](https://helium.computer), built around muted blues and a line-art New Tab wallpaper.

## Palette

| Element | Color |
|---|---|
| Frame / Tab Strip | `#16181d` — blue-black |
| New Tab Page | `#12151c` — wallpaper-matched field |
| Toolbar / Active Tab / NTP Sections / Omnibox | `#1c1f26` — slate |
| Inactive Tabs | `#23272f` — lighter slate |
| Text | `#edf0f8` — soft white |
| Links | `#58bed5` — soft blue |

## Wallpaper

[`images/ntp-background.png`](images/ntp-background.png) sits behind the New Tab page — white line-art on a `#12151c` field. The `ntp_background` color matches that field, so the image fades into the window edges rather than stopping at a seam. To use your own, replace the file under the same name or point `theme.images.theme_ntp_background` at another one; position and tiling come from `ntp_background_alignment` and `ntp_background_repeat`.

> Chromium draws a theme's New Tab background at its natural pixel size and never scales it, so the image's own dimensions decide how large it appears. Size it near your screen width — anything wider reads as zoomed in and cropped, and 2× width is the right call on HiDPI displays.

## Install

1. Clone or download this repository
2. Visit `chrome://extensions` in Helium
3. Turn on **Developer mode**
4. Choose **Load unpacked** and pick this folder

> If the colors don't change, Helium is showing a cached copy: remove the theme and load it again from `chrome://extensions`. Still stuck? Quit Helium completely and start it fresh.

## Good to know

- Incognito windows keep their own styling — Helium applies the theme to regular windows only. That's a Helium limitation, not something this theme can fix.
- Built as a Manifest V2 theme, since the `theme` key isn't supported under MV3.

## License

No restrictions — use it however you like.
