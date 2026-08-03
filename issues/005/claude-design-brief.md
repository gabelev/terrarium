# Claude Design brief — MOLD Issue 005: One Point

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
- Theme (precipitated from the public ledger, named last): **One Point**
- Editor's note (design it as an attributed, first-class element):
  > Two pieces landed on the same numbers this week — Opus 5's 61 against Fable 5's 60, the Agentic Index score of 55.3, DeepSeek V4-Flash's $0.14/$0.28 pricing — and read them in opposite directions. The Critic saw a coronation built on noise; the Culture Writer saw the gap where human timing used to live getting quietly absorbed by agentic loops. Neither piece disputes the numbers. They dispute what the numbers are for.

## The pieces
### piece-0 — The Critic
- headline: The Decimal Throne
- dek: A one-point lead over 586 models isn't a coronation — it's noise with a press release attached.
- declared stance: **contempt** (the form must ENACT this)
- opens: Claude Opus 5 is not a leap. It is a rounding error with a press release attached, and the numbers say so louder than Anthropic wants them to.

61 on the Artificial Analysis Intelligence Index. Fable 5 sits at 60. GPT-5.…
### piece-1 — The Culture Writer
- headline: Filling the Dead Air
- dek: Opus 5's agentic score and DeepSeek's cheap tokens are quietly taking over the beat between takes.
- declared stance: **fascination** (the form must ENACT this)
- opens: The dead air used to be where a producer thought. Four bars of silence between a generation and a decision, the human beat between prompts — that gap has been closing all year, and this week's leaderboard churn shows exa…
Accent to dominate this issue (the Art Director's pick — one loud color): **sulphur**

## Constraint active this issue (a structural provocation to obey)
- **field-notes**

## Taboo — moves used LAST issue, forbidden now (keep it never-the-same)
- collision:contempt
- colonization:fascination

## What the autonomous Art Director chose (reference, not obligation)
- piece-0: scale-violence {'ratio': 4.4, 'accent': 'sulphur', 'section': 'piece-0'}
- piece-1: colonization {'coverage': 0.83, 'base_frequency': 0.052, 'accent': 'sulphur', 'section': 'piece-1'}
- rationale: Sulphur's toxic clinical glow ties both pieces to the field-notes brief: scale-violence blows the hype-to-reality ratio wide open to sneer at the Decimal Throne's claims, while colonization saturates the page like data creeping into every silent gap the producer used to own.

## Hard constraints (non-negotiable)
- One self-contained HTML file: inline CSS, Google Fonts links OK, no frameworks.
- All type stays selectable text in the DOM; zero raster; SVG (feTurbulence etc.) encouraged.
- Copyright wall: the copy quotes briefly and links out; never embed/reproduce audio or lyrics.
- Keep the piece DOM hooks if you restyle rather than rebuild: `#piece-N`, `.kicker`, `.headline`, `.dek`, `.body`.
- Responsive 375px-1440px, no horizontal scroll; motion behind `prefers-reduced-motion`.
- Relative links: archive at `../../index.html`.

When done: `uv run python -m mold.handoff 005 <your-file.html>` swaps it
in for the autonomous render (verified through the same audit, logged as a
manual render in provenance).
