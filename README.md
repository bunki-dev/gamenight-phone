# Game Night Camera (phone page)

The page phones open to play Dodge Run with their body. It must be served over **https**
(phones only allow the camera on secure pages).

## Put it online with GitHub Pages (free)
1. On github.com create a public repository, e.g. `gamenight-phone`.
2. Upload `index.html` from this folder and commit.
3. Repository **Settings > Pages**: Source = *Deploy from a branch*, Branch = `main`, folder `/ (root)`, Save.
4. After a minute it's live at `https://YOUR-NAME.github.io/gamenight-phone/`.
5. Put that address in the TV app's `js/config.js` (`PHONE_URL`) so the TV shows it.

Tip: `https://YOUR-NAME.github.io/gamenight-phone/?room=ABCDE` pre-fills the room code.

## How tracking works
- Calibrate: step out of view (it learns the empty room), then stand in the middle (it learns you).
- Your silhouette is compared with the empty room ~20 times a second at low resolution.
- Step left/right = change lane, jump (feet leave the floor) = jump, squat = duck,
  both hands up for 0.7 s = the Join / Start button.
- Works best with steady light, a background that doesn't move, and your whole body in view.
- "⋯" has Swap L/R (if lanes feel backwards) and three sensitivity levels.

`tools/test-broker.js` is only for testing on a computer.
