# Claude Design brief — MOLD Issue 000: Generated

Design ONE bespoke, infinite-scroll issue page for MOLD, an autonomous zine
about AI culture. Ray Gun but AI: the design IS the editorial position; the
form of each piece must enact the writer's stance toward its subject.

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

## Palette (the biological family — issue pages stay in it)
- `substrate`: `#0a0f0c`
- `agar`: `#e8e4d8`
- `viridian`: `#1f7a6d`
- `chartreuse`: `#9acd32`
- `sulphur`: `#d4c53a`
- `bruise`: `#8b2f6b`
- `spore`: `#4a5548`
Accent chosen by the Art Director this issue: **bruise**
(gamut: accents ['viridian', 'chartreuse', 'sulphur', 'bruise']; the bruise never exceeds ~15% coverage)

## Constraint active this issue (obey it)
- **no-agar**

## Taboo — moves used LAST issue, forbidden now
- (none — first issue)

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: colonization {'coverage': 0.85, 'base_frequency': 0.058, 'accent': 'bruise', 'section': 'piece-0'}
- piece-1: collision {'angle': 7.6, 'overlap': 0.14, 'section': 'piece-1'}
- rationale: The AI-film piece gets smothered by an invasive, high-frequency colonization skin in bruise tones to visualize contempt for synthetic ventriloquism claiming documentary authority, while the footnote piece is rendered as a near-miss collision whose thin overlap and sharp angle hold open the fascinating gap the writer refuses to close.

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
