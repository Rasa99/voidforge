# VoidForge

A tiny browser-based pixel art editor for Steam emoticons. Paint on a grid using your
owned `:emoticon:` codes, and it generates ready-to-paste code for Steam chat, comments,
or your profile — gaps filled with the braille blank `⠀` (U+2800), the "void" Steam
users use to keep whitespace from collapsing.

No build step, no dependencies, no backend. It's a single `index.html` file that runs
entirely in the browser — nothing you draw ever leaves your machine.

## Features

- Brush / erase / flood-fill / line / rectangle / eyedropper tools, with undo/redo
- Resizable grid (up to 60×60), mirror and shift transforms, crop-to-art
- Gap-width control (1.5–3 voids per cell) so output actually lines up in Steam's
  proportional-width rendering instead of drifting — includes an auto-fit measurer
- Live "Steam preview" that renders the real emoticon images at real pixel size
- Import your own emoticon list by pasting a public Steam inventory JSON export, or
  just paste any text containing `:tokens:`
- Import existing emoticon-art code back into the grid for editing
- Save/open your work as `.json`, export the code as `.txt`

## Running it locally

Just open `index.html` in a browser. That's the whole app.

## Deploying

Static hosting only — point any static host (Vercel, Netlify, GitHub Pages, Cloudflare
Pages, or a plain web server) at this folder; `index.html` is the entry point.

## License

Public domain — [Unlicense](LICENSE). Do whatever you want with it.
