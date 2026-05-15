# 🔊 MemeSoundBoard

<div align="center">

**Upload, organize, and blast your favorite meme sounds – all from the browser.**

[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-Click%20Here-brightgreen?style=for-the-badge&logo=github&logoColor=white)](https://sonawanemayur-it.github.io/MemeSoundBoard/)
[![GitHub release](https://img.shields.io/github/v/release/Sonawanemayur-IT/MemeSoundBoard?style=flat-square)](https://github.com/Sonawanemayur-IT/MemeSoundBoard/releases)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)

</div>

---

## ✨ Features

- **🎵 Pre‑loaded with default meme sounds** – automatically fetched from a GitHub‑hosted ZIP when you first visit.  
- **📦 Bulk import** – drop a ZIP folder containing multiple MP3/WAV files and they all appear instantly.  
- **📁 Single file upload** – add one sound at a time with a custom name and emoji.  
- **🔊 One‑click playback** – click any card and the sound blasts at full volume.  
- **🗑️ Manage your collection** – delete individual sounds or clear everything with one button.  
- **📤 Export / 📥 Import** – share your collection as a JSON file, or load a friend’s collection.  
- **💾 Local storage** – everything is saved in your browser’s IndexedDB – no server, no tracking.  
- **📱 Responsive design** – works on desktop, tablet, and mobile.

---

## 🛠 Tech Stack

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![IndexedDB](https://img.shields.io/badge/IndexedDB-999999?style=for-the-badge&logo=indexeddb&logoColor=white)
![JSZip](https://img.shields.io/badge/JSZip-3A3A3A?style=for-the-badge&logo=npm&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=github&logoColor=white)

</div>

- **Frontend**: Vanilla HTML, CSS, JavaScript – no frameworks, just pure web goodness.  
- **ZIP handling**: [JSZip](https://stuk.github.io/jszip/) – extracts audio files from ZIPs in the browser.  
- **Data storage**: IndexedDB – stores your sounds locally with virtually no size limit.  
- **Hosting**: GitHub Pages – lightning‑fast, free, and always up to date.

---

## 🚀 Quick Start (Use it right now)

1. **Visit the live site** 👉 [Live Demo](https://soundboard-mocha-five.vercel.app/)  
2. The app automatically loads the default meme sounds (from your GitHub ZIP).  
3. Click any card to play the sound.  
4. Want your own? Drag & drop a ZIP file onto the upload zone, or add single files.

> 💡 **Tip**: The first time you open the site, it will fetch the default sounds. After that, they’re saved in your browser – no need to download again.

---

## 📦 Adding your own sounds

You can easily replace the default sounds with your own collection:

1. **Create a ZIP folder** containing your MP3, WAV, M4A, etc. files.  
2. Upload that ZIP to your own GitHub repository (or any public hosting).  
3. In `index.html`, change the `DEFAULT_ZIP_URL` variable to the **raw URL** of your ZIP:

   ```javascript
   const DEFAULT_ZIP_URL = 'https://raw.githubusercontent.com/YourUsername/YourRepo/main/your-sounds.zip';
