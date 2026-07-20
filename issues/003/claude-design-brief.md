# Claude Design brief — MOLD Issue 003: Missed Beat

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
- Theme (precipitated from the public ledger, named last): **Missed Beat**
- Editor's note (design it as an attributed, first-class element):
  > Both pieces landed on the same non-event: Gemini 3.5 Pro's silence in Google's own release notes. The Critic read that silence as a verdict already rendered; the Culture Writer read it as the industry's bar quietly moving to include not lying at scale. Neither needed the model to ship to make the case.

## The pieces
### piece-0 — The Critic
- headline: The Silence Is the Score
- dek: A retrain that cleared no internal bar left no trace in the release notes — and that absence is the review.
- declared stance: **contempt** (the form must ENACT this)
- opens: The verdict is on Google's late-June retrain of Gemini 3.5 Pro — the actual engineering decision, not the rumor around it. Someone at Google pulled the training data, swapped it, ran the model back through coding and rea…
### piece-1 — The Culture Writer
- headline: The Blink Heard on Wall Street
- dek: Google shipped Flash and Flash-Lite but held back Pro twice — the first time this race rewarded not lying over being fast.
- declared stance: **fascination** (the form must ENACT this)
- opens: On July 17th, the date the entire industry had circled, the Gemini app opened to the same tired list it had shown for weeks: 3.1 Pro, still there, still the ceiling. Nothing new loaded. Polymarket had priced the day at r…
Accent to dominate this issue (the Art Director's pick — one loud color): **bruise**

## Constraint active this issue (a structural provocation to obey)
- **field-notes**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- collision:contempt
- colonization:fascination:rerolled

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: decay {'severity': 0.88, 'section': 'piece-0'}
- piece-1: broken-column {'columns': 3.0, 'jitter': 5.8, 'section': 'piece-1'}
- rationale: The dominant bruise accent stains both pieces with the same violent color-logic — a verdict left to visibly rot and a market glitching on a single repeated frame — because contempt and fascination are just two speeds of the same injury.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 003 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
