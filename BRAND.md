# Chilyer Studios — Brand Assets

The Frost mark and CHILYER STUDIOS wordmark, ready to ship across GitHub, X, and beyond.

---

## What's in this bundle

```
chilyer-brand/
├── BRAND.md                              ← this file
├── svg/                                   ← scalable source files (preferred wherever possible)
│   ├── frost-icon-deep-frost.svg          ★ primary icon
│   ├── frost-icon-glacier.svg             secondary, friendlier
│   ├── frost-icon-steel.svg               monochrome fallback
│   ├── frost-icon-inverse.svg             for dark backgrounds
│   ├── frost-horizontal-deep-frost.svg    ★ primary horizontal lockup
│   ├── frost-horizontal-inverse.svg       horizontal lockup, dark
│   ├── frost-stacked-deep-frost.svg       primary stacked lockup
│   └── frost-stacked-inverse.svg          stacked lockup, dark
└── png/                                   ← raster exports for platforms that don't accept SVG
    ├── avatars/
    │   ├── avatar-deep-frost-cream-1024.png    ★ X / GitHub profile pic
    │   ├── avatar-deep-frost-cream-512.png       smaller version of same
    │   ├── avatar-inverse-dark-1024.png        for dark-mode optimized profiles
    │   └── avatar-inverse-dark-512.png
    ├── favicons/
    │   ├── favicon-16.png                       browser tab favicon
    │   ├── favicon-32.png                       ★ standard favicon
    │   ├── favicon-64.png
    │   └── favicon-128.png
    ├── lockup-horizontal-deep-frost-120h.png    ★ README header (standard)
    ├── lockup-horizontal-deep-frost-240h.png    README header (retina)
    ├── lockup-horizontal-inverse-120h.png       README header (dark theme)
    └── lockup-horizontal-inverse-240h.png

★ = primary file for that use case
```

---

## Color palette

| Token            | Hex       | Use                                       |
|------------------|-----------|-------------------------------------------|
| Deep Navy        | `#1A2740` | Primary mark body, wordmark on light bg   |
| Electric Cyan    | `#3CDFFF` | Primary icicle accent                     |
| Glacier Blue     | `#3D7AE5` | Secondary mark body (friendlier contexts) |
| Ice Highlight    | `#7AC1F0` | Secondary icicle / inverse mark body      |
| Steel            | `#2C3440` | Monochrome fallback                       |
| White-Blue       | `#E8F4FF` | Inverse icicle accent on dark             |
| Inverse BG       | `#0F1729` | Dark-mode avatar background               |
| Cream            | `#EFE9DC` | Light-mode avatar background              |

---

## When to use which mark

**Deep Frost (primary)** — `#1A2740` body, `#3CDFFF` icicles. Use this 90% of the time. GitHub avatar, X profile pic, repo headers, social posts. This is the studio's voice.

**Glacier (secondary)** — `#3D7AE5` body, `#7AC1F0` icicles. Use when warmth or approachability matters more than authority — game store thumbnails aimed at a wide audience, content that needs to feel friendly rather than serious.

**Steel (monochrome)** — single color `#2C3440`. Use where color is stripped or unavailable: laser-etched merch, single-color print, embroidery, official documents that require monochrome.

**Inverse** — light blue mark, `#E8F4FF` icicles. Use on intentionally dark backgrounds: dark-mode landing pages, Discord server icons, video end cards, anywhere the dark navy of Deep Frost would disappear into the background.

---

## Lockup choices

**Icon mark** — just the C. Use for avatars, favicons, profile pics, app icons, anywhere space is tight.

**Horizontal lockup** — mark on the left, CHILYER STUDIOS stacked on the right. Use for repo README headers, email signatures, footer logos, YouTube/Twitch banners.

**Stacked lockup** — mark above, CHILYER STUDIOS centered below. Use for splash screens, video end cards, business cards, any square or vertical context.

---

## Platform-specific guidance

### GitHub
- **Profile/org avatar** → `png/avatars/avatar-deep-frost-cream-1024.png`. GitHub crops to a circle; the cream square gets clipped, and the safe-zone padding ensures the icicles aren't trimmed off the top.
- **Repo README header** → embed `svg/frost-horizontal-deep-frost.svg` directly in markdown, or use `png/lockup-horizontal-deep-frost-240h.png` as fallback. SVG is preferred — it'll render crisp at every resolution.
- **Repo favicon (for Pages sites)** → `png/favicons/favicon-32.png` or the SVG icon mark.

### X (Twitter)
- **Profile picture** → `png/avatars/avatar-deep-frost-cream-1024.png`. X crops to a circle. The cream-bg version reads better on the X feed than baking a navy square into the avatar.
- **Header banner** → not included here (X banners are 1500×500 with a unique safe-zone for the avatar overlay). Build this when ready by composing the horizontal lockup over a Deep Navy field with intentional negative space.

### YouTube / Twitch (if/when you launch)
- **Channel avatar** → same as X profile picture above.
- **Channel banner** → build at 2560×1440 with the horizontal lockup positioned in the safe area (1546×423 centered region visible on all device sizes). Use Deep Frost on Cream, or Inverse on dark navy depending on channel theme.

### Discord
- **Server icon** → `png/avatars/avatar-inverse-dark-1024.png` if your server uses a dark theme, otherwise the cream version.

---

## Don'ts

These keep the brand cohesive across hundreds of touchpoints over time. Worth following even when no one's watching.

- **Don't recolor** outside the palette above. The cyan icicles are not a "vibe" — they're the brand color.
- **Don't stretch or skew.** The mark is square (within its bounding box including icicles). Always scale uniformly.
- **Don't add effects.** No drop shadows, no glows, no gradients on the mark itself. The flat treatment is the point.
- **Don't rotate the mark.** The icicles point up. Always.
- **Don't separate the icicles from the C.** They're a single design element.
- **Don't put the wordmark on a busy background.** If the background is busy, use the icon mark alone, or place the lockup on a flat field.
- **Don't add taglines** unless you've decided on one and committed across all assets at once.
- **Don't change the wordmark font** without regenerating all the lockup files. CHILYER is set in a geometric sans-serif (Inter or fallback); replacing it with a script or display face will break the brand cohesion.

---

## A note on the wordmark font

The lockup SVGs use a font stack of `Inter, -apple-system, BlinkMacSystemFont, 'Helvetica Neue', Helvetica, Arial, sans-serif`. On any modern OS or browser, one of these will be available and the wordmark will render in a clean geometric sans.

The PNG exports are baked at generation time, so they look identical everywhere regardless of viewer fonts.

For print, embedded use, or anywhere font portability matters, convert the wordmark text to outlined paths in your design software before export. You'd open the SVG in Figma, Illustrator, or Inkscape, select the text, and run "Convert to Path" / "Outline." That makes the wordmark render identically on systems that don't have Inter installed.

---

## Sizing minimums

- **Icon mark**: 16px minimum. Below that, the icicle detail vanishes and you're left with a generic dark C.
- **Horizontal lockup**: 120px wide minimum. Below that, the STUDIOS subtitle becomes illegible.
- **Stacked lockup**: 80px wide minimum.

When in doubt, prefer the icon mark over the lockup at small sizes — better to drop the wordmark entirely than to cram an unreadable one in.

---

## Trademark note

These files are safe to use today on your personal/studio profiles, repos, and channels. Before commercial launch (a paid game on Steam, Itch, or anywhere money changes hands under the studio name), commission a real trademark clearance search for "CHILYER STUDIOS" and the Frost mark through a trademark attorney or service like LegalZoom. The C-as-creature conceit and asymmetric icicle silhouette appear original, but a formal search before commerce is worth the few hundred dollars to confirm.
