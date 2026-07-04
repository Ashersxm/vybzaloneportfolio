# Vybz Alone — Site

Single-page bilingual (FR/EN) portfolio site for Vybz Alone.

## Structure

```
index.html          Main site (HTML/CSS/JS in one file — no build step needed)
robots.txt           Search engine crawl rules
sitemap.xml           Site map for search engines
assets/images/<cat>   Real photos go here, one folder per category
assets/video/         Real video files go here (if hosting your own instead of a CDN)
```

## Before going live — replace these placeholders in `index.html`

- [ ] `hello@vybzalone.com` → your real email
- [ ] `@vybzalone` Instagram link → your real handle
- [ ] `YOUR_FORM_ID` in the form's `action` URL → get one free at formspree.io
- [ ] All `picsum.photos` image URLs → your real photos (upload to `assets/images/...` and update the `src` paths)
- [ ] `https://www.vybzalone.com/` → your real domain, once purchased (appears in meta tags + schema + sitemap.xml)
- [ ] `assets/images/og-cover.jpg` → a real image for social-share previews

## Deploying

**Option A — Netlify or Vercel (recommended, easiest):**
1. Push this repo to GitHub
2. Connect the repo in Netlify/Vercel dashboard
3. Deploy — no build settings needed, it's static HTML
4. Add your custom domain in their dashboard (no CNAME file needed)

**Option B — GitHub Pages:**
1. Push this repo to GitHub
2. Repo Settings → Pages → set source to `main` branch, root folder
3. If using a custom domain, add a `CNAME` file at the repo root containing just your domain (e.g. `vybzalone.com`), and configure DNS at your registrar to point to GitHub Pages

## Local preview

No build tools required — just open `index.html` directly in a browser, or run a simple local server:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`
