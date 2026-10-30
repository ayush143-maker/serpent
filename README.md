# serpent

**SERPENT** is a browser-based take on the classic Snake game. The project consists of the single HTML page `index.html`, which contains a play area, current and best scores, pause and play controls, and on-screen guidance for keyboard and touch-style movement. Follow the on-screen guidance to control the snake.

## Play locally

No package installation is needed. Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>. To review a change, edit `index.html`, reload the page, and use its on-screen guidance and controls.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`. Keep the score displays and controls consistent with the guidance shown to players.
- Inspect `index.html` for the existing style rules before changing colors, typography, or layout; no separate stylesheet is listed in the project files.
- The page links to externally hosted Inter and Space Grotesk font stylesheets. Preserve those links if you want to retain the current font choices.
- Before moving or renaming anything, check `index.html` for local `href` and `src` references and keep their relative paths valid. No separate local asset files are listed.