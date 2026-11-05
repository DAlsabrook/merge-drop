# Merge Drop

A mobile-friendly browser tile-merging game.

## Play
Open `index.html` in a browser.

## Rules
- Tap a column to drop the next tile, or swipe a tile left or right into an adjacent empty space.
- Each drop or swipe uses one move; a swipe is followed by gravity and merge resolution.
- Orthogonally connected tiles of the same value merge into one tile whose value is their sum.
- The resulting tile is checked again for adjacent matches, enabling chain reactions.
- Clear each level's target tile before the move limit runs out.
- The run ends if any tile reaches the top row or you miss the target within the move limit.
- Later levels raise the target tile and give you a limited number of drops.

## Layout
- `index.html` — current 4-column × 7-row game.
- `archive/merge_drop_prototype_7x7.html` — original 7×7 prototype.

The next tile has a chance to match a larger value already on the board, giving you a setup opportunity when small drops stop helping.

No build tools or dependencies required.

## Version 0.3

The current build resolves chain reactions with gravity: after each merge, tiles settle downward before the board checks for another connected match. This allows a falling tile to create a new merge. Levels add a target tile and a limited drop budget.
