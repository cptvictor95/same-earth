# Infrastructure and funding

## Goal

Run the project at near-zero cost, with a clear path to voluntary support if traffic grows.

## Hosting: static site, no backend

The first release is a static Vite build: HTML, CSS, JavaScript, and a bundled TopoJSON file. Nothing needs a server, database, or paid map API.

**Recommended host: Cloudflare Pages, Free plan**, connected to this GitHub repository. Limits checked on the official limits page (last updated 2026-09-05):

| Resource | Free plan limit |
|---|---|
| Builds | 500 per month; one build at a time |
| Files per site | 20,000 |
| Single file size | 25 MiB |
| Custom domains | 100 per project |
| Preview deployments | Unlimited active |
| Projects per account | 100 |

The site's bundle should stay far below these limits. The page did not list a bandwidth cap; confirm current bandwidth terms on the Cloudflare plans page before launch.

**Alternative:** GitHub Pages for a public repository. Not evaluated in detail yet; check its current bandwidth and usage policies before choosing it.

## Recurring costs

| Item | Expected cost |
|---|---|
| Repository | Free (public GitHub repository) |
| Hosting | Free tier (above) |
| Domain name | Optional; the only likely recurring cost if you add one |
| Donation platform | Free to set up; fees depend on provider |

Keep the project on free hosting until real traffic makes a limit relevant. Revisit then, rather than preparing paid infrastructure now.

## Voluntary support

Possible sources, with the constraints verified so far:

- **GitHub Sponsors:** GitHub states it charges no fees on sponsorships from personal accounts. Eligibility requires living in a supported region and applying through GitHub. Verify the current application status before relying on it.
- **Other platforms** (for example, Ko-fi or Open Collective): not yet verified for fees, payout regions, or tax treatment. Verify before adding a donation button.

Donations are voluntary support for the project's running costs, not charitable donations unless you set up a registered charity or fiscal sponsor. Check tax treatment in your jurisdiction before presenting them as tax-deductible.

## Implementation rule

Add a single "Support this project" link to the site footer only after the first working release. No payment code, donor accounts, or third-party payment scripts are added to the application.

## Data sources

- Geographic data: World Atlas TopoJSON derived from Natural Earth 4.1.0 (ISC-licensed package; Natural Earth data is public domain per its terms). Record the exact version and checksum when the data is first bundled.
