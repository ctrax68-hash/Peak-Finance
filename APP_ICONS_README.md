# 🏔️ Peak Finance App Icons & PWA Assets

Complete icon set for installing Peak Finance as a native app on iOS and Android phones.

## 📦 What's Included

### App Icons (6 Sizes)
All icons feature the **Peak Finance visual identity**:
- Dark green radial gradient background (#1f6b3e → #050f09)
- Bright green mountain peak with 3D lighting (left highlight + right shadow)
- Mint tip star with white dot
- Gold conic ring border with shimmer effect
- Glass shine overlay

```
peak-finance-16x16.png       [552 bytes]   → Favicon (browser tab)
peak-finance-32x32.png       [1.2 KB]      → Favicon (bookmark, retina)
peak-finance-180x180.png     [9.2 KB]      → iOS home screen
peak-finance-192x192.png     [10 KB]       → Android home screen (maskable)
peak-finance-512x512.png     [32 KB]       → PWA app store
peak-finance-1024x1024.png   [72 KB]       → Store assets, promo
```

### Configuration Files
- **manifest.json** — PWA manifest with all icon references, shortcuts, and metadata
- **PWA_SETUP_INSTRUCTIONS.md** — Step-by-step integration guide

---

## 🚀 Quick Start

1. **Copy all files to your project root** (or `/public` directory)
2. **Add these lines to your HTML `<head>`:**

```html
<link rel="manifest" href="/manifest.json">
<link rel="icon" type="image/png" sizes="32x32" href="/peak-finance-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/peak-finance-16x16.png">
<link rel="apple-touch-icon" href="/peak-finance-180x180.png">
<meta name="theme-color" content="#0d3322">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
```

3. **Deploy to your server**

4. **On iPhone**: Safari → Share → Add to Home Screen
   **On Android**: Chrome → Menu → Install App

---

## 🎨 Design Details

### Color Palette
| Element | Color | Hex |
|---------|-------|-----|
| Background (light) | Dark Green | #1f6b3e |
| Background (dark) | Forest | #050f09 |
| Peak (top) | Mint | #d4fae8 |
| Peak (mid) | Bright Green | #4ade80 |
| Peak (base) | Forest | #0d5c2c |
| Border Ring | Gold | #c9a84c – #fef3c7 |
| Tip Star | Ecru | #ecfdf5 |
| Glass Shine | White | rgba(255,255,255,0.12) |

### Specs by Size

**16×16 & 32×32**
- Favicon for browser tabs and bookmarks
- Simplified geometry, no anti-alias artifacts
- Works at 1x and 2x (retina)

**180×180**
- iOS home screen (standard for all iPhones)
- Rounded by Safari automatically
- Crisp anti-aliased edges

**192×192**
- Android home screen
- Supports maskable icons (rounded by Android OS)
- Optimal for PWA installation prompts

**512×512**
- PWA splash screens
- Web app store listings
- Installation prompts

**1024×1024**
- High-res promotional assets
- App store listings (future)
- Marketing materials

---

## 📱 Platform Support

### iOS
- ✅ Home screen installation (Safari Share → Add to Home Screen)
- ✅ Splash screen on app launch
- ✅ Status bar styling
- ✅ Standalone mode (fullscreen, no Safari chrome)
- ✅ Supports all iPhone sizes via auto-scaling

### Android
- ✅ Home screen installation (Chrome → Install App)
- ✅ PWA manifest integration
- ✅ Maskable icon support (OS applies rounding/masking)
- ✅ Standalone mode (fullscreen)
- ✅ App shortcuts (in manifest.json)

---

## 🔗 Integration Checklist

- [ ] Copy all 6 PNG icons to project root or `/public`
- [ ] Copy `manifest.json` to project root
- [ ] Add 6 lines to HTML `<head>` (see Quick Start above)
- [ ] Test locally with `python3 -m http.server 8000`
- [ ] Verify icons appear in DevTools PWA tab
- [ ] Deploy to production
- [ ] Test on real iPhone (Safari → Share → Add to Home Screen)
- [ ] Test on real Android phone (Chrome → Install App)

---

## 🎯 Testing

### Local Testing
```bash
cd /path/to/your/project
python3 -m http.server 8000
# Visit http://localhost:8000 in your browser
# Open DevTools → Application → Manifest
# Should see all icon references with ✓ status
```

### Real Device - iOS
1. Open Safari on iPhone
2. Navigate to your app URL
3. Tap Share icon → "Add to Home Screen"
4. Verify icon shows green peak + gold ring
5. Tap to launch app in fullscreen mode

### Real Device - Android
1. Open Chrome on Android phone
2. Navigate to your app URL
3. Tap menu (⋮) → "Install app" or "Add to Home Screen"
4. Verify icon shows correctly
5. Tap to launch app in fullscreen mode

---

## 📊 File Sizes

| File | Size | Optimized |
|------|------|-----------|
| peak-finance-16x16.png | 552 B | ✅ |
| peak-finance-32x32.png | 1.2 KB | ✅ |
| peak-finance-180x180.png | 9.2 KB | ✅ |
| peak-finance-192x192.png | 10 KB | ✅ |
| peak-finance-512x512.png | 32 KB | ✅ |
| peak-finance-1024x1024.png | 72 KB | ✅ |
| manifest.json | 3.5 KB | ✅ |
| **Total** | **~127 KB** | **Gzip friendly** |

---

## 🎬 What Users See

### iPhone Home Screen
- Icon with rounded corners (auto-applied by iOS)
- App name: "Peak Finance"
- Green peak with gold shimmer
- Launches in fullscreen (no Safari address bar)

### Android Home Screen
- Icon with OS-specific rounding
- App name: "Peak Finance"
- Green peak with gold shimmer
- Launches in fullscreen with web app chrome

### Browser Tab / Bookmark
- Small favicon (16×16 or 32×32)
- Green and gold still visible at tiny scale
- Works across all browsers

---

## 🛠️ Troubleshooting

**Icon doesn't appear on iOS home screen**
- Make sure `manifest.json` is at root level
- Check that `<meta name="apple-mobile-web-app-capable">` is present
- Try clearing browser cache: Settings → Safari → Clear History & Website Data

**Icon appears blurry on Android**
- Ensure `peak-finance-192x192.png` and `peak-finance-512x512.png` exist
- Check manifest.json has correct icon paths
- Force refresh: Long-press app icon → App info → Storage → Clear Cache

**Colors look different on home screen**
- iOS may auto-adjust for dark mode (expected)
- Android respects the image colors exactly
- Both are correct behavior

**App doesn't open fullscreen**
- Make sure `"display": "standalone"` is in manifest.json
- Ensure `<meta name="apple-mobile-web-app-capable" content="yes">` is present
- Try reinstalling: Remove from home screen, add again

---

## 📚 Resources

- [MDN: Web App Manifest](https://developer.mozilla.org/en-US/docs/Web/Manifest)
- [PWA Checklist](https://developers.google.com/web/progressive-web-apps/checklist)
- [iOS Web App Icon Guide](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html)
- [Android Maskable Icons](https://www.w3.org/TR/appmanifest/#icon-masks)

---

**Ready to ship!** 🚀 Your app is now installable on iOS and Android phones with professional branding.

Peak Finance — Climb Higher. Spend Smarter. 🏔️
