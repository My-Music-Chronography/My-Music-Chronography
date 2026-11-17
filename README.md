# My Music Chronography

Catalog your music: albums, LPs, EPs and singles, with artists, years, genres, labels, covers and full tracklists.

- **Add New Album**: pick Album, LP, EP or Single, then look it up on MusicBrainz (album, artist, or both) and tap a result to fill everything in, or type it in yourself
- **Library**: search titles, artists, genres and song names; filter by type; sort by date added, title, artist, year, length, type or genre
- **Artists**: every artist with their releases; open one to see them grouped by type, or rename them everywhere at once
- **Data**: collection stats, and Backup / Import

Album details come from [MusicBrainz](https://musicbrainz.org) and covers from the [Cover Art Archive](https://coverartarchive.org). Both are free and need no account or key.

Everything is stored in your browser on this device. Use **Data → Save Backup** to keep a copy, and import it on another device or browser.

## Opening animation

Each time the app opens, it picks up from the phone's own launch screen (the icon) and plays a short record-stack animation into the name. Tap to skip.

## Works offline

After the first visit, the service worker (`sw.js`) keeps a copy of the app, so it opens with no connection. Covers are saved inside the app when you add an album. Looking albums up needs a connection.
It can be installed to your home screen (browser menu → **Install app** / **Add to Home Screen**).

## Files

| File | What it is |
|---|---|
| `index.html` | the app |
| `sw.js` | service worker: offline copy of the app |
| `manifest.webmanifest` | name, colours and icons for installing |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | app icons |
| `.nojekyll` | tells GitHub Pages to serve the files as they are |

## Updating

When you upload a new `index.html`, also change `VERSION` at the top of `sw.js` (for example `chronography-v2`), so installed copies fetch the new files.
