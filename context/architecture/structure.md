# Architecture

## Folder Structure

```
KAAC/
  src/                  # source code
    harp-view.js        # entry point
    controller.js       # app controller logic
    controller-view.js  # controller + view binding
    player.js           # audio/melody player
    ticker.js           # timing / sequencer
    viewer/             # visual rendering
      index.js
      notes-viewer.css
    helpers/            # utility functions
    vendor/             # third-party libs (ion.sound)
  dist/                 # built output (Parcel)
  sounds/               # audio assets (.mp3, .aac, .ogg)
  css/                  # global styles
  img/                  # images
  doc/                  # legacy documentation
  context/              # llm-wiki (this folder)
```

## Data Flow

```
User Click
  → controller-view.js
    → controller.js
      → player.js  (plays note via ion.sound)
      → viewer/    (updates visual state)
        → ticker.js (sequence timing)
```

## Build

- Bundler: Parcel 1.x
- Input:  `src/harp-view.js`
- Output: `dist/harp-view.js`
