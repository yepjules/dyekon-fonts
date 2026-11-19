# Dyekon fonts

The OFL edition of **Dyekon**, **Dyekon Text**, and **Dyekon Mono**, by Jules / Life Nerds LLC.

Hand-drawn and outlined by Jules Raymond with minor contributions by Beatrice and Arthur Raymond.

This repository distributes the approved Round 23 designs as desktop TTF and web WOFF2 files. Dyekon and Dyekon Text include the revised lowercase **m** and combining-accent placement. Dyekon Mono is the approved four-face Mono 23.

The current package is **v23**. Every font retains its embedded OpenType version of **1.902**. [Release](https://github.com/yepjules/dyekon-fonts/releases/tag/v23) · [Changelog](CHANGELOG.md)

## Families

| Family | Styles | Faces |
| --- | --- | ---: |
| Dyekon | Light, Regular, Semibold, Bold, Black; each with an italic. Condensed Light, Condensed Bold, Condensed Black. | 13 |
| Dyekon Text | Regular, Italic, Bold, Bold Italic | 4 |
| Dyekon Mono | Regular, Italic, Bold, Bold Italic | 4 |

Dyekon Text is a distinct reading design; its upright styles use a double-storey **a**.

## Download and install

Download and extract **[Dyekon-OFL-23.zip](https://github.com/yepjules/dyekon-fonts/releases/download/v23/Dyekon-OFL-23.zip)**. Open the `.ttf` files in [`ttf/`](ttf/) and use your operating system's font installer. Install only the styles you need.

## Use on the web

Copy [`fonts.css`](fonts.css) and the [`woff2/`](woff2/) directory into the same folder on your site. Load the stylesheet:

```html
<link rel="stylesheet" href="/fonts/dyekon/fonts.css">
```

```css
body {
  font-family: 'Dyekon Text', sans-serif;
}

h1, h2, h3 {
  font-family: 'Dyekon', sans-serif;
}

code, pre {
  font-family: 'Dyekon Mono', monospace;
}

.condensed {
  font-family: 'Dyekon', sans-serif;
  font-weight: 700;
  font-stretch: condensed;
}
```

These are static fonts. Request an available weight, style, and stretch from the table above.

## Rendering notes

Check your intended text at its final display size. Fine strokes, dense accents, and stacked combining marks can lose detail at small sizes. Dyekon Mono has no automatic `fi` or `fl` ligature substitution.

Round 23 preserves the existing line metrics. Tall and deep accent stacks can extend beyond them and may clip in a fixed-height text box. Test stacked accents with the line height you intend to use.

The original native rendering checks covered TTF in Chrome on macOS. They do not establish acceptance on every browser, operating system, or display.

## Versioning

The package version identifies the approved design round. Git tags prefix that value with `v`, as in `v23`. The manifest records the embedded font version separately. [Package version](VERSION) · [Manifest](manifest.json)

The earlier Round 21b package is archived under its original tag, `v1.902`. Use a tagged release when you need a fixed package. [Round 21b release](https://github.com/yepjules/dyekon-fonts/releases/tag/v1.902)

## Package integrity

[`manifest.json`](manifest.json) lists SHA-256 hashes for all 42 font files. The exported font bytes and embedded version numbers are unchanged from the approved delivery. This is a distribution repository for compiled fonts; editable sources and build tooling are not included.

On macOS or a system with `shasum`, verify the package from its root:

```sh
shasum -a 256 -c SHA256SUMS
```

## License

Copyright © 2026 Life Nerds LLC.

The fonts are licensed under the **SIL Open Font License, Version 1.1**. See [`OFL.txt`](OFL.txt) for the complete license. The accompanying CSS and documentation in this distribution are provided under the same license.

The separately licensed Dyekon colour families, SPC fonts, and ACT are outside this repository.
