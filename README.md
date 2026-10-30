# serpent

**SERPENT** is a browser-based take on the classic Snake game. The project consists of the single HTML page `index.html`, which contains a play area, current and best scores, pause and play controls, and on-screen guidance for keyboard and touch-style movement. Follow the on-screen guidance to control the snake.

## Play locally

No package installation is needed. Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Manual review checklist

These are actions to perform, not verified results. Record findings separately; this README does not report that the checks have passed.

- [ ] Open `index.html` and confirm the page loads, including its play area and score displays.
- [ ] Inspect `index.html` for image, media, stylesheet, script, and font references. Check that each referenced path or URL resolves. The listed project files include only `index.html` and this README; the page references externally hosted Inter and Space Grotesk font stylesheets.
- [ ] Follow the on-screen guidance to try keyboard and touch-style movement. Try the pause and play controls, and observe how the current and best scores are displayed.
- [ ] Inspect the game at a narrow viewport and a wide viewport. Check that the play area, score displays, controls, and instructions remain visible and usable; note overflow or layout issues.
- [ ] After a change, reload the page and repeat the checks affected by that change.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`. Keep the score displays and controls consistent with the guidance shown to players.
- Inspect `index.html` for the existing style rules before changing colors, typography, or layout; no separate stylesheet is listed in the project files.
- The page links to externally hosted Inter and Space Grotesk font stylesheets. Preserve those links if you want to retain the current font choices.
- Before moving or renaming anything, check `index.html` for local `href` and `src` references and keep their relative paths valid. No separate local asset files are listed.