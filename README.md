# 🎵 Spotify Clone

A fully functional Spotify-inspired music player built with HTML, CSS, and vanilla JavaScript.

---

## 📸 Preview

> Open `index.html` in a browser with a local server (Live Server recommended) to see the full experience.

---

## ✨ Features

- 🎧 **Music Playback** — Play, pause, skip to next/previous song
- 📁 **Multiple Playlists** — Browse albums like *Dusk Diaries*, *Nocturnal Bloom*, *Amber Haze* and more
- 🔊 **Volume Control** — Slider + mute/unmute toggle
- ⏱️ **Seekbar** — Click anywhere on the seekbar to jump to that position
- ⏲️ **Live Song Timer** — Shows current time and total duration
- 📱 **Responsive Design** — Works on mobile, tablet, and desktop
- 🍔 **Hamburger Menu** — Collapsible sidebar for smaller screens
- 🔐 **Sign In / Sign Up Pages** — Spotify-style auth UI

---

## 📂 Project Structure

```
Spotify/
├── index.html          # Main player page
├── sign in.html        # Login page
├── signup.html         # Registration page
│
├── css/
│   ├── style.css       # Main stylesheet
│   ├── utility.css     # Utility classes
│   ├── sign in.css     # Login page styles
│   └── sign up.css     # Signup page styles
│
├── js/
│   └── script.js       # All player logic
│
├── img/
│   ├── logo.svg        # Spotify logo
│   ├── play.svg        # Play icon
│   ├── pause.svg       # Pause icon
│   ├── volume.svg      # Volume icon
│   └── ...             # Other icons
│
└── songs/
    ├── ncs/            # Playlist: Dusk Diaries
    ├── cs/             # Playlist: Nocturnal Bloom
    ├── new1/           # Playlist: Amber Haze
    ├── new2/ ... new9/ # More playlists
    └── (each folder has cover.jpg, info.json, and .mp3 files)
```

---

## 🚀 How to Run

### Option 1: VS Code Live Server (Recommended)

1. Open the `Spotify` folder in **VS Code**
2. Install the **Live Server** extension
3. Right-click `index.html` → **"Open with Live Server"**
4. The app opens at `http://127.0.0.1:5500`

### Option 2: Any Local Server

```bash
# Python
cd Spotify
python3 -m http.server 5500

# Node.js (npx)
npx serve .
```

> ⚠️ **Do not open `index.html` directly** by double-clicking — songs won't load because the app uses `fetch()` to read the songs folder, which requires a server.

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Page structure |
| CSS3 | Styling, animations, responsive layout |
| JavaScript (ES6+) | Player logic, DOM manipulation, async/await |
| Web Audio API | `<audio>` element for playback |
| Google Fonts | Roboto & Lato fonts |

---

## 🎵 How to Add Your Own Songs

1. Create a new folder inside `songs/` (e.g. `songs/myplaylist/`)
2. Add your `.mp3` files to that folder
3. Add a `cover.jpg` (album art)
4. Create an `info.json` file:

```json
{
  "title": "My Playlist",
  "description": "A short description of this playlist."
}
```

5. The playlist will automatically appear on the main page!

---

## 👨‍💻 Made By

**Umer** — Spotify Clone Project  
Built as a frontend practice project.

---

## 📄 License

This project is for **educational purposes only**.  
All music belongs to their respective artists and labels.  
Spotify name and logo are trademarks of **Spotify AB**.
