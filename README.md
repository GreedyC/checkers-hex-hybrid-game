# Checkers + Hex

A two-player strategy game that combines the connection goal of Hex with the jump capture tactics of Checkers.

---

## How to play

### Step 1 — Download the game

1. Go to the repository page on GitHub
2. Click the green **Code** button
3. Click **Download ZIP**
4. Open your Downloads folder and double-click the ZIP file to unzip it
5. You will now have a folder called `checkers-hex-mvp`

---

### Step 2 — Open the game

1. Open the `checkers-hex-mvp` folder
2. Find the file called **`index.html`**
3. Double-click it
4. It opens automatically in your web browser — no installation needed

---

### Step 3 — Start a game

1. **Enter player names** (optional) — type your name in the Player 1 and Player 2 boxes, or leave them as-is
2. **Choose a game mode:**
   - **Human vs Human** — two people take turns on the same screen
   - **Human vs Agent** — you play against the computer
3. Click **▶ New Game**

---

## The goal

Connect **any two opposite sides** of the board with an unbroken line of your pieces.

The board has four sides:
- **Top and bottom** — marked with a green border
- **Left and right** — marked with a red border

You win the moment your pieces form a continuous path from one side to the opposite side — in any direction, any shape.

---

## How to place a piece

- Click any empty cell on the board to place your piece there
- Pieces are never moved after placement — **the only exception is a capture jump** (see below)

---

## Captures

You can capture an opponent's piece by **jumping over it**.

For a capture to happen:
1. Your piece must be on the board
2. An opponent's piece must be directly next to it **along a diagonal direction**
3. The cell on the other side of the opponent's piece must be **empty**
4. Your piece jumps over the opponent's piece and lands in that empty cell
5. The opponent's piece is removed from the board

### Captures are mandatory

If any of your pieces can capture at the start of your turn — you **must** capture. You cannot place a new piece instead.

**How to capture:**
- Pieces that must capture are highlighted in **purple**
- Click a purple piece to select it
- Valid landing cells appear in **bright green**
- Click a green cell to complete the jump
- If another jump is available from the landing cell, green cells appear again — keep clicking until the chain ends

### Capture chains

If your piece can jump again immediately after landing, you must continue jumping. The chain ends only when no further jump is available.

---

## Capture directions

Captures only work along two diagonal directions on the hex board:

- Northeast ↔ Southwest
- Northwest ↔ Southeast

The East ↔ West direction is **not** a capture direction.

All six directions still count for **connection** (winning path).

---

## Replay controls

After a game (or during one), you can review every move:

| Button | What it does |
|---|---|
| **▶ Play** | Auto-plays through all turns |
| **⏸ Pause** | Stops the auto-play |
| **← Prev Turn** | Steps back one turn |
| **Next Turn →** | Steps forward one turn |

If you go back during a game and make a different move, the game records it as a **fork** — a new branch from that point. All branches are saved.

---

## Download the game log

Click **↓ Download Game Log (JSON)** at any time to save a full record of the game to your computer.

The log includes:
- Every move made by both players
- Board state before and after each move
- Captures
- Date and time of each turn
- All branches and forks if you replayed and changed moves
- The winner

---

## Colour guide

| Colour | Meaning |
|---|---|
| Blue circle | Player 1's piece |
| Red circle | Player 2's piece |
| Purple cell | A piece that must capture this turn |
| Cyan cell | The piece you have selected |
| Bright green cell | A valid landing cell — click to jump |
| Orange cell | A piece that was just captured |
| Blue path | The winning connection |
| Green border | Top and bottom edges of the board |
| Red border | Left and right edges of the board |

---

## Rules summary

- 2 players
- Take turns placing one piece per turn
- Win by connecting any two opposite sides of the board
- Captures are jumps over adjacent opponent pieces — landing cell must be empty
- If a capture is available at the start of your turn, you must take it
- Chain captures continue until no further jump is available
- No piece promotion or kings
- Capturing all opponent pieces is not a win condition

---

## No installation required

The game runs entirely in your browser. You do not need to install anything.

---

## Contributing

You are welcome to fork this repository for non-commercial playtesting, study, feedback, and proposing improvements.

If you would like to suggest a change:

1. Fork the repository.
2. Test your idea locally by opening `index.html`.
3. Submit a pull request or issue explaining the change.

Please do not use this project commercially, rebrand it, redistribute it as a separate product, or claim ownership without written permission.

For collaboration or licensing inquiries:

https://nazakgul.games

---

## Intellectual property notice

Checkers + Hex is a working title for an original hybrid abstract strategy game designed by Naz Akgül.

The game design, source code, rules presentation, interface, written materials, and related materials in this repository are Copyright © 2026 Naz Akgül. All rights reserved unless otherwise stated.

This repository is provided for personal viewing, playtesting, study, feedback, and contribution to the original project. Forks are welcome for non-commercial playtesting and proposing improvements back to the project.

No permission is granted to sell, commercialize, rebrand, redistribute as a separate product, claim ownership, or create commercial derivative works without prior written permission.

For licensing, collaboration, publication, or commercial inquiries, please visit:

https://nazakgul.games

