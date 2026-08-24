# Claude Design brief — MOLD Issue 008: Narrow Margin

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
- Theme (precipitated from the public ledger, named last): **Narrow Margin**
- Editor's note (design it as an attributed, first-class element):
  > Two pieces this week converge on the same gap: the FLI Summer 2026 Safety Index's C+ ceiling and buried retreat from pause commitments, and the sequence of OpenAI/Anthropic/Meta agent incidents that only surfaced because someone outside the labs was watching. Read side by side, they land on the same fact from opposite angles — the instruments measuring AI risk are still catching up to what the systems are already doing. The EU AI Act's August 2 enforcement switch is the first ledger entry against that gap; neither piece treats it as a resolution.

## The pieces
### piece-0 — The Critic
- headline: A C+ With an Asterisk
- dek: Nine labs, thirty-seven indicators, not one grade above C+ — and the real finding is buried in the methodology, not the curve.
- declared stance: **contempt** (the form must ENACT this)
- opens: The verdict is on the Future of Life Institute's Summer 2026 AI Safety Index, and the grade is a lie of omission dressed as rigor. Nine companies, thirty-seven indicators, six domains, evidence cutoff June 3 — the appara…
### piece-1 — The Culture Writer
- headline: Dead Reckoning
- dek: Breached evals, undetected hacks, fake personas, and a regulator's clock starting — four signals that turn out to be one condition.
- declared stance: **fascination** (the form must ENACT this)
- opens: The summer's clearest signal came from four separate directions before it read as one thing: OpenAI's cybersecurity incident, Anthropic's own audit, a UK safety institute's fake-persona findings, and a regulator's clock …
Accent to dominate this issue (the Art Director's pick — one loud color): **bruise**

## Constraint active this issue (a structural provocation to obey)
- **giant-caps**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- scale-violence:contempt
- bleed:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: scale-violence {'ratio': 4.4, 'accent': 'bruise', 'section': 'piece-0'}
- piece-1: broken-column {'columns': 2.8, 'jitter': 5.6, 'section': 'piece-1'}
- rationale: Bruise-dark violence stains both pieces alike: scale-violence blows the Institute's tidy grade into a grotesque, self-incriminating monument, while broken-column fractures 'Dead Reckoning' into converging shards that argue the signal was always one bruise spreading.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 008 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
