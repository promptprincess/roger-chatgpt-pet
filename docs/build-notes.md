# Build notes

Roger started as a full-body character reference. The adaptation uses a muted gray body, an oversized head, half-lidded expressions, and an exaggerated facepalm so he reads as Roger at desktop-pet scale. The original pack provided nine motion rows and sixteen look poses.

## Size pass

The original idle pose occupied about 161 pixels vertically inside each 208-pixel cell. The size pass applied a common 1.15× scale to all 73 poses. An example idle frame grew to about 186 pixels high. The frame grid stayed fixed. The jump’s vertical travel was shortened so his head could clear the frame edge and his feet could return to the standing baseline.

[Original and resized poses](../previews/size-comparison.png) · [Idle to jump to idle](../previews/idle-jump-idle.gif)

## Outline pass

The first enlargement made the pale fringe around the head, fingers, and feet easier to see. The outline pass tightened partial transparency and added a subtle darker contour just inside the silhouette. We compared light and dark backgrounds and kept the updated geometry and frame order. The desktop WebP preserves the resulting pixels losslessly.

[Outline comparison](../previews/edge-comparison.png)

## Verification

Both distribution atlases passed the ChatGPT Pets sprite-sheet validator. The desktop WebP decodes pixel for pixel to the cleaned artwork that was verified on the active Roger pet. The web PNG was checked as an exact extract of the first nine rows and passed v1 structural validation. A browser upload and the terminal and Windows renderers were outside this verification.

The directional continuity check flagged several relatively sharp transitions. The most noticeable numeric warning is the wrap from 337.5° to 0°, which was already present before the outline pass. The [look-loop preview](../previews/look-loop.gif) and [continuity measurements](look-continuity.json) show what was measured.

[Packaged atlas validation](validation.json)
