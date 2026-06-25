# Player-Facing Ruleset: Checkers + Hex Hybrid

This ruleset is the current player-facing version of the Checkers + Hex hybrid. It is written to minimize ambiguity during play.

---

# 1. Game Objective

A player wins by creating an unbroken connected path between any two opposite sides of the board.

The game ends immediately when a player completes this connection.

Captures can remove opponent pieces and disrupt a connection attempt, but eliminating all opponent pieces is not a separate win condition.

---

# 2. Players

- The game is played by **2 players**.
- Each player uses a distinct color or mark.
- Players are not assigned specific side pairs in the hybrid game.

Example:

- Player A may win by connecting top ↔ bottom or left ↔ right.
- Player B may also win by connecting top ↔ bottom or left ↔ right.
- The first player to complete any valid opposite-side connection wins.

---

# 3. Board

- The board is a tilted rhombus-shaped hex grid with **8 cells per side**.
- Every hex cell on the board is playable.
- There are no restricted cells.
- There are no dark-square-only rules.

---

# 4. Pieces

- All pieces belonging to the same player are identical.
- Pieces do not promote.
- There are no kings.
- There are no special piece types.

---

# 5. Starting State

- The board begins empty.
- No pieces are placed before the first turn.
- Players alternate turns.

---

# 6. Turn Structure

The game is placement-driven, but capture has priority when a legal capture is available.

On a player’s turn:

1. First, check whether that player has a legal capture available.
2. If a legal capture is available, the player must capture instead of placing a new piece.
3. If no legal capture is available, the player places one piece on an empty cell.
4. If that placement creates a legal capture for the active player, the capture must be resolved immediately during the same turn.
5. If additional captures become available in the same capture chain, they must also be taken.
6. The turn ends when no further legal captures remain.

---

# 7. Placement Rule

A placement is legal only if all of the following are true:

1. The chosen cell is empty.
2. The chosen cell is on the board.
3. The player places exactly one of their own pieces.
4. The player does not currently have a mandatory capture available at the start of the turn.

Pieces may be placed next to friendly pieces or opponent pieces.

---

# 8. Normal Movement Rule

There is **no normal movement** in this game.

A piece may not move from one cell to another unless it is performing a legal capture jump.

The only allowed movement is movement caused by a capture.

---

# 9. Capture Rule

A capture removes one opponent piece from the board.

A capture is legal only if all of the following are true:

1. The capturing player has one of their pieces on the board.
2. An opponent piece is adjacent along a legal capture axis.
3. The cell directly beyond the opponent piece on that same axis is empty.
4. The capturing piece can jump over the opponent piece into that empty landing cell.
5. The jumped opponent piece is removed from the board.

If any one of these conditions is false, the capture is not legal.

---

# 10. Capture Axes

Capture is legal only on the two diagonal axes of the hex board:

- NE ↔ SW
- NW ↔ SE

The E ↔ W axis is **not** a capture axis.

All 6 hex directions still matter for adjacency, occupancy, and connection paths. The capture rule is narrower than the connection rule.

---

# 11. Jump Requirement

A capture always requires a jump.

A piece may not remove an opponent piece simply because it is next to it.

If there is no empty landing cell directly beyond the opponent piece on a legal capture axis, then no capture is possible in that direction.

---

# 12. Mandatory Capture Rule

Capture is mandatory when a legal capture is available.

If a player has a legal capture available at the start of their turn, that player must perform a capture instead of placing a new piece.

A player may not ignore a legal capture in order to place a piece elsewhere.

If multiple legal captures are available, the player may choose which legal capture to take. However, they must take one of them.

---

# 13. Capture Timing

Capture timing follows this order:

1. At the start of a player’s turn, check whether that player has at least one legal capture available.
2. If at least one legal capture is available, the player must capture.
3. If no legal capture is available, the player may place one piece on any empty cell.
4. If that placement creates a legal capture for the active player, the active player must resolve that capture immediately.
5. After each capture, check whether the same capturing piece has another legal capture available from its new position.
6. If another legal capture is available, the capture chain continues.

---

# 14. Multi-Capture Rule

Multiple captures are allowed in a single turn.

After a player completes one legal capture, check whether the same capturing piece has another legal capture available from its new position.

If another legal capture is available, the player must continue the capture sequence with that same piece.

A capture chain ends only when that piece has no further legal capture available.

---

# 15. Connection Rule

A player creates a connection when their pieces form one continuous path between any two opposite sides of the board.

A connection is valid when each piece in the path touches at least one other friendly piece in the path through hex-grid adjacency.

All 6 hex directions count for connection.

The game ends immediately when a player completes a valid connection.

---

# 16. Illegal Moves

The following moves are illegal:

1. Placing a piece on an occupied cell.
2. Placing a piece outside the board.
3. Moving a piece without capturing.
4. Capturing along a non-capture axis.
5. Capturing without an empty landing cell beyond the opponent piece.
6. Ignoring a mandatory capture at the start of the turn.
7. Removing an opponent piece without a legal jump.
8. Promoting a piece or treating a piece as a king.
9. Claiming elimination as a win condition.

---

# 17. End of Turn

A turn ends when one of the following is true:

1. The player places one piece legally and no immediate capture is created.
2. The player completes a legal capture and no further mandatory capture is available.
3. The player completes a legal multi-capture sequence.
4. A connection win is triggered.

---

# 18. Draws

No draw condition is currently applied.

The game continues until one player wins by connection.

If future playtesting reveals repeated states, locked positions, or non-ending games, a draw rule may need to be added.

---

# 19. Current Rule Summary

- 2 players.
- Rhombus-shaped hex board with 8 cells per side.
- All hex cells are playable.
- The board starts empty.
- Players alternate turns.
- The game is placement-driven.
- There is no normal movement.
- Capture is the only movement.
- Capture requires a jump over an opponent piece.
- Capture is legal only on NE↔SW and NW↔SE axes.
- E↔W is not a capture axis.
- All 6 hex directions count for connection.
- The landing cell beyond the captured piece must be empty.
- Capture is mandatory if available.
- Placement-created captures resolve immediately.
- Multiple captures are allowed and mandatory while available.
- No kings or promotion.
- A player wins by connecting opposite sides.
- Elimination is not a win condition.
