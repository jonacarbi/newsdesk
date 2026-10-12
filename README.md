# NewsDesk — landing page

**Live:** [newsdesk-app.netlify.app](https://newsdesk-app.netlify.app/) · [English](https://newsdesk-app.netlify.app/en/)

NewsDesk is a private news reader built by [VolNix](https://volnix.io). It collects headlines from RSS feeds, Google News, Reddit and Hacker News across six categories (tech, crypto, finance, sport, entertainment and politics). It then clusters differently worded headlines about the same story, so one story shows every outlet reporting it. It runs as a native macOS SwiftUI app with an in-app reader, alongside a browser dashboard, and includes a studio for drafting copy-ready posts per story.

## What this repository contains

The source of the public landing page only — not the application.

```
index.html          Dutch landing page (default)
en/index.html       English landing page
assets/newsdesk.css Styles: newsprint palette, night-edition dark mode
assets/favicon.svg  NEWS/DESK mark from the app icon
netlify.toml        Security headers and caching
```

The site is fully static: no JavaScript, no build step, no external fonts or requests. The interface visuals are illustrative HTML/CSS recreations with invented headlines, not screenshots.

The application, its integrations, account configuration and data stay private. There is no download, installer or hosted dashboard.

## Local preview

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080/` (Dutch) or `/en/` (English).

## Deploy

The site is a standalone Netlify project (`newsdesk-app`). It publishes this directory as-is:

```bash
netlify deploy --prod --dir . --site newsdesk-app
```

## Brand

| Token | Value |
|---|---|
| Paper | `#f7f2e6` → `#e9e1cf` |
| Ink | `#141414` |
| Accent | `#b3261e` (DESK, active states) |
| Display | New York / Iowan Old Style / Palatino / Georgia, bold |
| Meta | system-ui |

## Maintenance

Only reviewed, public landing-page files belong here. Never copy code, configuration or data from the operational application into this repository.
