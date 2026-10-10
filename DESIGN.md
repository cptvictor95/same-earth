# Design proposal

Working title: **Same Earth**. Direction: a contemporary public-science exhibit—expressive enough to invite exploration, precise enough to trust. Not a dashboard, not a vintage atlas imitation.

## Layout by available width

| Width | Layout | Notes |
|---|---|---|
| Narrow mobile | One large map with a Mercator / Equal Earth switch; optional "See both" stacked view | Country search above the map; selected-country detail below |
| Tablet portrait | Stacked maps, one shared toolbar | No duplicated controls |
| Tablet landscape / desktop | Side-by-side maps, one shared selection | Search, reset, and explanation panel |

Choose layout from measured map legibility and available width, not device detection.

## Interaction rules

- Tap and click are primary. Hover may preview but never gates information.
- Selection survives projection switches, resizes, and rotation.
- Switching projection on mobile keeps the viewport position stable.
- Search covers countries too small to tap reliably.
- Selection is shown by outline plus color change, and the country name appears as text.
- No map interaction traps page scrolling.
- No pan or zoom in the first release.

## Design system foundations

| Foundation | Rule |
|---|---|
| Color | Cool neutral surfaces, high-contrast text, one selection accent; map colors carry meaning |
| Typography | Distinctive heading face plus a readable UI face; final faces chosen during visual exploration |
| Spacing | Small reusable scale; generous space around maps, tighter around controls |
| Tokens | Semantic names: `surface`, `text`, `text-muted`, `border`, `selection`, `focus` |
| States | Default, hover, focus, selected, loading, no results, load failure |
| Motion | Short, purposeful; disabled under `prefers-reduced-motion` |
| Accessibility | WCAG 2.2 AA contrast, visible focus, roughly 44px touch targets |

## Responsive QA checklist

Verify before release at 375px, 768px, 1024px, and 1440px widths:

- No horizontal page overflow.
- Both projection labels remain visible and readable.
- Selected country remains highlighted after switching projection and resizing.
- Keyboard-only path selects, changes projection, and resets.
- Text remains usable at 200% zoom.

## Open decisions

- Final typeface pairing.
- Exact palette values and contrast verification.
- Whether "See both" on mobile is required for the first release or deferred.
