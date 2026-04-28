# 🎵 Anshi Music — by Anshi Singh

A live music discovery website powered by the **Deezer API** with real songs, real album art, and 30-second audio previews.

🌐 **Live at:** [https://anshi7898.github.io/Music-Website/](https://anshi7898.github.io/Music-Website/)

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎧 Real Audio Playback | 30-second previews via Deezer API (no API key needed) |
| 🖼️ Real Album Art | Actual cover images loaded from Deezer |
| 🔍 Live Search | Search any song or artist in real-time |
| 🎤 Artist Browsing | Click any artist to browse their songs |
| 💿 Album Browsing | Click albums to see their full track list |
| ⏯️ Music Player | Sticky bottom player with progress bar, prev/next, volume |
| 📱 Responsive | Works on mobile and desktop |
| 🌌 Dark Theme | Purple/pink gradient dark aesthetic |

---

## 🗂️ Project Structure

```
Music-Website/
├── index.html      ← Entire website (HTML + CSS + JS in one file)
└── README.md       ← This documentation
```

---

## 🚀 How to Host on GitHub Pages (Step-by-Step)

### Step 1 — Create GitHub Repository

1. Go to 👉 [https://github.com/new](https://github.com/new)
2. Repository name: `Music-Website`
3. Set to **Public**
4. Click **Create repository**

### Step 2 — Upload Files

**Easy way (GitHub website):**
1. Open your new repo on GitHub
2. Click **Add file → Upload files**
3. Drag and drop `index.html` and `README.md`
4. Click **Commit changes**

**Using Git (terminal):**
```bash
git init
git add index.html README.md
git commit -m "Launch Anshi Music website"
git branch -M main
git remote add origin https://github.com/anshi7898/Music-Website.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages** (left sidebar)
2. Under **Branch**, select `main` and `/ (root)`
3. Click **Save**
4. Wait ~2 minutes then visit:

👉 **https://anshi7898.github.io/Music-Website/**

---

## 🔌 API Used

**Deezer API** — Free, no API key required  
- Endpoint: `https://api.deezer.com`
- CORS Proxy used: `https://api.allorigins.win` (free, public proxy)

### API Calls Made

| Data | Deezer Endpoint |
|---|---|
| Trending tracks | `/chart/0/tracks?limit=30` |
| Top artists | `/chart/0/artists?limit=14` |
| Top albums | `/chart/0/albums?limit=10` |
| Album tracks | `/album/{id}/tracks` |
| Search | `/search?q={query}` |

---

## 🛠️ How to Customize

### Change Site Name
Search for `Anshi Music` and `Anshi Singh` in `index.html` and replace with your preferred name.

### Change Accent Colors
Edit these CSS variables at the top of `index.html`:
```css
:root {
  --accent: #a78bfa;   /* Purple */
  --accent2: #f472b6;  /* Pink */
  --bg: #080810;       /* Dark background */
}
```

### Load Different Genre/Country Charts
Replace the chart endpoint:
```js
// Bollywood / India chart
await deezer('/chart/116/tracks?limit=30')

// Pop chart
await deezer('/chart/132/tracks?limit=30')
```

---

## 🧰 Technologies

- **HTML5 / CSS3 / Vanilla JavaScript** — No frameworks needed
- **Deezer API** — Real music data & 30s previews
- **AllOrigins Proxy** — Handles CORS for the Deezer API
- **Google Fonts** — Playfair Display + DM Sans
- **GitHub Pages** — Free hosting

---

## 📄 Credits


- Rebuilt with live Deezer API by **Anshi Singh** (`anshi7898`)

---

*© 2025 Anshi Singh · [@anshi7898](https://github.com/anshi7898)*