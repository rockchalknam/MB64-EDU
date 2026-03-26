# MB64 EDU — The Web-Console

A browser-based hosting platform for Mario Builder 64 v1.1 Beta, built for classroom use.

## Setup

### 1. Add your ROM

Create a `rom/` folder in the repo root and place your patched ROM inside:

```
rom/
  mario_builder_64_v1.1.z64
```

The `index.html` points to this path by default. If your filename is different, update this line in the script:

```js
window.EJS_gameUrl = 'rom/mario_builder_64_v1.1.z64';
```

### 2. Enable GitHub Pages

- Go to your repo → **Settings** → **Pages**
- Set source to `main` branch, `/ (root)` folder
- Hit Save — your site will be live at `https://yourusername.github.io/your-repo-name`

### 3. Share with students

Give students the GitHub Pages URL. No downloads, no installs — it runs entirely in the browser.

---

## Controls

| Key | Action |
|---|---|
| W A S D | Move |
| Space | Jump |
| Z | A Button |
| X | B Button |
| Enter | Start |
| F | Fullscreen |
| M | Mute |

---

## File Structure

```
/
├── index.html        ← main page
├── rom/
│   └── mario_builder_64_v1.1.z64   ← your patched ROM goes here
└── README.md
```

---

## Notes

- EmulatorJS loads from CDN — students need internet access (standard school Wi-Fi is fine)
- The ROM file is not included in this repo — add your authorized copy to the `rom/` folder
- GitHub has a 100MB file size limit per file. The patched ROM should be well under that.
- If your school blocks GitHub Pages, the same `index.html` works on any static host (Google Sites embed, Netlify, etc.)

---

Built for educational use · Mario Builder 64 by [Rovertronic](https://github.com/rovertronic/Mario-Builder-64) & Arthurtilly
