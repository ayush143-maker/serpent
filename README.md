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

## Accessibility review checklist

These are future review checks, not claims of accessibility or verified results. Record issues and any follow-up separately.

- [ ] Use only the keyboard to reach every interactive control, including pause and play, and to operate the game using the movement guidance shown on the page. Check that the order is understandable and that keyboard use does not get trapped.
- [ ] Tab through the page and check that each focused control has a clearly visible focus indicator, including against the play area and surrounding backgrounds.
- [ ] Inspect the pause and play controls and any other interactive elements in `index.html`. Check that their accessible names describe their actions and that instructions identify the keys or input needed to play.
- [ ] Check text and control contrast against their backgrounds, including score values, instructions, and text that appears during play. Review all relevant states, not just the initial screen.
- [ ] If `index.html` includes images, check that informative images have useful text alternatives and decorative images are not announced as meaningful content. If there are no images, note that this check is not applicable.
- [ ] If the game uses animation or other motion effects, check how it behaves with the operating system's reduced-motion preference enabled. Consider reducing nonessential motion while keeping gameplay and state changes understandable.

## Personalize the page

- Edit the visible title, instructions, and other page copy in `index.html`. Keep the score displays and controls consistent with the guidance shown to players.
- Inspect `index.html` for the existing style rules before changing colors, typography, or layout; no separate stylesheet is listed in the project files.
- The page links to externally hosted Inter and Space Grotesk font stylesheets. Preserve those links if you want to retain the current font choices.
- Before moving or renaming anything, check `index.html` for local `href` and `src` references and keep their relative paths valid. No separate local asset files are listed.