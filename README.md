# 🗂️ The Nucleus — Archive

A single-file, self-contained web app for recording the lore, running jokes, and incidents of a Discord server ("The Nucleus"). No build step, no backend — open it in a browser and it works.

**[Live demo](https://claude.ai/artifact/LheTe4rRZX7Mb2gnJHghza)**

## Features

- 📜 Browsable list of archived events, expandable on tap/click
- ✏️ Inline-editable titles
- 📝 Freeform notes per entry for the actual story/lore
- 🔍 Instant client-side search/filter
- 💾 Persists locally via `localStorage` — no account, no server, no data leaves your browser
- 🌗 Light/dark mode, follows system preference
- 📱 Responsive, safe-area aware for mobile

## Getting Started

No dependencies, no build tools.

```bash
git clone https://github.com/<your-username>/nucleus-archive.git
cd nucleus-archive
open index.html   # or just double-click the file
```

### Hosting on GitHub Pages

1. Rename `nucleus-archive.html` to `index.html`.
2. Push to a repo, then enable **Settings → Pages → Deploy from branch → main / root**.
3. Your archive is live at `https://<your-username>.github.io/<repo-name>/`.

## Usage

- Tap an entry to expand it.
- Tap **✏️** next to a title to rename it (Enter or tap away to save).
- Type your notes in the textarea and hit **Save**.
- Use the search bar to filter events by title.

## Project Structure

```
.
├── index.html      # entire app — markup, styles, and logic in one file
├── README.md
└── LICENSE
```

## Data & Privacy

All data is stored in the browser's `localStorage`, scoped to the device and browser it was entered on. There is no backend, database, or sync — clearing browser data will erase entries. Export/backup is a good next feature if you want to extend this (see below).

## Roadmap / Ideas for Contribution

- [ ] Export/import archive as JSON
- [ ] Add new entries (not just edit existing ones)
- [ ] Timestamps / chronological sort
- [ ] Tagging system beyond the single `(ongoing)`-style tag

## Contributing

Pull requests welcome. For significant changes, open an issue first to discuss what you'd like to change.

## License

[MIT](LICENSE)
