# Product brief

## Purpose

Let curious visitors compare two map projections of the same world and understand what each one shows accurately and what it distorts.

## Audience

General curious visitors, students, and teachers. No login, account, or prior cartography knowledge required.

## First release scope

**Included**

- Two labeled views: Mercator and Equal Earth, built from one shared geographic dataset.
- Country selection by clicking or tapping a country, or by a searchable country list.
- Shared selection: a selected country is highlighted in every visible view.
- Reset control and selected-country name shown as text.
- Short explanation of what each projection preserves and distorts.
- Source and data-date disclosure, and a note on the UN context.

**Excluded**

- Accounts, comments, or user-generated content.
- Historical borders or changing political boundaries.
- Numerical area or distance comparisons.
- Payment processing or donor accounts inside the application.
- Additional projections, globe view, or pan/zoom, until the core comparison is validated.

## Acceptance criteria

1. Both projections render from the bundled dataset; no external map API is called at runtime.
2. Selecting a country in one view highlights the same country in the other.
3. Every control works with keyboard alone and shows a visible focus state.
4. Selection persists across projection switches, resizes, and orientation changes.
5. Loading, empty-search, and data-failure states are visible and recoverable.
6. Mercator's polar cutoff and the dataset source/version are stated on the page.
7. Reduced-motion preferences disable non-essential transitions.

## Accuracy commitments

- Describe Mercator and Equal Earth as projections, not as official or replacement maps.
- Attribute UN-related claims to the source reporting until the original resolution is checked.
- Do not present approximate geometry as legal boundaries; disputed boundaries need neutral sourcing and a disclaimer before publication.
