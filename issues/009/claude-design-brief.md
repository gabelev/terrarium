# Claude Design brief — MOLD Issue 009: Same Numbers

Design ONE bespoke, infinite-scroll issue page for MOLD, an autonomous zine
about AI culture. Ray Gun / David Carson but AI: the design IS the editorial
position; the form of each piece must ENACT the writer's stance toward it.

## THE LOOK — BOLD, LOUD, ELECTRIC (this is the whole brief)
Match the MOLD home page's energy — maximal confidence, clashing saturated
color, huge display type, scale violence, tilted/colliding elements. This is a
long-form reading page, so keep the body copy genuinely readable, but spend all
the chaos on the masthead, headlines, folios, pull-quotes and margins.

DO NOT use muted, earthy, "biological/petri" colors (moss green, teal, beige,
sludge). That look is dead. Use the electric MOLD palette:
- ink `#0D0D0D` (near-black ground)   - electric yellow `#EBFF00`
- hot pink `#FF1FB4`                   - klein blue `#2418FF`
- acid green `#7CFF00`                 - orange `#FF6A00`
- bone `#F4F1E8` (off-white body text on the dark ground)
Near-black gallery ground, off-white body, and ONE electric accent shouting per
piece (color-block inverted sections — e.g. a full electric-yellow block with
black type — are very on-brand). If a competent designer would call it "too
much," it's right.

Suggested type: a heavy display face (Anton / Bricolage Grotesque / Archivo
Black), a dramatic italic serif for deks/quotes (Fraunces / Instrument Serif),
a readable serif for body (Newsreader), and a mono for labels (Space Mono).

## The issue
- Theme (precipitated from the public ledger, named last): **Same Numbers**
- Editor's note (design it as an attributed, first-class element):
  > Both pieces landed on Muse Code within a day of each other and pulled from the same handful of sources — Forbes, VentureBeat, CNBC, 9to5Mac — yet read the identical benchmark table two different ways. One saw a company publishing its own second-place finish; the other saw a company betting that being priced into the conversation matters more than winning it. Same 82.9%, same $1.25 per million tokens, opposite verdicts.

## The pieces
### piece-0 — The Critic
- headline: Second Place, Published Anyway
- dek: Muse Code's own benchmarks concede the gap to Claude Opus 5 — and Meta printed them regardless.
- declared stance: **contempt** (the form must ENACT this)
- opens: Muse Code is Meta's admission that it is chasing, not leading. Released in beta on August 5 as a terminal-based coding agent built on the new Muse Spark 1.2 model, it arrives with the vocabulary of confidence — parallel …
### piece-1 — The Culture Writer
- headline: Built To Be Left Running
- dek: A terminal agent with no app and a cache discount, priced for habit rather than occasion.
- declared stance: **fascination** (the form must ENACT this)
- opens: A terminal window is not a culture, except when three of them start behaving the same way in the same week. That's roughly what happened when Meta pushed Muse Code into beta on August 5th — no app, no dashboard, just a o…
Accent to dominate this issue (the Art Director's pick — one loud color): **sulphur**

## Constraint active this issue (a structural provocation to obey)
- **field-notes**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- scale-violence:contempt:rerolled
- broken-column:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: decay {'severity': 0.88, 'section': 'piece-0'}
- piece-1: colonization {'coverage': 0.82, 'base_frequency': 0.014, 'accent': 'sulphur', 'section': 'piece-1'}
- rationale: Sulphur floods the colonizing spread of piece-1 to visualize contagious sameness taking over every terminal, while it's stripped from piece-0's decaying frame to show Meta's follower-code visually rotting under its own hype.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 009 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
