# Merge Drop

A mobile-friendly browser tile-merging game.

## Play
Open `index.html` in a browser.

## Rules
- Tap a column to drop the next tile, or swipe a tile left or right into an adjacent empty space.
- Each drop or swipe uses one move; a swipe is followed by gravity and merge resolution.
- Orthogonally connected tiles of the same value merge into one tile whose value is their sum.
- The resulting tile is checked again for adjacent matches, enabling chain reactions.
- Complete each level's goals before the move limit runs out. Goals include building target tiles, collecting exact-value tiles, clearing ice with an adjacent merge, and collecting gems by merging an equal-value tile into the marked block.
- Later levels combine goals and use different starting boards.
- From level 10, ice cracks after one adjacent merge and breaks after the second. At level 20, gem stages require two gems; the second gem tile arrives in the next-tile preview after several moves.
- Any tile reaching the top row ends the level. Retry the same level; cleared levels stay unlocked.

## Layout
- `index.html` — current 4-column × 5-row game.
- `archive/merge_drop_prototype_7x7.html` — original 7×7 prototype.

The next tile has a chance to match a larger value already on the board, giving you a setup opportunity when small drops stop helping. Ten handcrafted levels introduce goals gradually; later stages remix those board layouts with a gentle move-budget increase and carry forward unlocked mechanics.

No build tools or dependencies required.

## Version 0.3

The current build resolves chain reactions with gravity: after each merge, tiles settle downward before the board checks for another connected match. This allows a falling tile to create a new merge. Levels combine target, collection, ice-clear, and gem-collection goals with move limits.
