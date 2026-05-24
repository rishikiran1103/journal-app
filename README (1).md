# 📓 My Journal App

A fully offline, privacy-first journaling app with rich text editing and stylus handwriting support — built as a single HTML file with no frameworks or build steps.

**[→ Live Demo](https://YOUR-USERNAME.github.io/journal-app)**

---

## Features

**Writing**
- Rich text editor — bold, italic, underline, headings, bullet & numbered lists
- Highlight text, stamp date & time, word count in status bar
- Mood tagging per note (😊 😌 😐 😔 🙏 🎉)
- Live search across all note titles and content
- Export as `.txt` or print to PDF

**Drawing & Handwriting**
- Full canvas drawing mode — pen, marker, and eraser tools
- Stylus pressure sensitivity and tilt detection via Pointer Events API
- Palm rejection — finger touches ignored while stylus is active
- Pinch-to-zoom and scroll-wheel zoom with pan
- Customizable color palette with persistent preferences
- Toggleable lined paper overlay
- Undo / redo stroke history
- Export drawing as `.png`

**App**
- Dark / light theme — follows system preference, manually overridable
- Collapsible sidebar, responsive at all window sizes
- 100% offline — all notes stored locally, no account needed
- Zero dependencies — one `.html` file, open in any browser

---

## Tech Stack

| Layer | Technology |
|---|---|
| UI & Logic | Vanilla HTML, CSS, JavaScript (ES6+) |
| Styling | CSS custom properties (full theming system) |
| Text editing | `contenteditable` + `execCommand` |
| Drawing | HTML5 Canvas API |
| Stylus input | Pointer Events API (`pressure`, `tiltX`, `pointerType`) |
| Storage | `localStorage` (browser) |
| Fonts | Google Fonts — Lora, DM Sans |

Also available as a **native Windows desktop app** built with Electron — file storage via Node.js `fs`, native menus, print dialog, and a Windows installer packaged with electron-builder + NSIS.

---

## Getting Started

No install needed. Just open the file:

```
# Clone the repo
git clone https://github.com/rishikiran1103/journal-app.git

# Open in your browser
open journal-app.html        # macOS
start journal-app.html       # Windows
xdg-open journal-app.html    # Linux
```

Or just **[open the live demo](https://YOUR-USERNAME.github.io/journal-app)** directly in your browser.

---

## Screenshots

> *(Add screenshots here once deployed — one of the text editor, one of the draw mode)*

---

## Roadmap

- [ ] Export / import all notes as JSON backup
- [ ] Image paste into text notes
- [ ] OneDrive / cloud sync (desktop version)
- [ ] Mobile PWA packaging

---

## License

MIT — do whatever you like with it.
