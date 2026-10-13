# Ideas — room for improvement

Ready-to-paste issue texts. Pick one, open it as an issue, or just start a pull request.

---

## 1. Add automated tests for the rules engine

**Problem:** `npm test` runs, but there are no test files yet. Placement, mandatory capture, capture chains and connection detection are only checked by playing.

**Idea:** Pull the pure rule functions (board creation, legal moves, capture resolution, win detection) out of `app.js` into a module and cover them with `node --test`.

**Done when:** a mandatory capture, a multi-jump chain, and a win on each axis each have a passing test.

---

## 2. Agent-vs-agent mode with batch replay logs

**Problem:** The built-in agent only plays against a human.

**Idea:** Add an agent-vs-agent mode (in the browser or as a small Node script) that plays N games and saves one JSON log per game, in the existing log format.

**Done when:** you can run 100 games unattended and open any log in the replay viewer.

---

## 3. A stronger agent

**Problem:** The current agent is connection-first and greedy. It is easy to beat and does not plan around capture threats.

**Idea:** Try shortest-path / two-distance evaluation from Hex, look-ahead over capture chains, or Monte Carlo tree search.

**Done when:** the new agent beats the current one in most of 100 games (see idea 2).

---

## 4. Load a saved game log into the replay viewer

**Problem:** Logs can be downloaded as JSON but not loaded back in.

**Idea:** Add a "Load Game Log" button that reads a JSON log and opens it in replay mode.

**Done when:** a downloaded log replays turn by turn exactly as it was played.

---

## 5. Accessibility and keyboard play

**Problem:** The board is mouse-only, and some states rely on colour alone (purple must-capture, green landing cells).

**Idea:** Add keyboard navigation, ARIA labels for cells, and a shape or pattern alongside each highlight colour.

**Done when:** a full game can be played with the keyboard, and highlights are readable without colour.
