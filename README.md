# Panini FIFA World Cup 2026 — Adrenalyn XL Collection Tracker

A single-page tracker for the Panini FIFA World Cup 2026 Adrenalyn XL trading-card
collection (all 630 cards).

**Live:** https://panini-cards.github.io/fifa-wc-2026/

## Features

- Quick-add card numbers (`10, 15, 22-25`) to mark what you own.
- Click a tile to toggle owned. Right-click / long-press to set an exact count for duplicates.
- Overall percentage, per-team progress bars, per-special-set progress bars.
- Completed teams / sets (12/12, 9/9, etc.) highlight green in the summary panel.
- Search by card number, 3-letter team code, team name, or player name.
- Filter by Owned / Missing / Doubles.
- Export a missing list or doubles list as copy-pasteable text for trading.
- Export / import a JSON backup for cross-device transfer.
- Dark mode via system preference.
- Data stays in your browser (`localStorage`). No account, no server — you can safely
  share the link and each visitor tracks their own private collection.

## Local development

```bash
python3 -m http.server 8000
# open http://localhost:8000/
# tests: http://localhost:8000/tests.html
```

Deployment is GitHub Pages from `main` branch root — any push triggers a rebuild in
~20 seconds.

## Files

- `index.html` — the whole app (markup, CSS, JS in one file).
- `checklist.json` — the 630-card master list.
- `tests.html` — browser-run assertions for pure functions.

## Reporting typos

Card names were hand-transcribed from the Panini checklist PDF, so a few may be off.
If you spot one, open an issue with the card number and the correct name (as printed
on the physical card).
