# Roger sprite atlas

| Property | Desktop v2 | Web v1 |
| --- | --- | --- |
| File | [spritesheet.webp](../roger/spritesheet.webp) | [roger-web-v1.png](../web/roger-web-v1.png) |
| Format | Lossless WebP, RGBA | PNG, RGBA |
| Dimensions | 1536 × 2288 | 1536 × 1872 |
| Layout | 8 columns × 11 rows | 8 columns × 9 rows |
| Cell size | 192 × 208 | 192 × 208 |
| Populated cells | 73 | 57 |
| Unused cells | 15 | 15 |

Frames run from left to right, starting in the first cell of each row. Unused cells are fully transparent. Column and row indices start at zero. The top-left pixel of a cell is `(column × 192, row × 208)`.

| Row | State | Frames | Roger’s motion |
| --- | --- | --- | --- |
| 0 | Idle | 6 | Relaxed pose with a blink |
| 1 | Run right | 8 | Right-facing stride |
| 2 | Run left | 8 | Left-facing stride |
| 3 | Wave | 4 | Raises and lowers one hand |
| 4 | Jump | 5 | Crouches, lifts off, and lands |
| 5 | Failed | 8 | Facepalm reaction |
| 6 | Waiting | 6 | Expectant hand and body poses |
| 7 | Working | 6 | Focused thinking poses |
| 8 | Review | 6 | Head and eye movements as he checks his work |
| 9 | Look directions | 8 | 000°, 22.5°, 45°, 67.5°, 90°, 112.5°, 135°, 157.5° |
| 10 | Look directions | 8 | 180°, 202.5°, 225°, 247.5°, 270°, 292.5°, 315°, 337.5° |

Look angles are clockwise in screen coordinates. 0° is up, 90° right, 180° down, and 270° left. The web PNG contains rows 0–8 copied pixel for pixel from the desktop artwork.

The [manifest](../roger/pet.json) sets the local ID to `roger` and declares `spriteVersionNumber` as `2`. `spritesheetPath` is relative to the manifest. Keep both files together.

[Full contact sheet](../previews/contact-sheet.png) · [Labeled look directions](../previews/look-directions.png) · [Look loop](../previews/look-loop.gif)
