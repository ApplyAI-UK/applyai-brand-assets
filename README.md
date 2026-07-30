# Apply AI — Brand Assets

Logos, fonts, colors, and motion assets for Apply AI. Public repo so assets can be pulled directly into websites (e.g. via jsDelivr) without manual downloads.

## 📁 Structure

```
applyai-brand-assets/
├── logos/
│   ├── svg/              # vector, preferred for web
│   ├── png/               # raster, transparent bg
│   └── favicon/
├── fonts/
│   ├── woff2/              # use these for web
│   └── otf-ttf/             # source files for design tools
├── colors/
│   └── palette.md
├── motion/                  # animated brand assets
└── icons/
```

## 🎨 Colors

| Name | Hex | Usage |
|------|-----|-------|
| Primary | `#______` | e.g. main brand color |
| Secondary | `#______` | |
| Accent | `#______` | |

## 🖼 Logos

- Use `svg/` versions wherever possible — scales cleanly, smaller file size
- Use `png/` only when SVG isn't supported
- Don't stretch, recolor, or rotate the logo outside approved variants
- Minimum clear space: [fill in from brand guidelines]

## 🔤 Fonts

Primary typeface: **[Font Name]**

```css
@font-face {
  font-family: 'BrandFont';
  src: url('https://cdn.jsdelivr.net/gh/YOUR-USERNAME/applyai-brand-assets@main/fonts/woff2/brandfont.woff2') format('woff2');
}
```

## 🔗 Using assets in a live site

All assets in this repo can be pulled directly via jsDelivr (recommended — more reliable content-type handling than raw GitHub URLs):

```
https://cdn.jsdelivr.net/gh/YOUR-USERNAME/applyai-brand-assets@main/<path-to-file>
```

Example:
```html
<img src="https://cdn.jsdelivr.net/gh/YOUR-USERNAME/applyai-brand-assets@main/logos/svg/logo-primary.svg" alt="Apply AI logo">
```

> Note: jsDelivr caches files — if you update an asset, it may take a few hours to refresh unless you version the tag (e.g. `@v1.1` instead of `@main`).

## 📄 License / Usage

Internal brand assets — for use on Apply AI properties only. Not for external redistribution.

Fonts included here are licensed for [describe: web use / internal use / etc.] — confirm license terms before reuse outside this project.
