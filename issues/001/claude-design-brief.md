# Claude Design brief — MOLD Issue 001: Skin Deep

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
- Theme (precipitated from the public ledger, named last): **Skin Deep**
- Editor's note (design it as an attributed, first-class element):
  > Both pieces landed on the same four-hundred-dollar line item — DreadClub: Vampire's Verdict, cited in Raman Media Network's trends report — and read it in opposite directions. The Critic treated the number as the whole review, a receipt standing in for a film nobody screened. The Culture Writer treated genre itself as the thing being bought, the cheapest possible shortcut to audience trust. Neither piece needed the film to exist beyond its price tag.

## The pieces
### piece-0 — The Critic
- headline: The Invoice, Not the Film
- dek: A four-hundred-dollar vampire movie gets cited as proof of a cost curve — nobody mentions if it has a scene worth watching.
- declared stance: **contempt** (the form must ENACT this)
- opens: DreadClub: Vampire's Verdict costs four hundred dollars. Sit with that number. Not four hundred thousand — four hundred. A feature film, priced like a subscription tier, cited proudly in [Raman Media Network's global tre…
### piece-1 — The Culture Writer
- headline: Skin Is the Interface
- dek: Genre isn't style anymore in the AI pipeline — it's the fifteen words that make a cheap output feel trustworthy on first pass.
- declared stance: **fascination** (the form must ENACT this)
- opens: A vampire film for four hundred dollars is sharing a release calendar with a rumored James Bond script about a rogue machine intelligence, and neither is the outlier — they're the same bet, dressed in different skins. Dr…
Accent to dominate this issue (the Art Director's pick — one loud color): **sulphur**

## Constraint active this issue (a structural provocation to obey)
- **off-the-page**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- decay:contempt
- colonization:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: scale-violence {'ratio': 4.5, 'accent': 'sulphur', 'section': 'piece-0'}
- piece-1: bleed {'overflow': 0.55, 'side': 'right', 'section': 'piece-1'}
- rationale: A bilious sulphur wash unifies both pieces: the invoice number is blown so violently oversized it tears off the trim, while skin's fascination bleeds past the gutter, arguing that price and body alike refuse to stay contained on the page.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 001 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
