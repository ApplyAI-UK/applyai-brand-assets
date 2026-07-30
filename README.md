# Apply AI — Brand Assets

Logos and fonts for Apply AI. Public repo so assets can be pulled directly into live sites (e.g. via jsDelivr) without manual downloads.

## 📁 Structure

```
applyai-brand-assets/
├── LICENSE
├── README.md
├── APPLY AI FONT/
│   ├── EULA.pdf                          # font license — check before external reuse
│   ├── Albra Book Medium/
│   │   ├── OTF/                          # source, for design tools
│   │   └── WEB/                          # .woff / .woff2 — use these for web
│   ├── Albra Book Regular/
│   ├── Albra Display Light/
│   ├── Albra Grotesk Light/
│   └── Albra Grotesk Medium/
└── APPLY AI LOGO/
    ├── Digital/                          # RGB — use for web/screen
    │   ├── 1 Logo Lockup/
    │   │   ├── AI/                       # Illustrator source
    │   │   ├── PNG/High Res | Low Res/
    │   │   └── SVG/                      # preferred for web
    │   └── 2 Symbol/                     # same structure, icon-only mark
    └── Print/                            # CMYK — for print use only
        ├── 1 Logo Lockup/ (AI / EPS / PDF)
        └── 2 Symbol/ (AI / EPS / PDF)
```

Each logo folder has three color variants: **Black**, **Orange**, **White**.

## 🔤 Fonts

Typeface family: **Albra** (Book, Display, Grotesk — in Medium/Regular/Light weights)

Font license: see `APPLY AI FONT/EULA.pdf`. Confirm redistribution terms before using outside Apply AI properties.

```css
@font-face {
  font-family: 'Albra Book Medium';
  src: url('https://cdn.jsdelivr.net/gh/ApplyAI-UK/applyai-brand-assets@main/APPLY%20AI%20FONT/Albra%20Book%20Medium/WEB/RL-Albra-Book-Medium.woff2') format('woff2'),
       url('https://cdn.jsdelivr.net/gh/ApplyAI-UK/applyai-brand-assets@main/APPLY%20AI%20FONT/Albra%20Book%20Medium/WEB/RL-Albra-Book-Medium.woff') format('woff');
}
body {
  font-family: 'Albra Book Medium', sans-serif;
}
```

## 🖼 Logos

- Use **Digital → SVG** for web wherever possible — scales cleanly, smallest file size
- Use **Digital → PNG (High Res)** only when SVG isn't supported
- Use **Print** versions (CMYK) only for physical/print materials, never on web
- Don't stretch, recolor, or rotate the logo outside the provided Black/Orange/White variants

Example:
```html
<img src="https://cdn.jsdelivr.net/gh/ApplyAI-UK/applyai-brand-assets@main/APPLY%20AI%20LOGO/Digital/1%20Logo%20Lockup/SVG/ApplyAI_Lockup_Black_RGB.svg" alt="Apply AI logo">
```

## 🔗 Using assets in a live site

All assets can be pulled directly via jsDelivr (recommended over raw GitHub URLs — more reliable content-type handling, especially for fonts):

```
https://cdn.jsdelivr.net/gh/ApplyAI-UK/applyai-brand-assets@main/<path-to-file>
```

Folder/file names contain spaces, which must be URL-encoded as `%20` in the path (see examples above).

> jsDelivr caches files — if you update an asset, it may take a few hours to refresh unless you version the tag (e.g. `@v1.1` instead of `@main`).

## 📄 License

See [`LICENSE`](./LICENSE) — all rights reserved, Apply AI. Third-party fonts remain subject to the terms in `APPLY AI FONT/EULA.pdf`.
