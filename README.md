# Brendan's XP Portfolio

A personal website dressed up as a Windows XP desktop. Click icons, drag windows around, minimize stuff — the whole bit.

Built on top of [XP.css](https://github.com/botoxparty/XP.css), a CSS library that makes plain HTML look like old Windows UI. This repo has that library in it (`gui/`, `themes/`, `build.js`) plus the actual site.

## What's in `index.html`

Everything lives in one file — HTML, CSS, and JS. 

**The desktop**
- Bliss wallpaper background
- Six desktop icons: Welcome, Portfolio, About Me, Contact, Interests, and Photography
- Photography opens a confirmation dialog before sending you to [sarpongphotos.com](https://sarpongphotos.com)

**The windows**
- **Welcome** — intro popup with headshot and a quick bio. Opens on load.
- **Portfolio** — projects (Sample Search, GTS Misinformation, Surgery Turnover App, Gr8 Eagle Cyber, etc.)
- **About Me** — skills, experience, general background
- **Contact** — email, LinkedIn, GitHub, Spotify
- **Interests** — camcorder clips, photos, album covers, paintings, and other hobbies

**The taskbar**
- Start button (reloads the page)
- Live clock
- Taskbar buttons for each open window — click to restore, drag title bars to move

**Other behavior**
- XP startup sound on first click/tap
- Draggable windows with minimize/close controls (maximize is disabled)
- Photo lightbox for images in the Interests window
- Responsive tweaks for mobile

## Other folders (briefly)

| Folder | What it is |
|--------|------------|
| `gui/`, `themes/` | XP.css source — shared component styles and XP/98 theme overrides |
| `docs/` | Component documentation site for the CSS library |
| `misc images/`, `Windows XP Icons/`, `album covers/` | Assets for the portfolio |
| `dist/` | Built CSS output (from `npm run build`) |

## Running it

**Portfolio:** open `index.html` in a browser. A local server works better if audio or file paths act up:

```
npx live-server
```

**CSS library dev:** `npm install`, then `npm run build` to compile styles into `dist/`.

## Credits

- UI styling: [XP.css](https://github.com/botoxparty/XP.css) by Adam Hammad (MIT)
- Site content and window logic: Brendan Sarpong
