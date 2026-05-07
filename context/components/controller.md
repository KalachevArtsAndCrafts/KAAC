# Component: Controller

**Files:** `src/controller.js`, `src/controller-view.js`

## Responsibility

- Core application logic
- Bridges user interaction (view) with playback (player)
- Manages app state

## Key Relations

- Receives events from `controller-view.js`
- Delegates audio to `player.js`
- Updates `viewer/index.js`
