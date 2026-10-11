# NewsDesk — public project landing page

NewsDesk is a news reader with a local server, a native macOS app and a local web interface. It brings articles from news feeds into one overview.

- [Live landing page (Dutch)](https://volnix.io/work/newsdesk)
- [Live landing page (English)](https://volnix.io/en/work/newsdesk)
- [VolNix](https://volnix.io)

## What this repository contains

This is the source snapshot for the public NewsDesk landing page, not the operational application. `index.html` and `en/index.html` use reviewed public assets hosted on volnix.io. The project-specific stylesheet and vector mark are included under `assets/` for reference.

The application, integrations, account configuration and operational data remain private. No Twitter/X credentials or integration code are included here. This repository is not an installer or a hosted news dashboard.

## Local preview

Run `python3 -m http.server 8080` from this directory, then open the local server in a browser. The pages load shared branding and navigation from the public VolNix site. No environment variables, API keys or account connections are required.

## Maintenance

The live pages are deployed through the VolNix website workflow. Update this reviewed snapshot only from approved public landing-page files. Do not copy files from the operational application into this repository.
