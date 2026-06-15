# SET — The Card Game

A fully playable SET card game in the browser. Single HTML file, zero dependencies — just open and play.

🎮 **[Play now](https://yedi18.github.io/set-game/)**

## How to Play

Each card has **4 attributes**:

| Attribute | Values |
|-----------|--------|
| Number    | 1, 2, 3 |
| Color     | Red, Green, Purple |
| Shape     | Diamond, Squiggle, Oval || Fill      | Solid, Striped, Open |

A **SET** is 3 cards where for each attribute, the values are either **all the same** or **all different** across the three cards.

Click 3 cards to select them — the game validates automatically.

## Features

### Home Screen
- Personal records (score, time, streak, games played)
- Rules explanation with a live example SET
- Settings: sound, colorblind mode, keyboard shortcuts
- "Continue Game" button if a game is in progress

### Gameplay
- 12-card board (up to 21 when dealing extra)
- Click 3 cards → instant validation with animation
- Board returns to 12 cards after finding a SET (even when at 15)
- Pause anytime and return to the home screen

### Scoring
- **+3 points** per SET found without hints
- **Streak multiplier**: ×2 after 3 consecutive SETs, ×3 after 5
- **Hint penalty**: −1 / −2 / −3 / −5 depending on hint level

### Hint System (4 levels)
1. "Is there a SET on the board?"
2. Highlights one card that belongs to a SET
3. Highlights two cards of the same SET
4. Reveals the full SET with a text description

### Personal Records (localStorage)
- High score
- Fastest completion time
- Longest streak
- Total games played and total SETs found

### Accessibility
- **Colorblind mode**: adds symbols (◆ ≈ ●) below each shape
- **Sound**: audio feedback via Web Audio API (toggleable)

### Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `1`–`9` | Select cards 1–9 |
| `Q`–`Y` | Select cards 10–15 |
| `N` | New game |
| `H` | Next hint |
| `D` | Deal +3 cards |
| `Esc` | Pause / return to home |

## Running Locally

No server needed — just open `index.html` in any modern browser.

## Tech Stack

- Vanilla HTML5 + CSS3 + JavaScript
- Inline SVG for card rendering
- Web Audio API for sound effects
- localStorage for scores and settings persistence
