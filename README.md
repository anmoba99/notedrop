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

- **Built-in classifier** (default): keyword matching + similarity to notes already in your categories. Free, offline, instant.
- **Claude-powered** (optional): open *settings* and paste an Anthropic API key. Notes are then classified by Claude (`claude-opus-4-8`), which picks an existing category or invents a fitting new one. The key is stored only in your browser's localStorage and sent only to Anthropic's API.

## Storage

Notes live in your browser (`localStorage`) — private to your device, no account, no server. This repo holds only the code; GitHub Pages serves it.

## Stack

One `index.html`. No build, no dependencies, no framework.
