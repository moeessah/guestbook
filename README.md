# guestbook

Repo root doubles as a small portfolio page (`index.html`) with three link-outs to `v1/`, `v2/`, `v3/` — three design directions for the same site, all sharing one set of images from the folders below.

## Structure

```
guestbook/
├── index.html          portfolio landing page (links to v1/v2/v3)
├── favicon.svg
├── v1/  v2/  v3/        each: index.html, host.html, explore.html
└── shared image folders (used by all three versions via ../ paths)
    ├── hero/
    ├── activity/
    ├── destination/
    ├── listings/
    ├── review pics/
    ├── review icons/
    ├── Collections/
    └── journal/
```

## Before pushing

The shared image folders above are currently empty (just a `.gitkeep` placeholder). Copy your actual images into them at the **repo root**, keeping the same filenames the HTML already expects (e.g. `hero/8.webp`, `listings/1.webp`, `review icons/1.webp`). Every `v1`, `v2`, and `v3` page already points at `../<folder>/<file>`, so once the images land in these root folders, all three versions will pick them up automatically — nothing else to edit.

## Publishing

1. Push this folder as the repo `guestbook` under your GitHub account.
2. Enable GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).
3. Site goes live at `https://moeessah.github.io/guestbook/`:
   - Landing page: `https://moeessah.github.io/guestbook/`
   - Version 1: `https://moeessah.github.io/guestbook/v1/`
   - Version 2: `https://moeessah.github.io/guestbook/v2/`
   - Version 3: `https://moeessah.github.io/guestbook/v3/`

All internal links (nav, version switcher, image paths) are relative, so this works as-is once pushed — no URLs to hardcode.
