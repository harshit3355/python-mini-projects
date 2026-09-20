# Python Mini Projects

Seven small, self-contained console programs written while learning Python. Each one is a complete game or utility in a single folder, with no dependencies beyond the standard library.

## Why this exists

Each project targets a specific language concept, which is why they exist as separate programs rather than one growing codebase:

| Project | What it practises |
| --- | --- |
| **Blackjack** | Lists, game state, comparison logic, `random` |
| **Caesar Cipher** | String manipulation, character arithmetic, modular wrapping |
| **Calculator** | Functions as first-class values, dictionary dispatch, recursion |
| **Higher Lower Game** | Working with structured data, score tracking |
| **Hangman** | Loops, sets, string building, ASCII state machines |
| **Number Guessing Game** | Input validation, binary search intuition, difficulty levels |
| **Secret Auction** | Dictionaries, screen clearing, multi-user input flow |

They are deliberately kept in their original form rather than refactored — the point is the progression.

## Running them

Python 3.6 or later. No installation, no dependencies.

```bash
cd Blackjack
python blackjack.py
```

Run each from **inside its own folder**. Every project has its own `art.py` and imports it as a sibling module, so running from the repository root will fail on the import.

```bash
cd "Caeser Cipher"        && python cipher.py
cd Calculator             && python calc.py
cd "HIgher Lower game"    && python high.py
cd Hangman                && python hangman.py
cd "Number Guessing Game" && python number_guessing.py
cd "Secret Auction"       && python auction.py
```

Folder names with spaces need quoting in the shell.

## Structure

Most projects follow the same shape:

- `art.py` — ASCII art and banners, kept separate from the logic
- `<game>.py` — the program itself
- occasionally a data module, such as `game_data.py` for Higher Lower

Splitting the art out is the one deliberate structural habit across all seven: presentation constants stay out of the logic file.

## Notes

- The Secret Auction clears the screen between bidders. That works in a real terminal and not in every IDE console.
- Folder names carry their original typos (`Caeser`, `HIgher`). Left alone so existing links keep working.
- These are learning exercises, not libraries. Read them, run them, break them.
