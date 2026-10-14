# Neon Amber Glass

A dark glass theme with warm yellow text and glowing orange, green and ice-blue accents. Readable terminal typography, without flicker or animated effects.

![Default palette and navigation preview](preview.svg)

## Features

- Soft yellow body text. Glow is reserved for headings, titles and file names.
- Orange H1/H4, green H2/H5 and ice-blue H3/H6 headings.
- Navigation colors follow folder depth by default. Every item at the same level gets the same color, across different folders. The three colors repeat at deeper levels.
- Optional alternating colors for individual navigation entries.
- Adjustable background transparency, tint saturation, glow, line height and readable width.
- Tint strength changes chroma at a constant perceptual lightness.
- Fully transparent background surfaces at 100%, including the extra note shading. Text remains opaque.
- Color-picker swatches show the actual selected colors.
- Optional static scanlines, an opaque reading mode, reduced-transparency support and a clean print layout.

The preview illustrates the default palette with synthetic demo content. It contains no personal vault data.

## Install

The community-directory submission is pending. Until the theme is listed, download `manifest.json` and `theme.css` from the [latest release](https://github.com/khedrub/neon-amber-glass/releases/latest), put both files in `<vault>/.obsidian/themes/Neon Amber Glass/`, and select **Neon Amber Glass** in **Settings → Appearance**.

Install and enable [Style Settings](https://github.com/community-archive/obsidian-style-settings) to use the controls in **Settings → Style Settings → Neon Amber Glass**. Without it, the theme uses the same defaults, including navigation colors by depth.

The settings have German labels. **Navigation nach Ebene färben** controls depth-based navigation colors and is enabled by default. Turn it off for the alternating-entry palette.

Local fonts only: Monaco, Menlo, JetBrains Mono, Consolas or the system monospace fallback. Your Obsidian font preferences take precedence. No font downloads or bundled proprietary fonts.

## Glass and native transparency

CSS transparency applies to background surfaces, not to the entire window. Native desktop transparency requires a supported desktop platform and a window created with transparency enabled. On macOS, enable Obsidian's **Translucent window** setting.

The optional [Neon Amber Glass Companion](https://github.com/khedrub/neon-amber-glass-companion) selects clear, frosted or dark HUD window material on macOS. **Fensterglas** is the corresponding Style Settings control.

Some Obsidian/Electron installations create an opaque window even when translucency is enabled. A theme or a material switch cannot repair that window-creation flag. True desktop sampling is conditional on a transparent window. Neither this theme nor the companion modifies Obsidian application files or applies a startup patch.

**Blur hinter Popups** controls CSS blur behind in-app menus and popups. macOS controls the strength of native desktop blur; it is not a continuous pixel slider.

On unsupported platforms, the theme keeps its dark appearance. Transparent backgrounds over bright content can reduce contrast; use extra note shading or **Blickdichter Lesemodus** for an opaque reading surface.

## Compatibility

Tested with Obsidian 1.14.4 on macOS using installer 1.13.7. The theme uses modern Chromium CSS, including relative OKLCH colors, `color-mix()` and `mod()`. Use installer 1.13.7 or newer; updating only the Obsidian app package may leave an older Chromium renderer in place.

Dark mode is the supported visual mode. The theme remains dark when selected under a light system appearance.

No network assets, telemetry or note access.

## License

[MIT](LICENSE), © 2026 khedrub.
