# AppADay 055 — Morning Offering

A guided, timed companion for the Morning Offering: a five-minute daily rite that begins the day in God's presence and aligns the day's work to vocation.

## What it does

The app walks through five movements in sequence, each with its own duration, matching the flow it was built from:

1. **Posture & Silence (30s)** — a prompt for the Sign of the Cross and one slow breath, paced by a breathing sun disc.
2. **Offer (60s)** — the full Morning Offering prayer, revealed clause by clause across the minute so the pacing matches unhurried prayer rather than a wall of text.
3. **Intentions (60s)** — three fields for family, team, and one student or colleague named specifically. Entries persist locally so the same names don't need retyping every morning, while still being editable each day.
4. **Preview (60s)** — today's date, a free-text glance at the day's shape, and a choice of one virtue to practice: Faith, Hope, Charity, Prudence, Justice, Fortitude, or Temperance, each with a one-line note on what practicing it looks like that day.
5. **Close (30s)** — the St. John Paul II invocation and a closing Sign of the Cross, naming the chosen virtue back to the person.

Each step auto-advances on its timer by default, but auto-advance can be turned off, and every step can be paused, resumed, or navigated back to at any point, so an interruption mid-prayer never breaks the flow.

Completing the full sequence logs the day's virtue and intentions to a local history (last 30 entries) and tracks a day-over-day streak of completed offerings, visible on the closing screen.

## Design

The signature element is a central sun disc that rises from night indigo through violet, rose, and amber to full gold as the five steps progress, visually enacting dawn breaking alongside the prayer itself. A thin progress ring around the disc marks time remaining in the current step, and five small dots mark position in the sequence.

## Technical notes

Single-file vanilla HTML, CSS, and JavaScript. No build step, no external dependencies beyond Google Fonts (Cormorant Garamond, Source Serif 4). All state (intentions, streak, virtue history) is stored in `localStorage` and never leaves the browser. Verified ASCII-clean with no raw Unicode or smart-quote characters in source, and `node --check` clean on the extracted script.

## Category

Spirituality (S)

## Live

https://augustineiacopelli.github.io/appaday-055-morning-offering/

Part of [AppADay](https://augustineiacopelli.github.io/appaday/) — one app, every day.
