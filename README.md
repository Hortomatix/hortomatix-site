# hortomatix.com.au

The Hortomatix company website — single-page static site.

## Structure

```
hortomatix-site/
├── index.html                  Main and only page
├── netlify.toml                Netlify config (headers, caching)
├── robots.txt                  SEO basics
├── sitemap.xml                 SEO basics
├── README.md                   This file
└── assets/
    └── logos/                  SVG logo files
        ├── icon-white.svg
        ├── wordmark-horizontal-green.svg
        ├── wordmark-horizontal-white.svg
        └── wordmark-tagline-horizontal-white.svg
```

## Local preview

Open `index.html` in a browser, or run a local server:
```
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Pushed via Netlify drag-and-drop or git-based continuous deploy.

## Known issues / future work

- The logo SVGs are PNG-embedded inside SVG wrappers (~400KB each).
  Replace with true vector versions when available for substantial weight savings.
- No analytics installed. Add Plausible or Fathom when ready.
- No contact form — currently mailto: link only. Add Netlify Forms or
  Formspree when traffic justifies it.

## Fonts

Loaded from Google Fonts:
- Manrope (body)
- JetBrains Mono (technical accents)

## Colours

Defined as CSS custom properties at the top of `index.html`.
Brand green: `#00e87a` (display version of `#00742e` from the logo).
