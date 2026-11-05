# Merge Drop

A mobile-friendly browser tile-merging game.

## Play
Open `index.html` in a browser.

## Rules
- Tap a column to drop the next tile.
- Orthogonally connected tiles of the same value merge into one tile whose value is their sum.
- The resulting tile is checked again for adjacent matches, enabling chain reactions.
- The game ends when the top row is full.

## Layout
- `index.html` — current 4-column × 7-row game.
- `archive/merge_drop_prototype_7x7.html` — original 7×7 prototype.

No build tools or dependencies required.

## Version 0.3

The current build resolves chain reactions with gravity: after each merge, tiles settle downward before the board checks for another connected match. This allows a falling tile to create a new merge.
