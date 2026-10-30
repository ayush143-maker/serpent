# serpent

**SERPENT** is a browser-based take on the classic Snake game. The project centers on `index.html`, which contains the play area, current and best scores, pause and play controls, and on-screen guidance for keyboard and touch-style movement. Follow the on-screen guidance to control the snake.

## Play locally

No package installation is needed. Open `index.html` in a browser, or start a local server from the project folder:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Configuration and data handling

The supplied project-file list contains `index.html` and `README.md`; it does not include a documented environment template, separate configuration file, or backend setup. The page is delivered to the browser, so anything placed in its markup or scripts is public—not a place for passwords, API keys, tokens, or other secrets.

The page displays current and best scores, but this README does not establish whether scores are kept only during play or persisted in browser storage. Check `index.html` before describing or changing data storage, and avoid adding personal or sensitive information to game data. The page also requests Inter and Space Grotesk font stylesheets from jsDelivr; those external requests are a dependency to consider when reviewing privacy and offline behavior.

## Browser and platform reliability checklist

These are review steps, not verified results. No browser or device compatibility testing is reported here. Record findings separately, including the browser and version, device or viewport, and any issues found.

- [ ] Test in current stable browsers relevant to the intended audience and this browser-based HTML project. Consider Chromium-based Chrome or Edge, Firefox, and Safari; include mobile Safari on iOS and Chrome on Android when mobile use is in scope.
- [ ] In each browser, open the game and check that the play area, current and best scores, pause and play controls, and on-screen input guidance appear and work as expected.
- [ ] Open the developer console and review for JavaScript errors, warnings, and failed resource loads. Inspect the network panel for failed requests, unexpected status codes, or blocked resources. Record what you find; do not treat an uninvestigated message as harmless.
- [ ] Inspect `index.html` for local `src` and `href` references. Confirm every referenced local file exists and its path resolves both when opened directly and when served from the project folder. The supplied project-file list includes `index.html` and `README.md`, but no separate local assets.
- [ ] Review remote requests. The supplied link inventory lists jsDelivr font stylesheets for Inter (400, 600, 800) and Space Grotesk (500, 700). Confirm the references in `index.html` are intentional and load successfully when online. If a request fails or is blocked, check that fallback typography remains legible and the game remains usable.
- [ ] Compare narrow mobile and wide desktop viewports. Check for horizontal overflow, clipped content, and controls or instructions that become difficult to see or use. If possible, repeat on actual mobile devices, not only resized desktop windows.
- [ ] After changing markup, styles, or asset references, repeat the checks affected by the change.

## Gameplay and layout review checklist

These are manual checks to perform, not reported results.

- [ ] Check the play area, score displays, and controls.
- [ ] Follow the on-screen guidance to try keyboard and touch-style movement. Try pause and play, and observe the current and best score displays.
- [ ] Check that instructions, scores, controls, and the play area remain visible and usable at narrow and wide viewport sizes.

## Accessibility review checklist

These are review checks, not claims of accessibility or verified results.

- [ ] Use only the keyboard to reach and operate controls and to play using the on-screen movement guidance. Check that focus order is understandable and keyboard use does not get trapped.
- [ ] Check that focused controls have a clearly visible focus indicator.
- [ ] Check that interactive elements have accessible names describing their actions and that instructions identify the input needed to play.
- [ ] Review text and control contrast against their backgrounds, including scores and instructions, in relevant game states.
- [ ] If `index.html` references images, check that informative images have useful text alternatives and decorative images are not announced as meaningful content. If there are no images, this check is not applicable.
- [ ] If the game uses motion effects, check behavior with the operating system’s reduced-motion preference enabled and consider reducing nonessential motion.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`. Keep the score displays and controls consistent with the guidance shown to players.
- Inspect the existing style rules in `index.html` before changing colors, typography, or layout; no separate stylesheet is listed in the supplied project files.
- The supplied external font links are for Inter and Space Grotesk. Keep them if those choices are intentional; otherwise update the references and check fallback typography.
- Before moving, renaming, or removing assets, inspect `index.html` for local `href` and `src` references and confirm the assets are unused.