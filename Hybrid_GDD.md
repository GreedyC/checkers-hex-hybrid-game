# Hybrid GDD

## 1. Overview
This game is a two-player abstract strategy hybrid that combines Hex-style connection play with Checkers-style tactical jump capture. The game is built around placement-driven turns, mandatory capture when available, and a sole win condition based on connecting opposite sides of the board.

The experience is intended to feel strategic, positional, and pressure-driven. Players build toward a connection while defending their own structure and using capture threats to disrupt the opponent.

## 2. Board
The board is a tilted rhombus-shaped hex grid with 8 cells per side. It is not a square board and is not modeled as a masked larger board.

## 3. Core Objective
A player wins by creating a connected path of their pieces between any two opposite sides of the board.

## 4. Turn Structure
- Players alternate turns.
- The game is placement-driven, but capture has priority when a legal capture is available.
- At the start of a player’s turn, check whether that player has a legal capture available.
- If a legal capture is available, the player must perform a capture instead of placing a new piece.
- If no legal capture is available, the player places one piece on an empty cell.
- A placement may itself create a legal capture for the active player.
- If a placement creates a legal capture, that capture must be resolved immediately during the same turn.
- If a capture chain is available after the first capture, it is also mandatory.
- The turn ends only when no further mandatory captures remain.
- If a connection win is completed at any point, the game ends immediately.

## 5. Placement and Capture Timing
Capture can arise in two ways:
1. An existing piece may already have a legal capture available at the start of the active player’s turn.
2. The newly placed piece may immediately create a legal jump capture.

In either case, if a legal capture exists for the active player, that capture is mandatory and must be resolved. The player may choose among multiple legal captures, but once a capture sequence begins, any further legal captures in that chain must be taken until the chain ends.

Immediate capture resolution after placement is the main emergent rule of the hybrid. It exists because Checkers-style capture needed a timing rule inside a Hex-style placement game.

## 6. Placement Rules
- A piece may be placed only on an empty legal cell.
- Placement is the only primary action in the game.
- Placement may create tactical pressure or a capture opportunity.
- Placement may also be used for baiting, blocking, or separating opponent structures.

## 7. Capture Rules
Capture follows Checkers-style jump logic.

### Capture procedure
- A piece captures by jumping over an adjacent enemy piece.
- The landing space beyond the captured piece must be empty.
- Capture is mandatory if a legal capture exists.
- Capture chains are allowed and mandatory if available.
- Capture is diagonal in nature and does not use sideways capture.

### Capture axes
Capture is legal only on the two diagonal axes of the hex grid:
- NE ↔ SW
- NW ↔ SE

E ↔ W is not a capture axis.

All 6 hex directions still matter for adjacency and connection path logic.

## 8. Win Condition
A player wins immediately when a connected path of their pieces reaches between any two opposite sides of the board.

## 9. Strategic Identity
This hybrid is not a pure capture game and not a pure placement-only connection game. Its identity comes from the combination of:
- Hex-style placement and flexible connection
- Checkers-style tactical capture
- Mandatory capture as a rule constraint, not a strategic ban on baiting or blocking

Players may intentionally place pieces to bait, block, separate, or create pressure. These are valid strategic choices. The only hard rule is that if a legal capture exists for the active player, it must be taken.

