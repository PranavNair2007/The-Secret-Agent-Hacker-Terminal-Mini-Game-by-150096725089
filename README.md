# Secret Agent Hacker Terminal & Mini-Game

Created by Student 150096725089

A single-file, retro-futuristic web app: a matrix-style green screen with falling code, fake hacking tools, sound effects, progress bars and a hidden cipher mini-game. Everything (HTML, CSS and JavaScript) lives in one file, `hacker-terminal.html`.

## How to run

1. Download `hacker-terminal.html`.
2. Open it in any modern browser (Chrome, Edge, Firefox, Safari).

No install, build step or server is needed. An internet connection is optional: it only loads the Orbitron and JetBrains Mono fonts from Google Fonts, and falls back to system monospace fonts if offline.

## Features

- **Matrix rain:** animated falling characters drawn on a canvas behind the interface.
- **Hack tools:** four simulated tools, each with a live progress bar and log output:
  - Port scanner
  - Password cracker
  - Firewall breach
  - Satellite uplink
- **Access levels:** your clearance rises from GUEST to GHOST as you complete the tools.
- **Interactive terminal:** type commands, with history on the up and down arrow keys.
- **Sound effects:** synthesized with the Web Audio API, so there are no audio files. Toggle with the Sound button.
- **Click animations:** ripple and press effects on every button.
- **Hidden cipher mini-game:** a five-level Caesar cipher puzzle (see below).

## Terminal commands

| Command | What it does |
|---|---|
| `help` | Lists all commands |
| `scan` | Runs the port scanner |
| `crack` | Runs the password cracker |
| `breach` | Runs the firewall breach |
| `uplink` | Runs the satellite uplink |
| `whoami` | Shows your agent ID and clearance |
| `matrix` | Toggles the rain intensity |
| `clear` | Clears the terminal |
| `cipher` | Unlocks the hidden mini-game |

## The hidden cipher game

Unlock it any of these ways:

- Type `cipher` in the terminal.
- Click the faint **◈** glyph in the footer.
- Click the page title five times.

**How to play:**

1. A scrambled word appears. It was encoded with a Caesar cipher, which shifts every letter forward by a secret number.
2. Move the decoder slider. The decoded preview updates live as you change the shift.
3. When the letters spell a real word, type it in and press Submit.
4. Decode all five words to crack the vault.

**Scoring:** each correct word earns up to 200 points, minus 40 for every wrong attempt (minimum 50). Using the hint costs 50 points. The shifts are random, so every playthrough is different.

## Tech notes

- Plain HTML, CSS and vanilla JavaScript, with no libraries or frameworks.
- Responsive layout that stacks to one column on small screens.
- Respects the `prefers-reduced-motion` setting by turning off CSS animations.
- All hacking is fictional. Nothing touches a network or a real system.

## Files

| File | Description |
|---|---|
| `hacker-terminal.html` | The complete app |
| `README.md` | This file |
