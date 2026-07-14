# notedrop

A black page. Drop a note. It files itself.

**Live app:** https://anmoba99.github.io/notedrop/

## What it is

A radically simple reminder / list app:

- Open the app → one input on a black page. Type a sentence (or a word), hit enter.
- Every note is **auto-classified** into a category. Categories are **dynamic** — they're created as your notes need them.
- A sidebar shows your categories; click through to see the items in each.
- Every item has a **completion status** (tap the circle).
- Categories can be **renamed** (double-click), **merged**, or **deleted** (⋯ menu).

## How classification works

- **Built-in classifier** (default): a large dictionary (fruits/groceries → Shopping, dev & office vocabulary → Work, finance, travel, health, home, calls…), word stemming ("oranges" matches "orange"), similarity to notes already in your categories — **and it learns**: every time you re-file a note via the toast, those words are remembered for that category. Free, offline, instant, gets smarter with use.
- **Claude-powered** (optional): open *settings* and paste an Anthropic API key. Notes are then classified by Claude (`claude-haiku-4-5`), which picks an existing category or invents a fitting new one. The key is stored only in your browser's localStorage and sent only to Anthropic's API.

## Storage

Notes live in your browser (`localStorage`) — private to your device, no account, no server. This repo holds only the code; GitHub Pages serves it.

## Stack

One `index.html`. No build, no dependencies, no framework.
