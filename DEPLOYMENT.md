# BioGrow standalone deployment

Live site: https://jonathancheung718-lang.github.io/biogrow-garden/

## GitHub Pages

The site is published by `.github/workflows/publish.yml` from the `main` branch. The workflow verifies and extracts `site.tar.gz`, then publishes the resulting `public` directory. It runs when the archive or publishing workflow changes, and it can also be run manually. The archive includes the app's HTML, JavaScript, styles, tomato image, silver phone frame, local fonts, and font license files.

No ChatGPT account, OpenAI service, backend, runtime secrets, or external font requests are required. HTTPS is enabled by GitHub Pages.

Archive SHA-256: `d72ec1b76b2a5c1cee5d8442d467bea0da9170370e7729be6f8e72fac0991097`.

To update the app, rebuild the archive from its app files, update the expected checksum in the workflow, and commit both changes. Archive paths must be relative to the site's document root.

## Optional Render deployment

Render creation was not completed because the account requires payment information. No Render service was created. A future static-site deployment can use:

- Branch: `main`
- Build command: `mkdir -p public && tar -xzf site.tar.gz -C public`
- Publish directory: `public`

## Prototype and access notes

Soil readings and box pairing are simulated. Plant records are stored in each browser, so a new hostname starts a separate garden. Availability in a specific country or network must be verified from that location. The live site has been tested without login in a fresh browser session; access from Hong Kong and mainland China has not been independently verified.
