# Brand Workspace Context

_Last updated: 2026-05-26_

Chilyer Studios brand source of truth. The asset catalogue and operational
rules live in `BRAND.md` — read that first. This file describes the
*workspace lens*: when to enter and how brand reaches other workspaces.

## Workspace role

Brand defines the *studio's identity* — Frost mark, color palette
(Deep Navy `#1A2740`, Electric Cyan `#3CDFFF`, Glacier Blue `#3D7AE5`,
Ice Highlight `#7AC1F0`, Steel `#2C3440`, White-Blue `#E8F4FF`, Inverse BG
`#0F1729`, Cream `#EFE9DC`), voice, typography. It is the **single source
of truth**: other repos reference it, they never copy assets out.

## When to enter Brand

- Adding or revising a mark variant (deep-frost, glacier, steel, inverse)
- Adding or revising a brand color token
- Defining voice / tone for studio-level copy (README headers, OBS overlays,
  GitHub bios)
- Generating new export sizes (avatars, lockups, favicons)

## When NOT to enter Brand

- Per-game art direction — each game has its own art language; see the
  cast-philosophy rule in root `CLAUDE.md` (themes don't bleed between games)
- Marketing campaigns / social copy / dev updates — those are SocialMedia
- Embedding brand into a product — *reference* `chilyer-brand\` from the
  product, don't duplicate assets

## Process

When brand is being **applied** (the common case — you're working in
another workspace and need a brand asset):

1. Read `BRAND.md` for the rule (color token, mark variant, voice example)
2. Reference the source file in `chilyer-brand\` — don't copy
3. If the rule is missing or ambiguous, **update `BRAND.md` first**, then
   apply. Brand doesn't evolve through fait accompli in product repos.

When brand is being **changed**:

1. Edit `BRAND.md` to describe the new rule
2. Generate the asset file(s) under `svg/` and/or `png/`
3. Note the change in the current sprint (Studio workspace)

## What good looks like

- Exactly one answer to "what's the brand cyan" (`#3CDFFF`, Electric Cyan)
- New marks ship as SVG source AND raster exports at BRAND.md's primary sizes
- Voice examples are concrete paragraphs you'd actually publish, not adjectives

## What to avoid

- Duplicating brand assets into other repos
- Per-game mark variants — if a game needs its own logo, that's a *game
  brand*, not a studio brand; build it in the Product and link from
  `BRAND.md` as derivative

## Skills / tools to load

- `chilyer-brand-application` — Chilyer-specific brand application
  skill (lives at `.claude\skills\chilyer-brand-application\SKILL.md`).
  Encodes the palette tokens, mark variants, don'ts, and
  reference-not-copy rule. **Replaces the Anthropic `brand-guidelines`
  skill** that previously appeared here — that one applies Anthropic's
  brand, not Chilyer's.
- `canvas-design` — for new marks, posters, brand graphics (still
  useful; this is the *creation* tool, while
  `chilyer-brand-application` is the *application discipline*)
