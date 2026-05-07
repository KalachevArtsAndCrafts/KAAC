# Component: Player

**File:** `src/player.js`

## Responsibility

- Audio playback of individual notes and melodies
- Uses `ion.sound` (vendor) as audio engine
- Loads sounds from `/sounds/` folder

## Sound Assets

- Notes: A1–G3 (`.mp3`, muted variants ` m.mp3`)
- FX: `bell_ring`, `snap` (`.mp3`, `.aac`, `.ogg`)

## Key Relations

- Called by `controller.js`
- Sequencing timed by `ticker.js`
