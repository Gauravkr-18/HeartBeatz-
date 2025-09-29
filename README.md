# HeartBeatz — Static Music Web UI

A small static music player UI built with HTML, CSS and vanilla JavaScript. The project is a single-page layout that mimics a streaming app dashboard with a sidebar, header, scrollable music sections, and a floating music player.

This README documents the project's structure, how to run it locally, known issues found while analyzing the code, and recommended next steps.

## Project snapshot

- Technology: HTML, CSS, JavaScript (no build step)
- Files: single static site; audio and images are stored alongside the pages
- Main entry: `index.html`

## Features

- Sidebar navigation (Home, New Releases, Top Charts, Likes, Playlists, Albums, Following)
- Header with search and user profile link that sends user to `login.html`
- Several horizontally-scrollable music carousels: Recently Played, Made Just for You, Trending Now, New Releases
- Click a music card to update the player artwork and play the associated audio file
- Simple play/pause and seek UI in the floating player

## Project files (important)

- `index.html` — main UI and markup
- `styles.css` — presentation and responsive rules
- `scripts.js` — navigation, audio player logic and event handling
- `*.mp3`, `*.jpg`, `*.png` — media assets used by the UI
- `login.html` — target of the logout/user link

## How to run (local development)

Because this is a static site you can run it in two ways:

1) Open directly in a browser

   - Double-click `index.html` or open it using your browser's File > Open.
   - Note: some browsers restrict playing local media over `file://` in specific situations. If audio does not play, use the second method below.

2) Serve over a simple local HTTP server (recommended)

   - If you have Python installed, open a terminal in the project folder and run:

   ```powershell
   python -m http.server 8000
   ```

   - Then open http://localhost:8000 in your browser.

## Quick usage

- Click items in the left menu to switch sections (Home / New Releases / Top Charts).
- Click any card (tile) with an image to load and play the associated audio file.
- Use the play/pause button and the seekbar to control playback.
- Click the profile/log out link to go to `login.html`.

