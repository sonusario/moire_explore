# Moiré Exploré

A single-file web app for exploring moiré patterns. Open `index.html` in any modern browser — no build step, no dependencies.

Two patterns, **A** (bottom) and **B** (top), are layered on top of each other. Move, rotate, scale or animate one of them and watch the interference fringes appear.

## Patterns

Each layer can use a preset or a pattern you draw yourself:

- Parallel lines, square grid, concentric circles, radial spokes, spiral, zone plate
- Dot grid, hexagonal dots, checkerboard, wavy lines, random dots (Glass patterns)
- **Hand drawn** — paint a tile (or a single image) with pen, line, rectangle and ellipse tools, with eraser, mirror symmetry, seamless edge wrapping, invert and undo. The canvas updates live as you draw.

Every layer has its own colour and opacity (10 %–100 %) for the opaque parts, plus a visibility toggle. Under **Composite** you can pick the background colour and blend mode (normal, multiply, screen, difference…) and swap A and B.

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

- **Presets:** spin, sway, slide, orbit, figure eight, breathe (scale pulse), orbit + spin.
- **Drawn path / circuit:** choose the **Path** tool and drag on the canvas. The layer's centre then follows that path, either looping as a circuit or going back and forth. Rotation along the path can be set with:
  - *Turn with the path direction*: the pattern turns to follow the path,
  - *Spin per lap*: a steady extra rotation each lap,
  - *Keyframes*: set rotation angles at points along the lap; angles in between are interpolated.
- **Counter-move:** the other layer makes the opposite movement.

## Keyboard

`Space` play/pause · `H` hide panel · `G` guides · `1`/`2` pick layer · `M`/`R`/`P` move/rotate/path tool · `[` `]` rotate (Shift = fine) · arrows move (Shift = ×10) · `+`/`-` scale · `0` reset · `Esc` close editor · `Ctrl+Z` undo in the editor.

**Save PNG** (under *View*) downloads the current frame.
