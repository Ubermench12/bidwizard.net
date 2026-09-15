# Bid Wizard website

A single-page site for Bid Wizard — proposal development for small civil, environmental, and geospatial firms entering federal and SLED contracting.

## What's in here

```
index.html            the whole site (HTML + CSS + a few lines of JS)
assets/logo-full.png  full logo lockup (crest + wordmark + tagline), transparent background
assets/logo-mark.png  crest only, no text — used in the header and hero
assets/favicon.png    browser-tab icon, generated from the crest
```

There's no build step. It's plain HTML/CSS, so there's nothing to install or compile.

## Publish it with GitHub Pages (free)

1. Create a new repository on GitHub — e.g. `bidwizard-site`. Public repos get free Pages hosting.
2. Upload all the files in this folder to the repository, **keeping the `assets/` folder structure intact** (index.html at the root, the three images inside an `assets` folder next to it).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment," set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. GitHub will give you a URL like `https://yourusername.github.io/bidwizard-site/` — it usually goes live within a minute or two.

## Before you go live, replace these placeholders

- **Email address** — the site currently points to `hello@bidwizard.com` in two places (search for it in `index.html`). Swap it for whatever address you set up through IONOS.
- **Custom domain (optional)** — if you point a real domain (e.g. `bidwizard.com`) at this repo instead of using the github.io URL, add a file named `CNAME` (no extension) at the root containing just your domain name, and set that domain up in the same Settings → Pages screen.

## If you want to change something later

- Everything is in `index.html` — text, colors, and layout all live in that one file, with the CSS at the top in a `<style>` block and the page content below it.
- The color palette is defined once, near the top of the `<style>` block, as CSS variables (`--navy`, `--gold`, `--paper`, etc.) — changing a value there updates it everywhere on the page.
- To swap the logo, replace the PNG files in `assets/` with new ones of the same filename, or update the `src=` paths in `index.html` if you rename them.
