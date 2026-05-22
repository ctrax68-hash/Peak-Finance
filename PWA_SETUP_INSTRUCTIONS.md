# Peak Finance PWA Setup Guide

## What You Got

✅ App icons in 6 sizes (16, 32, 180, 192, 512, 1024px)
✅ PWA manifest.json ready to use
✅ All iOS & Android home screen sizes covered

---

## Step 1: Add to Your HTML `<head>` Section

Copy these lines into your main HTML file (after the existing meta tags):

```html
<!-- PWA Manifest -->
<link rel="manifest" href="/manifest.json">

<!-- Favicon -->
<link rel="icon" type="image/png" sizes="32x32" href="/peak-finance-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/peak-finance-16x16.png">

<!-- iOS Home Screen Icon (without rounded corners applied by browser) -->
<link rel="apple-touch-icon" href="/peak-finance-180x180.png">

<!-- Theme Color -->
<meta name="theme-color" content="#0d3322">

<!-- Apple Status Bar -->
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
```

---

## Step 2: File Structure in Your Repo

Place all files in your public/root directory:

```
/
├── index.html (your main app)
├── manifest.json
├── peak-finance-16x16.png
├── peak-finance-32x32.png
├── peak-finance-180x180.png
├── peak-finance-192x192.png
├── peak-finance-512x512.png
└── peak-finance-1024x1024.png
```

---

## Step 3: iOS Home Screen Install

1. Open your app in Safari on iPhone
2. Tap Share → Add to Home Screen
3. Icon appears with the green peak mark + gold ring

---

## Step 4: Android Home Screen Install

1. Open your app in Chrome on Android
2. Menu (⋮) → Install app / Add to Home Screen
3. Icon appears at 192x192 + 512x512 sizes

---

## Icon Specs

| Size | Use | Purpose |
|------|-----|---------|
| 16×16 | Favicon | Browser tab |
| 32×32 | Favicon | Bookmark bar, retina displays |
| 180×180 | iOS | iPhone home screen (all retina) |
| 192×192 | Android | Android home screen, maskable |
| 512×512 | PWA | Web app store, splash screens |
| 1024×1024 | Store | App store listings, promotional |

---

## Design System

- **Background**: Dark green radial gradient (#1f6b3e → #050f09)
- **Peak Mark**: Mint-to-forest green gradient with 3D lighting (left highlight, right shadow)
- **Tip Star**: Ecru sparkle with white center
- **Border**: Gold conic ring (#c9a84c → #fef3c7 → #c9a84c)
- **Shine**: Glass overlay on upper third

All sizes are consistent — same design, just scaled. No pixelation, crisp anti-aliased edges.

---

## Testing

### macOS / iOS Simulator
```bash
# In your project root, serve locally:
python3 -m http.server 8000
# Visit: http://localhost:8000
# Inspect > PWA tab in DevTools
```

### Real Device (iOS)
1. Safari → Visit your app URL
2. Share → Add to Home Screen
3. Verify icon appears with correct colors

### Real Device (Android)
1. Chrome → Visit your app URL
2. Menu → Install App
3. Verify icon appears at correct size with no distortion

---

## Next Steps

If you want to customize further:
- Edit `manifest.json` to add more shortcuts, screenshots, or categories
- Update theme colors in both manifest and HTML `<meta>` tags
- For maskable icons, ensure your design works well when rounded by the OS

Your app is now installable on phones as a native-feeling PWA! 🏔️

