# MC Cards

Swipeable cue cards for MCs and speakers. Write a list, reorder it, then present it as big full-screen cards you flick through with your thumb. It's a single HTML file that works offline.

## Features

- **Lists**: keep several lists (announcements, run sheets, speaker notes) saved in your browser.
- **Reorder**: drag the handle or tap ▲/▼ before presenting.
- **Swipe card stack**: the top card follows your thumb, tilts, and flies off; Back restores the last card. Keyboard: →/Space next, ← back, Esc exit.
- **Share via link**: the list is compressed into the URL hash (`#l=...`). The hash is never sent to a server. Opening a link asks before importing it as a new list.
- **Theming**: light, dark, or system mode, plus an accent colour picker.
- **Offline, single file**: no build, no dependencies, no backend.

## Usage

1. Open `index.html` (or the deployed site) on your phone.
2. Create or edit a list. Each item is a card: the first line is the title, the rest is detail.
3. Reorder, then tap **Present** and swipe through.
4. Tap **Share** to send the list to someone else.

## Deploy to Cloudflare Pages

It's a static site with no build step.

- Connect this repo in Cloudflare Pages.
- Framework preset: None. Build command: (leave empty). Build output directory: `/`.

Any static host (GitHub Pages, Netlify, etc.) works the same way.

## Privacy

Lists are stored only in your browser's localStorage (`mccards.v1`). Nothing is sent to any server. Shared links carry the list in the URL hash, which browsers don't send to servers, though anyone with the link can read it.

## License

MIT © 2026 Dave Pengelley. See [LICENSE](LICENSE).
