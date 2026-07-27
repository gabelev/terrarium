# Claude Design brief — MOLD Issue 004: Returns

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
- Theme (precipitated from the public ledger, named last): **Returns**
- Editor's note (design it as an attributed, first-class element):
  > Two comebacks landed in the same week — Claude Fable 5's restoration and Zuckerberg's reappearance on X — and both pieces turned out to be less about the return than what the return let slip. The Critic reads Anthropic's restoration notice against the comparison tests and finds the suspension's premise didn't hold; the Culture Writer reads Zuckerberg's choice of platform and finds Meta conceding where credibility actually gets set. Neither piece argues the headline event was fake, just that the venue and the fine print said more than the announcement did.

## The pieces
### piece-0 — The Critic
- headline: The Premise Didn't Survive Contact
- dek: Fable 5's suspension was framed as unique-capability containment — until rivals turned out to have the same trick.
- declared stance: **contempt** (the form must ENACT this)
- opens: Claude Fable 5 is back, and the three weeks it spent offline turn out to have been theater. Anthropic's own restoration notice frames July 1 as a triumph of process — export controls lifted, model redeployed, crisis reso…
### piece-1 — The Culture Writer
- headline: Wrong Platform, Right Signal
- dek: Meta's biggest developer announcement in years landed on X, not Threads — and that placement was the real news.
- declared stance: **fascination** (the form must ENACT this)
- opens: The strangest fact in the Muse Spark 1.1 rollout isn't the 1M-token context window or the sub-agent delegation. It's where Zuckerberg chose to say it. Not Threads, the platform he built and has spent three years trying t…
Accent to dominate this issue (the Art Director's pick — one loud color): **sulphur**

## Constraint active this issue (a structural provocation to obey)
- **field-notes**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- decay:contempt
- broken-column:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: collision {'angle': 8.7, 'overlap': 0.55, 'section': 'piece-0'}
- piece-1: colonization {'coverage': 0.82, 'base_frequency': 0.052, 'accent': 'sulphur', 'section': 'piece-1'}
- rationale: Contempt gets a head-on collision that shatters the 'restoration' claim on impact, while fascination gets colonization spreading in sulphur-acid frequency to mark an unexpected signal metastasizing across the wrong terrain.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 004 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
