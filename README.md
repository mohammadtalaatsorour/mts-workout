# 🏋️ MTS Workout — Round System PWA
### by Mohamed Talaat Sorour · #MTSCodes

---

## 📱 How to Install as a Mobile App

### Android (Chrome) — Recommended
1. Upload the folder to **GitHub Pages** (free) — see below
2. Open the URL in Chrome on your Android phone
3. Chrome will show a banner: **"Add to Home Screen"** — tap it
4. The app installs with its own icon, runs fullscreen, and **screen sleep is fully prevented** ✅

### iOS (Safari)
1. Upload to GitHub Pages (see below)
2. Open the URL in Safari
3. Tap the **Share button** → **"Add to Home Screen"**
4. Done — runs as a standalone app

---

## 🚀 Deploy to GitHub Pages (Free, 5 minutes)

1. Go to **github.com** → sign in or create a free account
2. Click **New Repository** → name it `mts-workout` → set to **Public** → Create
3. Upload all files from this folder (index.html, manifest.json, sw.js, icon-*.png)
4. Go to **Settings** → **Pages** → Source: **main branch / root**
5. Your app is live at: `https://YOUR-USERNAME.github.io/mts-workout`
6. Open that URL on your phone → install → done!

---

## 💻 Run Locally (Quick Test)

```bash
# Option 1: Python (built-in)
cd mts-workout
python3 -m http.server 8080
# Open: http://localhost:8080

# Option 2: Node
npx serve .
```

Then open `http://localhost:8080` in Chrome — Wake Lock works on localhost too.

---

## ✨ Features as a PWA

| Feature | Status |
|---------|--------|
| Install to Home Screen | ✅ Android + iOS |
| Fullscreen (no browser chrome) | ✅ |
| Works Offline | ✅ Service Worker |
| Screen Always On (Wake Lock API) | ✅ Works when installed |
| App Icon | ✅ Custom dumbbell icon |
| Theme Color (dark red) | ✅ |
| Notch / Safe Area Support | ✅ |
| 45s Tap Reminder Overlay | ✅ |
| Triple Beep + Vibration | ✅ |
| Round Auto-tracking | ✅ |

---

## 📁 Files

```
mts-workout/
├── index.html          ← Main app
├── manifest.json       ← PWA config
├── sw.js               ← Service Worker (offline)
├── icon-192.png        ← App icon (Android)
├── icon-512.png        ← App icon (large)
└── apple-touch-icon.png ← App icon (iOS)
```

---

## Why Wake Lock Works as a PWA

When opened as `file://`, Chrome blocks the Wake Lock API for security.
When installed as a PWA (or served over HTTPS/localhost), Chrome grants full
Wake Lock access — the screen **never** sleeps while the countdown is running.

The small green dot (top-right corner) shows Wake Lock is active 🟢

---

*Consistency is the key to success 💪 — #MTSCodes*
