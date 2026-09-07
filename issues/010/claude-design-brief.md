# Claude Design brief — MOLD Issue 010: Frozen Tempo

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
- Theme (precipitated from the public ledger, named last): **Frozen Tempo**
- Editor's note (design it as an attributed, first-class element):
  > Both pieces landed on Atlas, World Labs' September 1 world model, from opposite directions within days of each other. The Critic reads the splats and the early-access gate as stillness dressed up as agency; the Culture Writer holds that same launch against Suno's discover feed and finds the real story in the contrast — one field still spending to chase a benchmark, another that quietly stopped trying to outrun its own ninety-second floor.

## The pieces
### piece-0 — The Critic
- headline: The Snow Globe Model
- dek: Atlas renders gorgeous, walkable-looking rooms where nothing you do produces a consequence.
- declared stance: **contempt** (the form must ENACT this)
- opens: Atlas is a $1.2 billion machine for producing beautiful stillness. World Labs' [omni world model](https://www.worldlabs.ai/blog/atlas) claims to natively fuse text, images, video, and 3D into one shared spatial context —…
### piece-1 — The Culture Writer
- headline: The Frontier Nobody's Funding
- dek: Atlas chases a benchmark score while Suno's feed proves music-gen stopped chasing anything at all.
- declared stance: **fascination** (the form must ENACT this)
- opens: The scroll doesn't stop moving, but nothing in it accelerates. Open Suno's discover feed this week and you get the same ninety-second architecture over and over: intro-hook-drop-fade, no track daring past the length a Ti…
Accent to dominate this issue (the Art Director's pick — one loud color): **bruise**

## Constraint active this issue (a structural provocation to obey)
- **giant-caps**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- decay:contempt
- colonization:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: scale-violence {'ratio': 4.4, 'accent': 'bruise', 'section': 'piece-0'}
- piece-1: colonization {'coverage': 0.82, 'base_frequency': 0.011, 'accent': 'bruise', 'section': 'piece-1'}
- rationale: Bruise-toned violence runs through both pieces: scale-violence blows the $1.2B snow-globe claim up until its stillness looks grotesquely disproportionate, while colonization lets the same repeating pattern spread and thicken across the frame, mimicking Suno's stalled, fascinating loop.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 010 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
