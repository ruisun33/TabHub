# TabHub

**Your tab command center.**

TabHub replaces your new tab page with a clean dashboard of everything you have open. Tabs are grouped by domain — and by native tab groups — so you can see, navigate, and close them without hunting through a cluttered tab bar.

Works on **Chrome** and **Firefox**.

---

## Features

- **Domain grouping** — tabs from the same site grouped into one card
- **Native tab group support** — Chrome and Firefox tab groups shown as their own cards with group name and color
- **Homepages group** — Gmail, X, LinkedIn, YouTube, GitHub homepages pulled into one card for easy cleanup
- **Duplicate detection** — flags when you have the same page open twice, one-click cleanup
- **Click any tab to jump to it** — works across windows
- **Save for later** — bookmark tabs before closing them, stored locally in your browser
- **Localhost grouping** — shows port numbers next to each tab so you can tell your local projects apart
- **Expandable groups** — first 8 tabs visible, rest behind a "+N more"
- **Toolbar badge** — live tab count, color-coded green → amber → red as tabs pile up
- **100% local** — no server, no account, no data sent anywhere

---

## Install

**1. Clone the repo**

```bash
git clone https://github.com/rsunam/Tabout.git
cd Tabout
```

**2. Load the extension**

**Chrome:**
1. Go to `chrome://extensions`
2. Enable **Developer mode** (top-right toggle)
3. Click **Load unpacked** → select the `extension/` folder

**Firefox:**
1. Go to `about:debugging` → **This Firefox**
2. Click **Load Temporary Add-on** → select `extension/manifest.json`

**3. Open a new tab — you'll see TabHub.**

---

## Tech stack

| What | How |
|---|---|
| Extension | Chrome + Firefox Manifest V3 |
| Storage | chrome.storage.local |
| Tab groups | chrome.tabGroups API (Chrome + Firefox 138+) |
| Animations | CSS transitions + JS confetti particles |

---

## License

MIT
