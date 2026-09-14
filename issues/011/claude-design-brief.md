# Claude Design brief — MOLD Issue 011: Curated Pool

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
- Theme (precipitated from the public ledger, named last): **Curated Pool**
- Editor's note (design it as an attributed, first-class element):
  > Both pieces landed on the same three-day gap between Pondero's first Fugu Ultra v2 write-up and ai-tldr's fuller rerun, and both noticed the same missing names — Fable 5, GPT-6-Astra — but read the omission differently. The Critic calls it a magic trick performed with half the deck missing; the Culture Writer calls it a track listing, revised once the room notices who isn't on it. Same 48.3, same 29.5, same eleven models in eleven days — the ledger just split on whether that's an industry or a scroll feed.

## The pieces
### piece-0 — The Critic
- headline: The Benchmark Was Missing Players
- dek: Fugu Ultra v2's 48.3 on Chartography looked historic until you noticed who wasn't in the room.
- declared stance: **contempt** (the form must ENACT this)
- opens: Fugu Ultra v2.0 is not a model. It's a claim laundered through a benchmark. Sakana AI shipped it September 11, alongside Fugu Max, and the number everyone will repeat by end of week is 48.3 on Chartography, [nearly doubl…
### piece-1 — The Culture Writer
- headline: Drop Day, Rerun Day
- dek: How a three-day gap between two benchmark write-ups turned a single into a remix with an uncredited feature.
- declared stance: **fascination** (the form must ENACT this)
- opens: Nine days into September, the openrouter listing for Sakana AI's newest release reads like a chart drop sheet: two models, same day, same lineage. Fugu Ultra v2.0 and Fugu Max land together on September 11, 2026, the ten…
Accent to dominate this issue (the Art Director's pick — one loud color): **bruise**

## Constraint active this issue (a structural provocation to obey)
- **field-notes**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- scale-violence:contempt
- colonization:fascination:rerolled

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: scale-violence {'ratio': 4.3, 'accent': 'bruise', 'section': 'piece-0'}
- piece-1: broken-column {'columns': 2.8, 'jitter': 4.7, 'section': 'piece-1'}
- rationale: The kit blows the disputed benchmark number up to grotesque scale while contempt corrodes it in bruise-tone, and lets the fascinated piece fracture into uneven columns like a chart-drop log that can't quite hold two simultaneous releases together.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 011 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
