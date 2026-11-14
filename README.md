# Left Luggage

<pre></pre>
<p align="center"><a href="https://dinocodes-potter.github.io/Left-Luggage/"><strong>🌐 OPEN LEFT LUGGAGE — PLAY THE LIVE WEBSITE</strong></a></p>

**A peculiar little lost-property office. Forty-four unclaimed bags. Forty-four tags. A lot more going on than meets the eye.**

Left Luggage is a browser-based puzzle experience built around an old-fashioned railway lost-property counter. Each luggage tag presents a small challenge: some are word puzzles, some require a closer look at the page, and a few ask you to interact with the browser itself.

The visual identity is deliberately tactile and archival: deep station-green, aged luggage-tag paper, brass details, red claim stamps, stencil lettering and typewriter text.

## Play

**[Open the website](https://dinocodes-potter.github.io/Left-Luggage/)** or open [`index.html`](index.html) locally in a modern browser. There is no build step, package manager or server-side dependency.

## Features

- **44 progressive puzzles** combining riddles, wordplay, visual clues and browser-based interactions.
- **Persistent progress** saved locally in the browser, so claimed bags stay claimed on the same device and browser.
- **Day and night themes**, with the selected theme remembered between visits.
- **Clerk hints**, optional feedback, hidden interactions and playful easter eggs.
- **Responsive layout** for desktop and mobile, with keyboard focus states and reduced-motion support.
- **No framework or runtime dependencies.** Google Fonts are loaded remotely; system fallbacks are provided.

## Project structure

```text
left-luggage/
├── index.html          # Complete application: markup, styles and puzzle logic
├── assets/
│   └── favicon.svg     # Matching luggage-tag site icon
└── README.md
```

The experience is intentionally kept as a self-contained static page. This keeps deployment simple and avoids introducing a build pipeline for a project that does not need one.

## Run locally

1. Clone or download this repository.
2. Open `index.html` in your browser.

For a local HTTP server (optional):

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select `main` and `/ (root)`, then save.
4. Wait for the Pages deployment to finish; GitHub will show the published URL in the Pages settings.

## Privacy and storage

Puzzle progress and the selected theme are stored in the browser's `localStorage`. They are not sent to a server. Clearing this site's browser storage resets local progress and preferences.

## Accessibility notes

The interface includes semantic buttons and form controls, visible keyboard focus, descriptive control labels, a live app region, and a `prefers-reduced-motion` override. Some puzzles intentionally rely on browser features such as hover, selection, the developer console or viewport dimensions; the clerk's hint is available when a clue needs a nudge.

## Credits

Created as a standalone interactive web project. The visual language and puzzle content are part of the Left Luggage experience.
