# Claude Design brief — MOLD Issue 000: Generated

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
- Theme (precipitated from the public ledger, named last): **Generated**
- Editor's note (design it as an attributed, first-class element):
  > Two pieces landed on opposite ends of the same question: what happens when the label 'AI-made' has to carry actual weight. The Critic took apart Dreams of Violets, Tribeca's $2,000 synthetic docudrama of the Tehran protests; the Culture Writer read Tidal's new no-royalties policy against Spotify and Apple's disclosure checkboxes and found the only one with teeth.

## The pieces
### piece-0 — The Critic
- headline: No Cameras, No Witness
- dek: The Critic on Dreams of Violets, Tribeca's AI-generated Tehran protest docudrama, and what 'premiere' is covering for.
- declared stance: **contempt** (the form must ENACT this)
- opens: Dreams of Violets is a $2,000 act of ventriloquism dressed as documentary. [Variety](https://variety.com/2026/film/festivals/tribeca-festival-ai-film-dreams-of-violets-fountain-0-1236759724/) confirms Tribeca gave this 7…
### piece-1 — The Culture Writer
- headline: The Footnote That Pays
- dek: The Culture Writer on why Tidal's AI royalty ban does something Spotify and Apple's disclosure rules don't.
- declared stance: **fascination** (the form must ENACT this)
- opens: There's a gap opening between two kinds of platform sentences, and it's worth sitting inside it before the industry averages them out into one boring compliance memo. Spotify and Apple's language, per existing distributo…
Accent to dominate this issue (the Art Director's pick — one loud color): **bruise**

## Constraint active this issue (a structural provocation to obey)
- **house**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- decay:contempt
- colonization:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: scale-violence {'ratio': 4.5, 'accent': 'bruise', 'section': 'piece-0'}
- piece-1: broken-column {'columns': 2.0, 'jitter': 5.5, 'section': 'piece-1'}
- rationale: Under the issue's 'house' constraint, contempt gets blown into a lopsided monument (scale-violence) while fascination gets literally housed in two unstable rooms (broken-column) before the industry paves over the gap.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 000 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
