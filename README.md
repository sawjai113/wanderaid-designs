# wanderaid-designs

Interactive HTML design explorations for **Wanderaid** (Group Trip App). Every round is a set of throwaway mockup variants you can review from any device — the point is to compare directions, not to ship production code.

## Live site

https://sawjai113.github.io/wanderaid-designs/

## How to review

- Open the live site (or `index.html` locally) — it embeds all variants in phone frames.
- Click **Open full screen** on a variant to try it on a real phone.
- Mockups are interactive: tabs, carousels, collapsible sections, modals.
- All content is fake sample data.

## Variant rounds

### Round 2 — Trip Dashboard refinement

User-selected direction: **Variant 1 — Calm Editorial**.

| # | Stance | One-liner |
|---|--------|-----------|
| 1b | **Calm Editorial Refined** | Keeps the warm travel-journal feel, but adds clearer app actions, a “today at a glance” anchor, quieter stats, and calm collaboration cues. |

Review first: [`variants/001b-calm-editorial-refined/index.html`](variants/001b-calm-editorial-refined/index.html)

### Round 1 — Trip Dashboard (home screen)

| # | Stance | One-liner |
|---|--------|-----------|
| 1 | **Calm Editorial** | Travel-journal warmth: serif type, paper tones, forest-green accent, content-first. |
| 2 | **Utilitarian Dense** | Tool-first console: compact rows, Current/Upcoming/Past tabs, mono numerals, one blue accent. |
| 3 | **Playful Social** | Group-chat energy: avatar stacks, per-feature colors (people purple, places red, chat blue), activity feed, New Trip modal. |

Each variant's `README.md` explains its stance, key choices, and trade-offs.

## Workflow

1. I build 2–3 stances per round from the real app structure.
2. You pick a winner (or a hybrid) after reviewing on any device.
3. The winning direction gets translated into SwiftUI + design tokens.

## Conventions

- Self-contained HTML (inline CSS/JS, system fonts) — opens anywhere, no build step.
- Realistic fake content only, no lorem ipsum.
- Every revision is a commit — history doubles as the design log.
