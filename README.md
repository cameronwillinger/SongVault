# SongVault Mobile

A private, offline-first song organizer for iPhone (and any modern phone browser). Install it to the Home Screen from Safari and it runs like an app.

- **No account, no server, no tracking.** Everything is stored on your device (IndexedDB). This repository contains only the app code; it holds no user data.
- Edit every field of a song: title, artist/pen name, album, key, BPM, genre, lyrics, meaning, notes, streaming links, music-video plan, artwork, audio/voice memos, versions, checklist, custom fields, tags.
- One-tap **New idea** capture (with voice recording).
- **Lyric Desk**, section tools, a completeness meter, a "What's missing" list, and Grok prompt boxes that work by copy/paste (no API key).
- **Sync with the SongVault desktop app** by exporting and importing a "SongVault Sync File" (`.songvault.zip`). Merges are two-way; the newest edit wins per field, nothing is deleted unless you deleted it, and conflicts are kept as a "conflict copy" in the song's version history.

See [SETUP-IPHONE.md](SETUP-IPHONE.md) for install and sync steps.

## Files
`index.html` (the whole app), `manifest.webmanifest`, `sw.js` (offline cache), icons.

Host it on any static HTTPS host (this repo is served with GitHub Pages at https://cameronwillinger.github.io/SongVault/). HTTPS is required for the service worker, microphone, and camera.
