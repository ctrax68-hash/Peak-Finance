# 🚀 Quick Start — Peak Finance

Get Peak Finance running in 3 minutes.

## For Users: Install the App

### On iPhone
1. Open Safari → go to your deployed Peak Finance URL
2. Tap Share (↗️)
3. Tap "Add to Home Screen"
4. Tap "Add"
5. Launch from home screen — opens fullscreen, no Safari chrome

### On Android
1. Open Chrome → go to your Peak Finance URL
2. Tap Menu (⋮)
3. Tap "Install app" (or "Add to Home Screen")
4. Tap "Install"
5. Launch from home screen — opens fullscreen, no browser chrome

### On Desktop/Browser
Just visit the URL in any modern browser. Works on Mac, Windows, Linux.

---

## For Developers: Deploy Your Own

### Option 1: GitHub Pages (Free)

```bash
# Fork the repo
https://github.com/ctrax68-hash/Peak-Finance

# Enable GitHub Pages in repo settings
# Settings → Pages → Source: main branch
# URL: https://YOUR-USERNAME.github.io/Peak-Finance

# That's it! Live in seconds.
```

### Option 2: Vercel (Free)

```bash
# Deploy with one command
vercel

# Or connect GitHub repo for auto-deploy on push
# https://vercel.com/new
```

### Option 3: Netlify (Free)

```bash
# Drag and drop the folder to Netlify
# https://app.netlify.com/drop

# Or connect GitHub for auto-deploy
```

### Option 4: Manual (Your Own Server)

```bash
# Upload all files to your server root via FTP/SFTP
# Make sure HTTPS is enabled (required for PWA)
# Visit https://YOUR-DOMAIN.com
```

---

## What You Need to Deploy

Copy these files to your server:

```
├── index.html                   ← Main app
├── manifest.json                ← PWA config
├── peak-finance-16x16.png       ← Icons (all 6)
├── peak-finance-32x32.png
├── peak-finance-180x180.png
├── peak-finance-192x192.png
├── peak-finance-512x512.png
├── peak-finance-1024x1024.png
├── README.md                    ← Documentation
├── PWA_SETUP_INSTRUCTIONS.md
├── APP_ICONS_README.md
└── .gitignore                   ← Git config
```

That's it. No build step. No npm install. Just upload and done.

---

## First Steps in the App

1. **Welcome Tutorial** (optional) — Skip or complete the tour
2. **Create a Budget** — Set up your first monthly budget
3. **Add Transactions** — Log your first income or expense
4. **Import Data** — Upload CSV/Excel to bulk import historical data

---

## Customize for Your Brand

Edit these in `index.html`:

```javascript
// Find and update:
- "Peak Finance" → Your app name
- "#0d3322" → Your brand color
- Logo SVG (search for peak-finance SVG)
```

Update `manifest.json`:
```json
{
  "name": "Your App Name",
  "short_name": "Your Name",
  "theme_color": "#your-color"
}
```

---

## Need Help?

- **PWA issues?** → See `PWA_SETUP_INSTRUCTIONS.md`
- **Icon issues?** → See `APP_ICONS_README.md`
- **General?** → See `README.md`

---

**Done!** Your app is now live and installable on all devices. 🎉

Peak Finance — Climb Higher. Spend Smarter. 🏔️
