# BioGrow standalone deployment

This repository contains the self-contained BioGrow app in `site.tar.gz`. The archive includes the HTML, JavaScript, styles, tomato image, phone frame, local fonts, and font license files.

## Render settings

- Service type: Static Site
- Branch: `main`
- Build command: `mkdir -p public && tar -xzf site.tar.gz -C public`
- Publish directory: `public`
- No runtime secrets, backend, OpenAI service, or external font requests are required.

Archive SHA-256: `d72ec1b76b2a5c1cee5d8442d467bea0da9170370e7729be6f8e72fac0991097`.

To update the app, rebuild this archive from the app files and trigger a Render deployment. The archive paths are relative to the site's document root.

This is a prototype: soil readings and box pairing are simulated. Plant records are stored in each browser, so a new hostname starts a separate garden. Availability in a specific country or network must be verified from that location.
