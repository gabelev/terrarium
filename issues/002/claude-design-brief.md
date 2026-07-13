# Claude Design brief — MOLD Issue 002: Uneven Restoration

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
- Theme (precipitated from the public ledger, named last): **Uneven Restoration**
- Editor's note (design it as an attributed, first-class element):
  > Both pieces this week landed on the same nineteen-day gap — Fable 5 and Mythos 5, cut off by a Commerce letter on June 12 and brought back unevenly on July 1 — but read the asymmetry in opposite registers. The Critic sees a leash dressed as a comeback; the Culture Writer sees a live demonstration of how creative infrastructure gets triaged by policy. Neither called the restoration clean, which is what made the cluster worth naming.

## The pieces
### piece-0 — The Critic
- headline: Probation, Not Pardon
- dek: The restoration reads like vindication until you check the usage cap and the fine print.
- declared stance: **contempt** (the form must ENACT this)
- opens: Verdict: Claude Fable 5's restoration is not a comeback. It's a probation.

Seventeen days offline, June 12 to July 1, over what Commerce called national security concerns, and the model returns not with a clean bill but…
### piece-1 — The Culture Writer
- headline: The Switch Was Always There
- dek: Nineteen days of downtime showed the field which model gets to be infrastructure and which gets fenced off.
- declared stance: **fascination** (the form must ENACT this)
- opens: For nineteen days this summer, a silence rippled through every workflow built on top of Claude Fable 5 and Mythos 5 — not a crash, not a bug, but a government letter. On June 12, the Commerce Department's Bureau of Indus…
Accent to dominate this issue (the Art Director's pick — one loud color): **bruise**

## Constraint active this issue (a structural provocation to obey)
- **fractured**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- decay:contempt
- colonization:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: collision {'angle': 9.0, 'overlap': 0.6, 'section': 'piece-0'}
- piece-1: colonization {'coverage': 0.85, 'base_frequency': 0.052, 'accent': 'bruise', 'section': 'piece-1'}
- rationale: Contempt gets a head-on collision at maximum angle and overlap—an unresolved crash where verdict meets no mercy—while fascination spreads as a bruised colonization, high coverage and frequency mapping the government switch as an infection already under the skin.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 002 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
