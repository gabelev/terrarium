# Claude Design brief — MOLD Issue 007: Cadence

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
- Theme (precipitated from the public ledger, named last): **Cadence**
- Editor's note (design it as an attributed, first-class element):
  > Two writers looked at the same three-week gap between Gemini 3.6 and 3.7 Flash and saw different machines: one a metronome ticking against a regulator's clock, the other a price drop financing bedroom lyric-batch pipelines nobody at Google budgeted for. Neither piece disputes the release happened fast. They just disagree about what fast is for.

## The pieces
### piece-0 — The Critic
- headline: The Beat Is the Deliverable
- dek: Gemini 3.7 Flash shipped 23 days after 3.6 — the cadence, not the model, is the product.
- declared stance: **contempt** (the form must ENACT this)
- opens: Gemini 3.7 Flash is not a model. It is a metronome click. Google shipped it on August 13, 2026, twenty-three days after Gemini 3.6 Flash landed on July 21, and the [gap between them](https://memeburn.com/google-launches-…
### piece-1 — The Culture Writer
- headline: Cheap Meters Change Behavior First
- dek: A halved token price on Gemini 3.7 Flash is quietly financing thousand-variation lyric batches nobody built it for.
- declared stance: **fascination** (the form must ENACT this)
- opens: Somewhere in a Discord server dedicated to Suno prompt-chains, someone posted a screenshot last week that had nothing to do with music at all: a pricing table. Gemini 3.7 Flash, half the cost of its predecessor on input …
Accent to dominate this issue (the Art Director's pick — one loud color): **sulphur**

## Constraint active this issue (a structural provocation to obey)
- **off-the-page**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- scale-violence:contempt:rerolled
- colonization:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: scale-violence {'ratio': 4.5, 'accent': 'sulphur', 'section': 'piece-0'}
- piece-1: bleed {'overflow': 0.55, 'side': 'left', 'section': 'piece-1'}
- rationale: Sulphur burns across both pieces like an alarm, but where contempt is rendered as a headline scaled so violently it shears off the page, fascination is rendered as a screenshot literally bleeding past the margin into the reader's world.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 007 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
