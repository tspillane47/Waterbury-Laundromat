# Waterbury Laundromat Website

Static website for [Waterbury Laundromat](https://www.waterburylaundromat.com) — Waterbury, VT.

## 🚀 Deploy to GitHub Pages (free hosting)

### First time setup

1. **Create a GitHub account** at [github.com](https://github.com) if you don't have one
2. **Create a new repository** — click the `+` button → "New repository"
   - Name it: `waterbury-laundromat` (or anything you like)
   - Set it to **Public**
   - Click "Create repository"

3. **Upload your files** — on the new repo page, click "uploading an existing file"
   - Drag the entire `waterbury-laundromat` folder contents in
   - Click "Commit changes"

4. **Enable GitHub Pages**
   - Go to your repo → **Settings** → **Pages** (left sidebar)
   - Under "Source", select **Deploy from a branch**
   - Branch: `main` / folder: `/ (root)`
   - Click **Save**

5. **Your site goes live** at:
   `https://YOUR-USERNAME.github.io/waterbury-laundromat/`
   (takes ~2 minutes to build)

---

## 🗺️ Add Google Maps embed

In `index.html`, find this comment near the bottom:

```
Paste your Google Maps iframe embed here
```

Replace the `<div class="map-box">` block with your iframe from Google Maps:
1. Go to [maps.google.com](https://maps.google.com)
2. Search "5 Park Row Waterbury VT"
3. Click **Share** → **Embed a map** → Copy the `<iframe>` code
4. Paste it in place of the map placeholder

---

## 🌐 Connect your custom domain (waterburylaundromat.com)

1. In GitHub Pages settings, enter your domain in the "Custom domain" field
2. At your domain registrar (where you bought the domain), add these DNS records:

   | Type  | Name | Value |
   |-------|------|-------|
   | A     | @    | 185.199.108.153 |
   | A     | @    | 185.199.109.153 |
   | A     | @    | 185.199.110.153 |
   | A     | @    | 185.199.111.153 |
   | CNAME | www  | YOUR-USERNAME.github.io |

3. Check "Enforce HTTPS" in GitHub Pages settings
4. DNS changes take up to 24 hours to propagate

---

## 📁 File structure

```
waterbury-laundromat/
├── index.html          ← main website (edit this)
├── README.md           ← this file
├── .gitignore
└── images/
    ├── logo-diecut.png       ← die-cut logo (transparent)
    ├── interior-lounge.jpg   ← leather chairs interior
    ├── machines-row.jpg      ← washer row
    ├── machines-wide.png     ← washer wide shot
    ├── mural-wall.jpg        ← blue mural wall
    ├── hours-window.jpg      ← "Everyday 6a-9p" door
    ├── exterior-day.png      ← daytime exterior
    └── exterior-night.webp   ← nighttime exterior
```

## ✏️ Quick edits

All content is in `index.html`. Key things to update:
- **Prices** — search for `$1.70` or `$2–5`
- **Hours** — search for `6:00 am – 9:00 pm`
- **Phone** — search for `802) 391-4447`
- **Reviews** — search for `★★★★★`
- **Google review link** — search for `Leave us a Google review` and update the `href`
