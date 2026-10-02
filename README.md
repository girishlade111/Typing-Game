# Typing Scroller Adventure

A browser-based side-scrolling typing game that tests your speed and expands your vocabulary. Explore procedurally generated worlds, bump into floating words, and type them fast and accurately to score points. Themed word lists, hints, and definitions are generated on demand via the Gemini API (bring your own key).

## Features

- **Side-scrolling adventure** — move your character with W/A/S/D through a vibrant canvas world
- **Typing challenges** — collide with a floating word to open a typing modal; score scales with word length and speed
- **AI-generated themes** — click "New Theme" to generate a fresh world with a new word set via the Gemini API
- **Learn as you play** — "Learn Word" fetches a definition after each challenge
- **Contextual hints** — "Get a Hint" produces a sentence using the word in the current theme
- **Responsive, mobile-friendly UI** — minimal design with Tailwind CSS

## Tech stack

- Single-file HTML5 game (`index.html`) — no build step
- HTML5 Canvas for the scrolling world, Tailwind CSS via CDN for styling
- [Gemini API](https://ai.google.dev/) (`gemini-2.5-flash-preview`) for dynamic themes, hints, and definitions

## Quick start

Just open `index.html` in a browser — no install or build needed. For Gemini-powered features, get a free API key from [Google AI Studio](https://aistudio.google.com/) and paste it where prompted in the game UI.

```bash
git clone https://github.com/girishlade111/Typing-Game.git
# then open index.html, or:
npx http-server -p 8080
```

Note: the `Typing Scroller Adventure - Web Page` file is an alternate exported copy of the game.

## Environment variables

None — the game is fully client-side. Your Gemini API key is entered in the browser at runtime and never stored in the repo.

## Deploy notes

Static site — serve the repo root from any static host (GitHub Pages, Netlify, Cloudflare Pages). The root `index.html` is the live game.

## License

MIT

---

Built by [Girish Lade](https://ladestack.in)
