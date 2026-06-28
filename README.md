# Happy Birthday Website — Setup Guide 💛

This is a complete, ready-to-open birthday website built with React. There is
**no installation, no Node.js, and no command line needed** — everything
runs from the `index.html` file in this folder.

---

## 1. What's inside

```
birthday-surprise/
├── index.html              ← open this file to view the website
├── README.md                ← this guide
└── assets/
    ├── hero.jpg              ← the hero/background photo
    ├── vendor/                ← React + Babel, bundled locally (don't touch)
    ├── music/
    │   └── ADD_YOUR_SONG_HERE.txt
    └── photos/
        ├── photo_1.jpg   ✅ already added
        ├── photo_2.jpg   ✅ already added
        ├── photo_3.jpg   ✅ already added
        ├── photo_4.jpg   ⬜ add this
        ├── photo_5.jpg   ⬜ add this
        ├── photo_6.jpg   ⬜ add this
        ├── photo_7.jpg   ⬜ add this
        ├── photo_8.jpg   ⬜ add this
        ├── photo_9.jpg   ⬜ add this
        └── photo_10.jpg  ⬜ add this
```

I could only use the 4 images you uploaded in our chat (the hero photo +
3 gallery photos), so those are already in place. The gallery is built for
**10 photos** with captions exactly as you wrote them — you just need to
drop in the remaining 7 photos.

## 2. Add your remaining photos (optional but recommended)

1. Open the `assets/photos` folder.
2. Add your photos and **rename each one exactly**: `photo_4.jpg`,
   `photo_5.jpg`, `photo_6.jpg`, `photo_7.jpg`, `photo_8.jpg`, `photo_9.jpg`,
   `photo_10.jpg`.
3. If a photo is a `.png` or `.jpeg`, just rename the extension to `.jpg` —
   browsers don't actually check the file content, so this works fine.

> Don't have a photo for one of the slots yet? No problem — the gallery
> will show a friendly placeholder for that slot instead of breaking, so you
> can still send the site before all 10 are filled in.

## 3. Add a song for the final surprise (optional)

The very last screen (after she taps "YES ❤️") is built to play a song while
hearts and confetti fill the screen.

1. Pick any song file you have the rights to use (mp3 format).
2. Rename it to exactly `music.mp3`.
3. Put it inside `assets/music/`.

If you skip this step, the celebration screen still works perfectly — it
will simply be silent.

## 4. Open the website

Just **double-click `index.html`**. It will open in your default browser
(Chrome, Edge, Firefox, or Safari all work great).

That's it — no setup, no terminal, nothing to install.

> 💡 One thing to know: the decorative fonts (the elegant headings and the
> handwriting font for the letter) load from Google Fonts, so it's best to
> have an internet connection the first time it's opened. Everything else —
> React, the animations, the photos, the letter, the confetti — works
> completely offline.

### If double-clicking doesn't work well on your computer
Some browsers are a little stricter about opening local files directly.
If anything looks off, you can run a tiny local server instead:
- **Mac/Linux:** open Terminal in this folder and run
  `python3 -m http.server 8000`, then visit `http://localhost:8000` in your
  browser.
- **Windows:** open this folder, type `cmd` in the address bar to open a
  terminal there, then run the same command (use `python` if `python3`
  isn't recognized).

## 5. The secret passcode 🔒

The love letter is locked behind a passcode: **17-05-26**. She can type it
with or without the dashes (`170526` also works). If you want to change it,
open `index.html` in any text editor, search for:

```js
const CORRECT_PASSCODE = "170526";
```

and replace `170526` with your own date, digits only (e.g. for 04-08-23,
use `040823`).

## 6. Want to tweak anything else?

Everything — text, colors, the birthday date, the letter, the reasons list —
lives inside `index.html`, in clearly labeled sections near the top of the
`<script type="text/babel">` block (look for `PHOTOS`, `REASONS`, and
`LETTER`). You don't need any special tools, just a text editor (Notepad,
TextEdit, or VS Code all work).

---

Made with care, for the surprise you're planning. I hope she loves it. ❤️
