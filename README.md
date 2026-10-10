# Same Earth

**Same planet. A different perspective.**

An independent, curiosity-first project for exploring how Mercator and Equal Earth change the way we see the world.

## Status

Planning stage. This repository contains the product brief, proposed design direction, and infrastructure decisions. There is no runnable website or deployment yet.

## The experience

- Compare two projections of the same geographic dataset, not historical changes in borders.
- Select a country in either view or through a searchable selector; highlight it in both.
- On desktop, compare side by side. On tablet, adapt to legibility. On narrow mobile, switch between projections or choose a stacked comparison.
- Understand what each projection preserves and distorts, with transparent sources.
- Keep exploration free, accessible, and usable without an account.

## Project documents

- [Product brief](PRODUCT.md): scope, behavior, acceptance criteria.
- [Design proposal](DESIGN.md): presentation, responsive behavior, components, accessibility.
- [Infrastructure and funding](INFRASTRUCTURE.md): static hosting, cost boundaries, voluntary support.

## Implementation direction

Vite, vanilla JavaScript, D3 geographic projections, and locally bundled TopoJSON data. No backend, database, paid map API, or payment processing in the application.

Implementation will follow the design brief; these dependencies have not been installed yet.

## Geographic context

Mercator preserves local angles but exaggerates relative area toward the poles. Equal Earth preserves relative area, not every shape, angle, or distance. Neither is universally the best projection for every purpose.

Recent [ABC reporting](https://www.abc.net.au/news/2026-09-05/africa-bigger-us-smaller-united-nations-adopts-new-world-map/107119646) describes a UN resolution urging adoption of Equal Earth. This project is not affiliated with the UN; the original resolution has not yet been independently verified for publication here. No claim is made that all maps must be replaced.

## Contributions

Design and implementation proposals are welcome through issues and pull requests. Preserve geographic accuracy, keyboard access, mobile usability, and the no-backend first-release scope. Do not commit credentials or personal payment information.

## License

MIT for this project's original material. Future third-party code and geographic datasets retain their own licenses and notices.
