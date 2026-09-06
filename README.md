# Amrin Kharawala

This repository contains the Astro source for [drkharawala.com](https://drkharawala.com), the professional cardiology and academic portfolio of Amrin Kharawala, MD.

The site preserves the visual system of the [Astro Scholar](https://github.com/whydevils/astro-scholar) template and publishes through GitHub Pages.

## Local development

Install dependencies with `npm ci`.

Run the site with `npm run dev`.

Create a production build with `npm run build`.

## GitHub Pages

The workflow in `.github/workflows/deploy.yml` builds and deploys the site when `main` changes.

In the repository settings, open Pages, select GitHub Actions as the source, and set the custom domain to `drkharawala.com`.

After DNS resolves, enable Enforce HTTPS in the Pages settings.

## Cloudflare DNS

Import `drkharawala.com.zone` from Cloudflare DNS Records, Import and Export.

The file keeps the GitHub Pages records DNS-only so GitHub can issue and renew the HTTPS certificate directly.

Review existing MX, TXT, DKIM, DMARC, and service records before importing because this file contains only the records required for the website.
