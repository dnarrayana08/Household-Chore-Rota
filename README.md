# 🏡 Household Chore Rota

A single-page web app for families and housemates who want a simple weekly chore board. See the week's chores in one place, assign them to the people you live with, and tick them off — all on one screen.

Everything runs entirely in the browser: **no backend, no database, no login, no payments**. Open `index.html` and start using it.

## What it does

The screen is organised as three stacked sections (no tabs, no separate pages):

- **Progress this week** — live counts of done, still-to-do, and overdue chores, a completion progress bar, and the current Monday–Sunday date range.
- **People** — add the people in your household with an optional fun label. Each card shows a coloured avatar and how many open chores that person has. Tap a card to highlight their chores across the roster.
- **Weekly roster** — add chores with a day of the week (the picker defaults to today). Each chore shows its day chip, assignee, and status (Done ✓ / Today / Pending / Overdue / Needs someone).

## How to use it

1. **Add people** — type a name (and optionally a label like "Bin-day hero") in the People section, then press *Add person*.
2. **Add chores** — type a chore and pick a day in the Weekly roster section, then press *Add chore*.
3. **Assign** — tap the coloured dot next to a chore to give it to that person. Dots are colour-matched to each person's card.
4. **Mark done** — press *Mark done* when a chore is finished; press *Undo* to reopen it.
5. **Remove** — the ✕ on any person card or chore row deletes it. Removing a person returns their chores to *Unassigned*.

Statuses are day-aware: chores earlier in the week that aren't done show as **Overdue**, and today's chores show as **Today**.

## Notes

- Data is not simulated — the board starts empty and everything on it is entered by you.
- Nothing is saved or sent anywhere. The board lives in memory and resets when the page reloads.

## Tech

One self-contained `index.html` — plain HTML, CSS, and vanilla JavaScript. No frameworks, no build step, no dependencies.
