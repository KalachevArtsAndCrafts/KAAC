# Project Overview

**Name:** KAAC — KalachevArtsAndCrafts  
**Package:** harp-view  
**Version:** 2.0.0  
**License:** MIT

## Description

Web-based Kora harp viewer and player. Allows visual interaction with a harp interface — plays notes on click, supports melodies and sequences.

## Entry Points

- `index.html` — main page
- `src/harp-view.js` — JS entry point (bundled via Parcel → `dist/harp-view.js`)

## Stack

- Vanilla JS (ES modules)
- Parcel bundler
- ion.sound (vendor) for audio playback
- HTTP server for local dev

## Scripts

```bash
npm run dev     # parcel watch
npm run build   # parcel build
npm start       # dev + http-server
```
