# Moiré Exploré

**Live:** [https://sonusario.github.io/moire_explore/](https://sonusario.github.io/moire_explore/)

A single-file web app for exploring moiré patterns. Open `index.html` in any modern browser — no build step, no dependencies.

Two patterns, **A** and **B**, are layered on top of each other. Move, rotate, scale or animate one of them and watch the interference fringes appear. Not sure where to start? Pick something from **Try a recipe** at the top of the panel.

## Patterns

Each layer can use a preset or a pattern you draw yourself:

- Parallel lines, square grid, concentric circles, radial spokes, spiral, zone plate
- Dot grid, hexagonal dots, checkerboard, wavy lines, random dots (Glass patterns)
- **Scanimation** — patterns that turn into an animation when one slides or spins past the other:
  - *Scanimation frames* interlaces 2–12 frames of a spinning star, bouncing ball, beating heart, orbiting moons or travelling wave. Pair it with a *Scanimation barrier* on the other layer and use the **Drift** animation.
  - *Radial scanimation frames* interlaces frames by angle (ripples, pinwheel, circling dots). Pair it with a *Radial scanimation barrier*, keep both centred, and use **Spin**.
  - Frames and Slit settings stay matched between a frames layer and its barrier automatically.
- **Hand drawn** — paint a tile (or a single image) with pen, line, rectangle and ellipse tools, with eraser, mirror symmetry, seamless edge wrapping, invert and undo. The canvas updates live as you draw. The drawing panel has an **A / B** switch, so you can work on either layer's drawing, and **Copy A → B** / **Copy B → A** buttons. Each layer keeps its own undo history.

Every layer has its own colour and opacity (10 %–100 %) for the opaque parts, plus a visibility toggle. Under **Composite** you can pick the background colour and blend mode (Normal by default; also multiply, screen, difference…) and choose which layer is on top. A and B keep their own settings when you change the stacking.

## Moving the patterns

Choose which layer moves (A or B), then on the canvas:

| Action | Effect |
| --- | --- |
| Drag | Move |
| Shift + drag, right-drag, or the **Rotate** tool | Rotate around the layer's centre |
| Mouse wheel (Shift for fine steps) | Rotate |
| Ctrl + wheel, or pinch | Scale |
| Two-finger drag / twist | Move / rotate on touch screens |

Rotation, scale and offset can also be typed in exactly.

## Animation

- **Presets:** spin, drift (steady glide in any direction), sway, slide, orbit, figure eight, breathe (scale pulse), orbit + spin. Changing a rate, period or lap time while it plays changes the speed smoothly, without the pattern jumping.
- **Drawn path / circuit:** choose the **Path** tool and drag on the canvas. The layer's centre then follows that path, either looping as a circuit or going back and forth. Rotation along the path can be set with:
  - *Turn with the path direction*: the pattern turns to follow the path,
  - *Spin per lap*: a steady extra rotation each lap,
  - *Keyframes*: set rotation angles at points along the lap; angles in between are interpolated.
- **Counter-move:** the other layer makes the opposite movement.

## Keyboard

`Space` play/pause · `H` hide panel · `G` guides · `1`/`2` pick layer · `M`/`R`/`P` move/rotate/path tool · `[` `]` rotate (Shift = fine) · arrows move (Shift = ×10) · `+`/`-` scale · `0` reset · `Esc` close editor · `Ctrl+Z` undo in the editor.

**Save PNG** (under *View*) downloads the current frame.
