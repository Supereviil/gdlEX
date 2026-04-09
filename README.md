# gdlEX
## A practical companion for `gallery-dl` power users

`gdlEX` isn’t trying to replace `gallery-dl`. It sits on top of it and handles the parts that get annoying when you’re running downloads every day:  queue prep, repeatable settings, safer starts/stops, and a cleaner workflow overall.

If you already use `gallery-dl`, this fills in the gaps and makes the whole process easier to manage on Windows.

---

## Why gdlEX exists

`gallery-dl` is great at what it does, but running it repeatedly can turn into a pile of command lines, half‑finished queues, and folders that need cleanup.

`gdlEX` helps with the parts around the downloader:

- preparing and sanitizing URL lists  
- keeping your settings consistent between runs  
- pausing, stopping, and resuming cleanly  
- organizing output in a predictable way  
- saving receipts/logs so you can see what happened later  

It’s the “operator layer” that sits above the CLI.

---

## What gdlEX adds on top of a basic GUI

### 1) Workflow continuity
- Restores your last queue and output folder  
- Single‑URL and multi‑URL queue modes  
- Queue cleanup (dedupe, comment stripping, invalid URL removal)  
- Pause/resume support using full process‑tree suspension  

### 2) Safer operation
- Controlled start/stop/pause/resume flow  
- More reliable shutdown for long sessions  
- Optional tray mode if you want it running in the background  

### 3) Post‑download cleanup
- Rename/sanitization options:
  - remove emojis, punctuation, spaces, custom strings  
  - trim long filenames  
  - swap extensions  
- Optional CBZ creation (skips single‑image folders)  
- Optional session log (`gdlEX_session_*.txt`)  
- End‑of‑run summary with file‑type breakdown  

### 4) Auth and extractor setup
- Cookie extraction (browser or file)  
- OAuth/API key fields  
- Proxy, retries, timeout, user‑agent, and other network controls  

### 5) Consistent configuration
- All settings saved in `gdlEX.ini`  
- Optional visual themes (Windows, Carbon, Slate, Windows 11 styles)  
- No more re‑typing CLI arguments or digging through terminal history  

---

## A typical run looks like this

1. Paste or build your URL list  
2. Sanitize the queue  
3. Adjust your settings  
4. Run with live output  
5. Let gdlEX handle renaming/CBZ/archive cleanup  
6. Review the session receipt if you want a record  

It turns one‑off commands into a repeatable workflow.

---

## Who this is for

- People downloading from multiple sites and managing big queues  
- Anyone who wants consistent, clean filenames  
- Comics/manga users who want folder‑to‑CBZ automation  
- Anyone who uses `gallery-dl` often and wants fewer mistakes and less friction  

---

## Current release state

**Version:** `0.0.9.9 alpha` — the last alpha before the beta cycle.

This build focuses on hardening:

- standardized naming (`gdlEX`, `gdlEX.ini`, `gdlEX_session_*.txt`)  
- safer shutdown behavior  
- improved tray handling  
- safer post‑processing in threaded runs  

Features intentionally locked until beta:

- watch‑folder automation  
- scheduled runs  
- completion actions  
- webhook notifications  

---

## Requirements

- Windows 10/11  
- `gallery-dl.exe` in the same folder as the gdlEX executable  

Optional:
- `yt-dlp` for fallback mode  
- cookies/auth for protected sources  

---

## Important note

`gdlEX` depends on `gallery-dl`.  
It doesn’t bundle it, fork it, or replace it — it just makes it easier to use.
