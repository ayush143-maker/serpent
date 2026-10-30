# serpent

**SERPENT** is a canvas-based Snake game. Steer the snake to eat food, grow, and increase your score; hitting a wall or your own body ends the run. Filling the board also produces a game-over screen.

## Play locally

No package installation is needed. Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Controls and scoring

Use the arrow keys or WASD to steer. On touch screens, swipe to choose a direction; the swipe must exceed 16 pixels. A tap during play pauses. Space or Enter starts, resumes, pauses, or restarts via the primary action; P toggles pause/resume, and R restarts after game over. The on-screen Pause button is available during a run. Direction inputs queue up to three turns; repeated directions and direct reversals are rejected.

Eating adds one point and speeds up movement. The interval starts at 150 ms, decreases by 2.6 ms per food, and bottoms out at 70 ms. The HUD displays the current and best scores. The board adapts to the viewport and clamps its grid to 11–28 columns and rows; canvas pixel scaling is capped at device-pixel ratio 3.

The game pauses when the page becomes hidden or the window loses focus. An overlay can be clicked or tapped to start, resume, or restart.

## Persistence and browser features

Only the best score is saved, under `serpent.best.v1` in localStorage. The current run’s score is not persisted. If localStorage access fails, the game uses an in-memory fallback, so that best score lasts only for the current page session in that case.

Game visuals are drawn on canvas. Sound effects are synthesized with the Web Audio API; eating or dying can also trigger `navigator.vibrate` where available. Inter and Space Grotesk load from jsDelivr’s Fontsource CDN, so those fonts require network access. No separate build step or local asset directory is documented. Check keyboard and touch controls, pause behavior, score handling, and layout in the browser when changing the page.