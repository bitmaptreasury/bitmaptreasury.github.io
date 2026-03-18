# Bitmap Treasury

**[@bitmaptreasury](https://twitter.com/bitmaptreasury)** — 4,169 Bitcoin-native Bitmap parcels across 57 tranches.

A visual portfolio and treasury dashboard for tracking Bitmap Ordinals holdings on Bitcoin.

## Deploy to GitHub Pages

### 1. Create the repo

Go to [github.com/new](https://github.com/new) and create a new repository:

- **Repository name:** `bitmaptreasury.github.io` (this gives you a clean URL)
- Set to **Public**
- Click **Create repository**

### 2. Push the files

```bash
cd bitmaptreasury
git init
git add .
git commit -m "Bitmap Treasury portfolio"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/bitmaptreasury.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Branch: `main`, folder: `/ (root)`
4. Click **Save**

Your site will be live at: **https://YOUR_USERNAME.github.io** (or **https://bitmaptreasury.github.io** if that's your username)

### 4. Custom domain (optional)

To use a domain like `bitmaptreasury.com`:

1. In repo Settings → Pages → Custom domain, enter your domain
2. Add these DNS records at your registrar:
   - `A` records pointing to GitHub's IPs (185.199.108-111.153)
   - `CNAME` record: `www` → `YOUR_USERNAME.github.io`
3. Check "Enforce HTTPS"

## Updating data

Edit the `RAW` array in `index.html` to add new tranches. Each entry is `{p: PRICE_IN_BTC, q: QUANTITY}`.

## Stack

- Pure HTML/CSS/JS — zero build step
- [Chart.js](https://www.chartjs.org/) via CDN for visualizations
- Google Fonts (Instrument Serif, JetBrains Mono, Outfit)

## License

MIT
