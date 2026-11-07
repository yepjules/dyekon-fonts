# Dyekon fonts

The OFL edition of **Dyekon**, **Dyekon Text**, and **Dyekon Mono**, by Jules / Life Nerds LLC.

Hand-drawn and outlined by Jules Raymond with minor contributions by Beatrice and Arthur Raymond.

This repository distributes the approved Round21b fonts, unchanged, in desktop TTF and web WOFF2 formats.

Current version: **[1.902](https://github.com/yepjules/dyekon-fonts/releases/tag/v1.902)**. See the [changelog](CHANGELOG.md).

## Families

| Family | Styles | Faces |
| --- | --- | ---: |
| Dyekon | Light, Regular, Semibold, Bold, Black; each with an italic. Condensed Light, Condensed Bold, Condensed Black. | 13 |
| Dyekon Text | Regular, Italic, Bold, Bold Italic | 4 |
| Dyekon Mono | Regular, Italic, Bold, Bold Italic | 4 |

Dyekon Text is a distinct reading design; its upright styles use a double-storey **a**.

## Download and install

Download **[Dyekon-OFL-1.902.zip](https://github.com/yepjules/dyekon-fonts/releases/download/v1.902/Dyekon-OFL-1.902.zip)**, then extract the archive. Open the `.ttf` files in [`ttf/`](ttf/) and use your operating system's font installer. Install only the styles you need.

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

The original native rendering checks covered TTF in Chrome on macOS. They do not establish acceptance on every browser, operating system, or display.

## Versioning

[`VERSION`](VERSION) and the `version` field in [`manifest.json`](manifest.json) record the package's font version as a string. Git tags use the same value prefixed with `v`, such as `v1.902`. This follows the existing font version numbering rather than semantic versioning.

Version 1.902 matches the embedded version string in every supplied TTF. Tagged releases preserve their published font files; future font updates receive a new version and tag. Documentation changes may appear on `main` between releases. Use a tagged release when you need a fixed package.

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
