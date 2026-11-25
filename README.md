# Buddhist Center Retreat Website

A simple static retreat website starter for a Theravada Buddhist center, built with Astro. Retreat frequency, duration, dates, registration, and practical details in the current copy are examples or planning notes; confirm them before publishing.

## Development

```sh
npm install
npm run dev
```

## Build

```sh
npm run build
npm run preview
```

## GitHub Pages

The `main` branch workflow in `.github/workflows/deploy.yml` builds the site and publishes Astro's `dist/` output. It uses the repository URL `https://arun2k17.github.io/meditation-center/`; configure the repository's Pages source as **GitHub Actions** under Settings → Pages.

Update the sample retreat details, teachers, FAQ, contact details, and donation link before publishing. The website is static and does not include accounts or user data collection.
