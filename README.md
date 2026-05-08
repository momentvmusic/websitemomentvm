# Momentvm Music — Marketing Website

Static single-file website for the Momentvm Music label.

## Stack

- Plain HTML/CSS/JS (no framework, no build step)
- All images embedded as base64 → single portable file
- Liquid glass design (Apple-style) with orange gradient accents

## Sections

1. Hero (with abstract orange bg + animated laser lines)
2. About (3 pillars: Sound · Energy · Moments)
3. Artists (Sevenkey, 2 Nomads, Joe Diem)
4. Catalog (Falling Into You — Sevenkey, MMVM 001)
5. Send your demos
6. Spotify Playlists (Best Afro House, Running Summer, Gym Music)
7. Footer

## Deploy to Netlify

### Option A — Drag & drop (fastest, 30 seconds)
Go to [app.netlify.com/drop](https://app.netlify.com/drop) and drag the entire folder. Done.

### Option B — GitHub → Netlify (auto-deploy on push)
1. Push this repo to GitHub
2. In Netlify: New site → Import from Git → select repo
3. **Leave build command EMPTY** — there's nothing to build
4. **Publish directory:** `.` (just a dot, the root)
5. Deploy

Every push to main triggers a redeploy automatically.

## Editing the site

The entire site lives in `index.html`. Look for these comments to find sections to edit:
- Catalog releases: `▼▼▼ AÑADIR NUEVOS RELEASES AQUÍ ▼▼▼`
- Artists, Playlists: same pattern, duplicate the existing card blocks

## Why no Vite / React / build step?

Because adding them would only add complexity (build pipeline, dependencies, dev server, deploy time) with zero benefit:
- No client-side routing needed
- No state management
- No API calls
- All assets are already inlined in the HTML

If we ever need a CMS, user accounts, or dynamic content, a real framework will make sense. Until then, plain HTML is faster, simpler, and more maintainable.

---

© Momentvm Music · MMXXVI
