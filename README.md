[README.md](https://github.com/user-attachments/files/29923289/README.md)
# Wisp

Wisp helps you make decisions, without making them for you.

Making decisions isn't easy. We spend too little thought on the important ones, or waste too much on the small ones. Wisp doesn't decide for you, and it never will. It notices the shape of your decision, how much is at stake, how clear your feelings already are, and sets out a structured process for *you* to think it through: weighing trade-offs, surfacing what you actually feel, testing a lean you already have, or just settling a coin-flip-worthy choice. Each process is grounded in published decision-science and psychology research, not invented from scratch.

**[Open Wisp →](#)** *(link once this is live on GitHub Pages)*

---

## What this is

A single HTML file. No install, no account, no build step. Open the link (or download `index.html` and open it in a browser) and it runs entirely client-side.

- **Everything you write stays on your device**, in your browser's local storage. Nothing is transmitted anywhere by default.
- **No server, and no API key of the developer's, anywhere in this repository.** There is nothing here for anyone but you to see.
- **One optional feature uses AI**: Distil, which can turn a free-write brain-dump into themes and tensions reflected back in your own words. It's opt-in, and it works one of two ways, both entirely on your terms:
  - Bring your own Anthropic API key (if you have a developer profile with Anthropic), sent only from your browser directly to Anthropic, never through this app's developer.
  - Or copy a ready-made prompt plus your writing, and paste it into any AI chat you already use, then paste the response back in to save it.
- **Every other mode** — Flip, Surface, Gut check, Analyze, Mull, Good enough — runs entirely on-device and never touches a network at all.

## Privacy and security

This is the whole point of the project, so it's worth stating plainly:

- Search this repository yourself. There is no API key, no `.env`, no server route, and no build pipeline that could hold or leak one.
- The one AI feature (Distil) only ever uses a key **you** provide, entered into your own browser, used only to call Anthropic directly from your machine. It's never sent to, or visible to, whoever's hosting this page.
- Your journal, your key (if you choose to save one), and everything else lives in your browser's local storage on your device only. Clearing your browser data, or using a different device or browser, means it won't be there. You can export your journal (About → Your data → "Download journal") or erase everything at any time.

## Running it yourself

No build step required. Clone the repo and open `index.html` directly in a browser, or serve the folder with any static file server:

```bash
git clone <this-repo-url>
cd wisp
open index.html          # macOS
# or: python3 -m http.server, then visit localhost:8000
```

If this repo also includes the readable source (`wisp.jsx`), that's the uncompiled version, useful for reading exactly what the app does before trusting it with anything. `index.html` is the same code, bundled and minified for distribution.

## What's inside

- **Flip / roll** — when either option is honestly fine
- **Surface** — sentence stems and feeling-words, for when you're not sure what you think yet; a matched question bank helps you go further, entirely local, no AI
- **Gut check** — pressure-tests a lean you already have
- **Analyze** — weighted scoring for measurable trade-offs
- **Mull** — for big, personal decisions you want to sit with over time
- **Good enough** — for when comparing more options stops helping
- **Distil** — free-write reflection, the one optional AI-assisted feature, described above

A one-way safety gate declines to help with anything touching self-harm, harming others, or illegal acts, and points toward real crisis resources instead. It runs entirely on-device, deliberately erring on the side of caution.

## Tech

Plain React, bundled with esbuild into a single self-contained file (React and ReactDOM are inlined, not loaded from a CDN). No frameworks beyond that, no backend.

## License

*(add your preferred license here)*

## Credits

Developed by Ndromedia.
