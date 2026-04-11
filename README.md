# 🧘‍♀️ Yoga with Jib — Class Tracker

A clean, minimal class tracking app for yoga teachers. Students buy prepaid packages and you deduct one each time they attend. Students can see their own balance on the same page.

---

## How to deploy (GitHub Pages)

1. Go to [github.com](https://github.com) and create a free account
2. Click **New repository** → name it `yoga-with-jib` → set to **Public** → click **Create**
3. Click **Add file → Upload files** → drag `index.html` in → click **Commit changes**
4. Go to **Settings → Pages** → Source: **Deploy from branch → main** → Save
5. Wait ~1 minute → your app is live at `https://yourusername.github.io/yoga-with-jib`

---

## How to use

### Student view (default)
- Shows all students' name, symbol, class balance and status
- Read-only — students can look but not change anything
- Share the URL with your students so they can check anytime
---

## Adding Fabfeltscript Bold (optional)

1. Download **Fabfeltscript Bold** from [cdnfonts.com](https://www.cdnfonts.com) or [dafont.com](https://www.dafont.com)
2. Upload the font file (e.g. `FabfeltScript-Bold.woff2`) to your GitHub repo alongside `index.html`
3. In `index.html`, replace the Google Fonts `<link>` tag with:

```css
@font-face {
  font-family: 'FabfeltScript';
  src: url('FabfeltScript-Bold.woff2') format('woff2'),
       url('FabfeltScript-Bold.ttf') format('truetype');
  font-weight: bold;
}
```

4. Find `.brand-main` in the CSS and add:

```css
.brand-main {
  font-family: 'FabfeltScript', cursive;
}
```

---

## Customisation

| What | Where in index.html |
|------|-------------------|
| Brand name | Find `Yoga with Jib` in the HTML (appears twice) |
| Pink color | Find and replace `#fb2a7b` |
| Package sizes | Edit the `.pkg-opt` buttons in the modals |
| Card colors | Edit the `COLORS` array in the script |
| Symbol options | Edit the `SYMBOLS` array in the script |
| Default PIN | Change `'1234'` in `let pin = '1234'` |

---

## Tech

- Plain HTML + CSS + JavaScript — no frameworks, no build tools
- IBM Plex Sans via Google Fonts
- Data saved in `localStorage` (stays on the device/browser)

> **Note:** Because data is stored in `localStorage`, each device/browser has its own copy. If you want all devices to share the same data, you would need a backend database.

---

Made with 💗 for Yoga with Jib
