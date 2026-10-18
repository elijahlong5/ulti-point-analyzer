# Mixed Point Sheet

A single-page simulator for mixed ultimate. It plays out a full game point by point, following the ABBA gender-matching pattern, with offense/defense tracking, X/Y D-lines and a running score.

## Use it

Open `index.html` in a browser. There is no build step and no dependencies (fonts load from Google Fonts).

To host it, turn on GitHub Pages for this repo (Settings → Pages → deploy from the `main` branch, root folder).

## How it works

- **Setup:** choose whether you start on offense or defense, whether the first point is woman or man matching, and what the game is played to (default 15).
- **Gender pattern:** points run W2, M1, M2, W1 and repeat (or M2, W1, W2, M1 if you start man matching), regardless of who scores.
- **Scoring:** every point is a hold by default. Tap **Break** on a point to make the defense score. A hold flips offense/defense for the next point; a break keeps the same side.
- **Lines:** O points use the O line. D points alternate X, Y, X, Y. Tap O, X or Y on any point to override it, and tap the selected override again (or "Reset lines") to return to automatic.
- **Summary:** the scoreboard shows the final score, breaks for and against, and W/M point counts. The "Points by line" table splits W and M points for O, X and Y.

Settings, breaks and line overrides are saved in the browser's local storage.
