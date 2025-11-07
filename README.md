# Minesweeper CLI Template

This repository contains a small, self-contained template for a Minesweeper game implemented in Python (CLI).

Files:
- `minesweeper.py` — main script. Start it with `python3 minesweeper.py`.

Quick start:
```bash
# default 9x9 with 10 mines
python3 minesweeper.py

# custom: width height mines
python3 minesweeper.py 10 8 12
```

How to play:
- Commands are entered at the prompt:
  - `r x y` — reveal the cell at column x and row y (0-based)
  - `f x y` — toggle a flag on the cell
  - `q` — quit
- The board display uses:
  - `#` for unrevealed cells
  - `F` for flagged cells
  - `.` for revealed cells with zero neighboring mines
  - `1-8` for revealed cells with that many neighboring mines
  - `*` (only shown after you lose or when board is revealed) for mines

Notes:
- Coordinates are 0-based: top-left is `0 0`.
- The code is intentionally minimal and easy to extend (e.g., add a GUI, better input parsing, timer, or difficulty presets).

Ideas to extend:
- Add recursion limit checks and iterative flood-fill improvements.
- Add difficulty presets or a small GUI using tkinter or pygame.
- Add unit tests covering board generation and reveal behavior.

Enjoy!
