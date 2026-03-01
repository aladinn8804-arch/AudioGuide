# АудиоГид / AudioGuide — Setup Guide

## How to host (free, 5 minutes)

### Option A — Netlify Drop (easiest)
1. Go to https://app.netlify.com/drop
2. Drag the entire `audio-guide-app` folder onto the page
3. Netlify gives you a URL like `https://quirky-name-123.netlify.app`
4. Share that link with everyone

### Option B — GitHub Pages
1. Create a free GitHub account
2. Create a new repository, upload all 3 files
3. Go to Settings → Pages → Deploy from branch (main)
4. Your app will be at `https://yourname.github.io/repo-name`

---

## How to install on phone
1. Open the URL in **Chrome** (Android) or **Safari** (iPhone)
2. Tap the browser menu → **"Add to Home Screen"**
3. Done — it works like a real app, offline too

---

## Admin setup
- Default password: **admin123**
  (change it by editing `ag_adminpass` in browser localStorage, or ask a developer to hardcode it)

## Google Drive integration (optional)
For the shared Drive feature, as admin:
1. Create a folder in Google Drive
2. Right-click → Share → "Anyone with the link can view"
3. Copy the folder ID from the URL (the long string after `/folders/`)
4. Go to https://console.cloud.google.com → Create a project → Enable Drive API → Create API Key
5. In the app: ⚙ → Admin Panel → paste Folder ID + API Key → Save & Connect

> Note: Google Drive integration lets you reference files by URL.
> For fully offline audio, use the Upload feature — files are stored directly in the app on each device.

---

## Features
- 🗂 Create / rename / delete folders (admin only)
- 🎧 Upload audio files — auto-numbered, play in order
- ⏮⏯⏭ Full playback controls with progress bar
- 🌐 Russian / English language toggle
- 📴 Works offline after first load
- 🔒 Password-protected admin panel
