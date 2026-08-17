# wanderaid-designs

Interactive HTML design explorations for **Wanderaid** (Group Trip App). Every round is a set of throwaway mockup variants you can review from any device — the point is to compare directions, not to ship production code.

## Live site

https://sawjai113.github.io/wanderaid-designs/

## Selected direction

The selected app direction is the **Calm User Dashboard** in the Calm Editorial visual language. Light and dark mockups are ready to use as implementation references for the Wanderaid app.

The earlier Utilitarian Dense and Playful Social variants are no longer shown in the gallery so future work can focus on the approved direction.

Implementation tracking:

- App spec: `Group Trip App/docs/plans/calm-user-dashboard-design-direction.md`
- GitHub issue: https://github.com/sawjai113/GroupTrip/issues/1

### Round 3 — Calm User Dashboard

User feedback shifted the home page from a trip-centered landing page to a current-user dashboard.

| # | Stance | One-liner |
|---|--------|-----------|
| 1c | **Calm User Dashboard** | Keeps the tappable current/future trip card and past-trip access, but surfaces user-centered info: net outstanding balance, decisions, personal actions, profile-menu create/join, and bottom navigation. |
| 1d | **Calm User Dashboard Dark** | Same dashboard structure translated into warm dark surfaces with cream typography, subdued borders, and forest-green highlights. |

Review first:

- Light: [`variants/001c-calm-user-dashboard/index.html`](variants/001c-calm-user-dashboard/index.html)
- Dark: [`variants/001d-calm-user-dashboard-dark/index.html`](variants/001d-calm-user-dashboard-dark/index.html)

Key design decisions:

- The current trip card remains visually prominent, but the whole card is tappable instead of using internal buttons.
- The old trip-level “spent” metric becomes a user-level **net outstanding** card.
- Drill-in rows split money into **Owed to you** and **You owe** across trips.
- **Needs your attention** appears above the money card so actionable items lead.
- Create/join actions move into the top-right profile dropdown.
- Bottom navigation introduces `Dashboard`, `Current`, and `All Trips`, anchored to the bottom edge.
- Past trips stay easy to find, but no longer compete with the primary user dashboard.
- Dark mode should preserve the same information hierarchy instead of becoming a separate layout.

## Prior calm references

### Round 2 — Trip Dashboard refinement

| # | Stance | One-liner |
|---|--------|-----------|
| 1b | **Calm Editorial Refined** | Warm travel-journal feel with clearer app actions, a “today at a glance” anchor, quieter stats, and calm collaboration cues. |

Reference: [`variants/001b-calm-editorial-refined/index.html`](variants/001b-calm-editorial-refined/index.html)

### Round 1 — Trip Dashboard exploration

| # | Stance | One-liner |
|---|--------|-----------|
| 1 | **Calm Editorial** | Travel-journal warmth: serif type, paper tones, forest-green accent, content-first. |

Reference: [`variants/001-calm-editorial/index.html`](variants/001-calm-editorial/index.html)

## How to review

- Open the live site (or `index.html` locally) — it embeds the current calm variants plus prior calm references in phone frames.
- Click **Open full screen** on a variant to try it on a real phone.
- Mockups are interactive: profile menu, tappable current trip card, and collapsible past trips.
- All content is fake sample data.

## Workflow

1. I build/refine the selected direction from the real app structure.
2. You review on any device and call out what feels right/wrong.
3. Once the mockup feels close, the winning direction gets translated into SwiftUI + design tokens.

## Conventions

- Self-contained HTML (inline CSS/JS, system fonts) — opens anywhere, no build step.
- Realistic fake content only, no lorem ipsum.
- Every revision is a commit — history doubles as the design log.
