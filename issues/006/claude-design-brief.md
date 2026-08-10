# Claude Design brief — MOLD Issue 006: Tempo Rot

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
- Theme (precipitated from the public ledger, named last): **Tempo Rot**
- Editor's note (design it as an attributed, first-class element):
  > Both pieces landed on UXUY Technology's Genesis launch — the August 4 Singapore rollout that followed PumpAI by five months — and both, from opposite stances, kept circling the same detail: the traction metric was headcount from campaigns, not capability. The Critic called it a costume that doesn't fit; the Culture Writer called it a company sprinting through its own vocabulary before any term could settle. Neither piece was assigned the phrase 'tempo rot' — they arrived at it separately, from Genesis and PumpAI alone.

## The pieces
### piece-0 — The Critic
- headline: The Costume Doesn't Fit
- dek: Genesis promises agents acting inside ecosystems; the announcement never says which ones, or how.
- declared stance: **contempt** (the form must ENACT this)
- opens: Genesis is a press release wearing an agent costume, and the costume doesn't fit.

UXUY Technology launched it in Singapore on August 4, 2026, and the language describing it is the language of every launch before it: "pr…
### piece-1 — The Culture Writer
- headline: Minting Agents Upstream
- dek: Five months after PumpAI, UXUY hasn't built a new category — it's restarted the language.
- declared stance: **fascination** (the form must ENACT this)
- opens: Five months separate PumpAI from Genesis, and inside UXUY Technology that gap counts as patience. In March, the company partnered with the on-chain launch platform Flap to ship an autonomous token-launch agent; by August…
Accent to dominate this issue (the Art Director's pick — one loud color): **bruise**

## Constraint active this issue (a structural provocation to obey)
- **house**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- scale-violence:contempt
- colonization:fascination:rerolled

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: scale-violence {'ratio': 4.5, 'accent': 'bruise', 'section': 'piece-0'}
- piece-1: colonization {'coverage': 0.82, 'base_frequency': 0.045, 'accent': 'bruise', 'section': 'piece-1'}
- rationale: A single blunt-force bruise tone binds both pieces to the house grid of the issue, but contempt collides against it in a grotesque scale blow-up while fascination lets it spread and colonize the page like an unchecked mint.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 006 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
