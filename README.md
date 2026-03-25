# xihale intro

Standalone Astro + Bun navigation site for xihale's projects, websites, packages, and selected contribution trails.

## Local development

```bash
bun install
bun dev
```

## Build

```bash
bun run build
```

## GitHub Pages

This project is configured for GitHub Pages with a custom domain:

- site URL: `https://intro.xihale.top`
- custom domain file: `public/CNAME`
- workflow: `.github/workflows/deploy.yml`

Assumptions:

- the repository will be deployed with GitHub Pages Actions
- the Pages source is set to GitHub Actions in repository settings
- DNS for `intro.xihale.top` points to GitHub Pages

Because this setup targets a custom domain root, `astro.config.mjs` uses `site` only and does not set `base`. If you later deploy under a repo path like `https://xihale.github.io/<repo>/`, add a matching `base` value.
