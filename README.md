# 🎵 Mast Music

Mast Music is a simple music discovery web application built using **HTML, CSS and Vanilla JavaScript** that allows users to search for songs and artists using the **iTunes Search API**, preview tracks, and browse featured music banners.

---

## 🚀 Features

- 🔎 Search songs by artist or track name
- 🎧 30-second audio previews
- 🖼 Album artwork display
- 👤 Artist information cards
- ⏸ Auto-pause currently playing audio when another track starts
- 🎨 Custom dark-themed responsive UI
- 🏠 Featured music banners and artist showcase section

---

## 📂 Project Structure

```bash
Mast-Music/
│
├── index.html      # Main application structure
├── style.css       # Styling and responsive layout
├── script.js       # Search logic, API integration, audio controls
└── README.md
```

---

## 🛠 Tech Stack

- HTML5
- CSS3
- JavaScript (ES6)
- iTunes Search API

---

## ⚙️ How It Works

### 1. Search for Music
Enter an artist or song name in the search bar:

```text
Arijit Singh
```

The app fetches matching tracks from:

```javascript
https://itunes.apple.com/search?term=<search-term>
```

---

## 2. Dynamic Song Cards
Each result displays:

- Album artwork
- Artist name
- Song title
- Audio preview player

---

## 3. Single Audio Playback Logic
Only one preview plays at a time.

```javascript
document.addEventListener('play', event => {
    const audio = document.getElementsByTagName('audio');
    for (let i = 0; i < audio.length; i++) {
        if (audio[i] != event.target) {
            audio[i].pause();
        }
    }
}, true)
```

---

## 📸 UI Sections

### Header
- Brand logo/title
- Search bar
- Search button

### Search Results
Dynamic song cards rendered from API responses.

### Featured Home Section
Includes:
- Featured banners
- Artist highlights
- Curated playlist visuals

---

## ▶️ Running Locally

Clone the repository:

```bash
git clone https://github.com/yourusername/mast-music.git
cd mast-music
```

Open:

```bash
index.html
```

in your browser.

No build setup required.

---

## 📷 Preview

Add screenshots/gif here:

```markdown
![App Screenshot](screenshots/home.png)
```

---

## 🔮 Possible Improvements
Future enhancements:

- Search on Enter key press
- Pagination / infinite scrolling
- Genre filters
- Favorites playlist
- Dark/Light mode toggle
- Mobile optimization improvements
- Spotify or YouTube integration
- Lyrics support

---

## 🐛 Known Issues
- Depends on iTunes API availability
- Some search terms may return incomplete previews
- Layout can be further optimized for smaller screens

---

## 🤝 Contributing

Pull requests and improvements are welcome.

1. Fork the repo  
2. Create feature branch

```bash
git checkout -b feature-name
```

3. Commit changes

```bash
git commit -m "Added feature"
```

4. Push branch

```bash
git push origin feature-name
```

5. Open Pull Request

---

## 📄 License
MIT License

---

## 👨‍💻 Author
Developed by **Sourav** just for testing


```
