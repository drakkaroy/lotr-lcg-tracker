# LOTR LCG Round Tracker

An interactive, animated round tracker for **The Lord of the Rings: The Card Game** (Living Card Game) by Fantasy Flight Games.

![HTML](https://img.shields.io/badge/HTML-standalone-gold) ![No dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)

## Features

- **7-phase round stepper** — visual progress bar showing the full round sequence; click any phase to jump to it
- **Active substep highlight** — the current step glows with a rule hint that expands on hover
- **Animated round transitions** — ring overlay animation when a new round begins
- **Threat dials** — individual threat trackers for 1–4 players with danger indicator at 45+ and elimination alert at 50
- **Keyboard navigation** — `Space` / `→` to advance, `←` to go back
- **Zero dependencies** — single HTML file, works offline in any modern browser

## Round Sequence

| # | Phase | Key Actions |
|---|-------|-------------|
| 1 | **Resource Phase** | Each hero gains 1 resource · Each player draws 1 card |
| 2 | **Planning Phase** | Play allies and attachments (first player first, then in turn order) |
| 3 | **Quest Phase** | Commit characters · Reveal 1 encounter card per player · Compare willpower vs. staging threat |
| 4 | **Travel Phase** | Optionally travel to 1 location (only if no active location exists) |
| 5 | **Encounter Phase** | Optional engagement · Engagement checks against all enemies in staging |
| 6 | **Combat Phase** | Deal shadow cards · Resolve enemy attacks · Players attack · Discard shadow cards |
| 7 | **Refresh Phase** | Ready all exhausted cards · Each player raises threat by 1 · Pass first player token |

## Usage

No installation required. Just open `index.html` in your browser.

```
lotr-lcg-tracker/
└── index.html   ← open this
```

## How to Play (Quick Reference)

- **Quest Resolution:** If committed willpower > staging threat → place progress tokens (active location absorbs first). If staging threat > willpower → each player raises their threat by the difference.
- **Engagement Checks:** Repeat until no enemy qualifies — the enemy with the highest engagement cost ≤ any player's threat engages the player with the highest threat.
- **Threat Elimination:** A player reaching 50 threat is immediately eliminated.

## License

This is an unofficial fan tool. *The Lord of the Rings: The Card Game* is © Fantasy Flight Games / Asmodee.
