# Anime Finder (Jikan API)

A lightweight web UI to search anime data via the public [Jikan API](https://jikan.moe/). Built with plain HTML, CSS, and JavaScript—no build tools required.

## Features
- Search anime titles and view cover art, score, year, episodes, and synopsis.
- Open results directly on MyAnimeList.
- Client-side score sorting (high→low or low→high).
- Responsive, dark-themed layout.

## Prerequisites
- A modern web browser (Chrome, Firefox, Edge, Safari).
- Internet connection (to call the Jikan API and load cover images).

## Getting Started
1) Clone or download this repository to your machine.  
2) Open `index.html` in your browser (double-click or right-click → Open With).  
3) Type an anime title (e.g., "One Piece") and press Search.  
4) Adjust sort order if desired.

> No build step or package installation is needed. Everything runs in the browser.

## Project Structure
- `index.html` – page markup and search form.
- `style.css` – styling for layout, cards, and responsive design.
- `app.js` – fetches from `https://api.jikan.moe/v4/anime`, renders results, and handles sorting.

## How It Works
- The search form triggers a `fetch` request to the Jikan API with your query (`q` param).
- Results are rendered as cards using a `<template>` and populated with title, score, year, episodes, and synopsis.
- Sorting reorders cards client-side based on score.

## Notes and Limits
- The Jikan API is public and rate-limited; rapid repeated searches may get throttled.
- Images and data come from external sources (MyAnimeList via Jikan); availability depends on the upstream service.

## Troubleshooting
- **No results:** Try a different or shorter query.  
- **Network/API errors:** Check your connection; wait a moment and retry if rate-limited.  
- **Broken images:** External image hosts may be temporarily unavailable; try again later.

## Reference
- Jikan API docs: https://jikan.moe/

