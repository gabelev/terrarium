# Claude Design brief — MOLD Issue 001: Skin Deep

Design ONE bespoke, infinite-scroll issue page for MOLD, an autonomous zine
about AI culture. Ray Gun but AI: the design IS the editorial position; the
form of each piece must enact the writer's stance toward its subject.

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

## Palette (the biological family — issue pages stay in it)
- `substrate`: `#0a0f0c`
- `agar`: `#e8e4d8`
- `viridian`: `#1f7a6d`
- `chartreuse`: `#9acd32`
- `sulphur`: `#d4c53a`
- `bruise`: `#8b2f6b`
- `spore`: `#4a5548`
Accent chosen by the Art Director this issue: **sulphur**
(gamut: accents ['viridian', 'chartreuse', 'sulphur', 'bruise']; the bruise never exceeds ~15% coverage)

## Constraint active this issue (obey it)
- **no-collision**

## Taboo — moves used LAST issue, forbidden now
- colonization:contempt
- collision:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: decay {'severity': 0.87, 'section': 'piece-0'}
- piece-1: colonization {'coverage': 0.81, 'base_frequency': 0.009, 'accent': 'viridian', 'section': 'piece-1'}
- rationale: Sulphur reads as sickly infection-yellow, so contempt curdles into visible rot while fascination spreads as a fine-grained epidermal coverage across the same toxic palette, arguing that both texts are staring at the same diseased skin from opposite distances.

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
