# Or Levi · Portfolio

My personal site: one static page, no build step. A dark stage in mint and forest green, set in
Sora and Plus Jakarta Sans.

## Files

- `index.html` holds all the markup, styles and script.
- `og-image.jpg` is the 1200×630 preview shown when the link is shared.
- `favicon.svg` is the tab icon.
- `assets/or-cutout.webp` is the hero portrait with its background removed.
- `assets/or.jpg` is a square crop of the same photo, used in the assistant's header.
- `assets/family-me-film.mp4` and `assets/family-me-fan.webp` are a short silent cut of the
  Family Me launch film and its poster frame.

## Preview

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy on Vercel

Import this repository in Vercel and keep the defaults: framework preset "Other", no build
command, output directory `.` (the repository root). Every push to `main` redeploys.

Once the domain is known, make the share image absolute in `index.html`, because LinkedIn and
most crawlers ignore a relative one:

```html
<meta property="og:image" content="https://your-domain/og-image.jpg" />
```
