# Data Visualisation Style Guide

An Astro application built from the DDL (Data Design Language) style guide.

## Getting started

```bash
npm install
npm run dev
```

Open http://localhost:4321

## Build for production

```bash
npm run build
npm run preview
```

## Deploy

### Netlify / Vercel
Drop the repo in — both platforms auto-detect Astro. No config needed.

### GitHub Pages
Uncomment `base: '/dataviz-style-guide/'` in `astro.config.mjs` and set up the GitHub Actions workflow.

## Structure

```
src/
├── layouts/
│   └── Base.astro              # HTML shell, fonts, meta
├── styles/
│   └── global.css              # CSS variables, base styles, utility classes
├── components/
│   ├── Header.astro            # Guide masthead
│   ├── SideNav.astro           # Sticky nav with active state
│   ├── SectionShell.astro      # Reusable section wrapper
│   └── sections/               # One .astro file per section (00–14)
│       ├── S00_DesignValues.astro
│       ├── S01_ColourPalette.astro
│       └── ...
└── pages/
    └── index.astro             # Composes all sections
```

## Sections

| # | Section |
|---|---------|
| 00 | Design Values |
| 01 | Colour Palette |
| 01b | Tints — Usage Guide |
| 01c | Extended Colour Palette |
| 02 | Accessibility & Contrast |
| 03 | Colour Usage Rules |
| 04 | Chart Examples |
| 05 | Tooltips & Annotations |
| 06 | Typography in Charts |
| 07 | Readability Principles |
| 08 | Chart Type Guidance |
| 09 | Palette Types |
| 10 | Data Uncertainty & Special Values |
| 11 | Responsive Design & Chart Sizing |
| 12 | Interaction & Annotation States |
| 13 | Chart Library by Purpose |
| 14 | Data Storytelling & Narrative |

## Tech

- [Astro](https://astro.build) v4
- Public Sans + DM Mono via Google Fonts
- Zero client-side JS frameworks (plain Astro components)
- Intersection Observer for nav active state
