# animalbar pixel assets

Original ASCII-grid artwork for the animalbar landing page. Regenerate from the
project root with `python3 tools/pixel_assets.py`. Pillow is used if importable;
otherwise the script writes RGBA PNGs using Python's standard library and zlib.
Use `--pure-python` to explicitly exercise that fallback. No external art or fonts.

Every source shape uses integer art pixels. SVGs use art-pixel `viewBox` dimensions,
`shape-rendering="crispEdges"`, and merged horizontal runs. PNG scaling repeats
pixels exactly, with only fully transparent or fully opaque alpha. All individual
assets are transparent; the contact sheet has a pure `#000000` background.

The custom wordmark has 7×11 glyphs (M: 9×11), 1-pixel letter spacing, and a
4-pixel word gap. Its first A has tiny ears. Each glyph's lower two rows are
`#9BE8C9`; the upper rows are `#F4FFF8`. The glyphs remain inside the 11-pixel height.
The apple is an original, unbitten orchard fruit; the windows icon is a generic
framed window. Neither is a platform trademark reproduction. Icons use only
`#FFFFFF`. Color sprites have a `#1a1410` outline and individually limited palettes.

`sparkle-strip.png` contains four 16×16 frames left to right: seed, bloom, flash,
fade. Suggested playback: 100 ms per frame, then hide or repeat; this PNG itself
is a sprite strip, not an animated PNG. The cursor's intended hotspot is `(0, 0)`.
The contact sheet includes all unique artwork at 4×, including every sparkle frame.
The black cursor outline naturally blends into its black background.

For web display, use integer dimensions and `image-rendering: pixelated` on PNGs.
Any soft aquamarine glow should be applied by the site as a separate CSS effect;
the source assets deliberately keep hard, unblurred pixel edges.

## File inventory

Art size is independent of exported PNG size. The generator is
`../../tools/pixel_assets.py` (source code; no art-pixel dimensions).

| File | Art-pixel size | Export size | Format / purpose |
| --- | --- | --- | --- |
| [logo-wordmark.svg](logo-wordmark.svg) | 76 × 11 | Art-pixel viewBox | SVG |
| [logo-wordmark@1x.png](logo-wordmark@1x.png) | 76 × 11 | 76 × 11 px | 1× PNG |
| [logo-wordmark@4x.png](logo-wordmark@4x.png) | 76 × 11 | 304 × 44 px | 4× PNG |
| [icon-apple.svg](icon-apple.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-apple@4x.png](icon-apple@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-windows.svg](icon-windows.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-windows@4x.png](icon-windows@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-download.svg](icon-download.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-download@4x.png](icon-download@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-play.svg](icon-play.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-play@4x.png](icon-play@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-release.svg](icon-release.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-release@4x.png](icon-release@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-keyboard.svg](icon-keyboard.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-keyboard@4x.png](icon-keyboard@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-mouse.svg](icon-mouse.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-mouse@4x.png](icon-mouse@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-egg.svg](icon-egg.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-egg@4x.png](icon-egg@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-book.svg](icon-book.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-book@4x.png](icon-book@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-star.svg](icon-star.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-star@4x.png](icon-star@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-arrow-right.svg](icon-arrow-right.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-arrow-right@4x.png](icon-arrow-right@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-check.svg](icon-check.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-check@4x.png](icon-check@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-warning.svg](icon-warning.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-warning@4x.png](icon-warning@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-folder.svg](icon-folder.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-folder@4x.png](icon-folder@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-zip.svg](icon-zip.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-zip@4x.png](icon-zip@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-shield.svg](icon-shield.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-shield@4x.png](icon-shield@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-sound.svg](icon-sound.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-sound@4x.png](icon-sound@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [icon-gear.svg](icon-gear.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [icon-gear@4x.png](icon-gear@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [acorn.svg](acorn.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [acorn@4x.png](acorn@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [egg.svg](egg.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [egg@4x.png](egg@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [coin.svg](coin.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [coin@4x.png](coin@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [heart.svg](heart.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [heart@4x.png](heart@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [shell.svg](shell.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [shell@4x.png](shell@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [banana.svg](banana.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [banana@4x.png](banana@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [skull.svg](skull.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [skull@4x.png](skull@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [crown-coin.svg](crown-coin.svg) | 16 × 16 | Art-pixel viewBox | SVG |
| [crown-coin@4x.png](crown-coin@4x.png) | 16 × 16 | 64 × 64 px | 4× PNG |
| [sparkle-strip.png](sparkle-strip.png) | 64 × 16 | 64 × 16 px | 1× PNG |
| [cursor.svg](cursor.svg) | 12 × 19 | Art-pixel viewBox | SVG |
| [cursor.png](cursor.png) | 12 × 19 | 12 × 19 px | 1× PNG |
| [preview.png](preview.png) | Artwork at 4× | 1008 × 1000 px | Opaque black contact sheet |
| [README.md](README.md) | N/A | N/A | This inventory |
