# Variant 005 — Calm Basecamp Clickable Prototype

## What this is

A single self-contained HTML prototype for the Wanderaid v1 product brief and seven-room basecamp model.

Open locally:

```sh
open /Users/sawjai/Documents/wanderaid-designs/variants/005-calm-prototype/index.html
```

## Included screens and flows

- Home — user lens with live ticking countdown, action-needed calls, grouped feed, and personal money glance.
- Welcome Desk — per-trip lobby with countdown, place/date, crew avatars, invite code, group chat entry, room navigation, and trip activity.
- Map Wall — map-like POI surface, filter chips, weighted votes, call-for-vote item, and locked-in marker linking to Schedule Board.
- Schedule Board — day-grouped flight/hotel/activity timeline with participant chips and undated backlog.
- Crew — dorm hall list; tapping a person opens their room with role, money status, arrival/departure, places/expenses/bookings/votes summary, and message button.
- Kitty — expenses, user-first balances, quick-add affordance, and toggled repayment plan.
- Journal — guest-book entries, external album link, and chat link.
- Chat — trip channel thread plus cross-trip direct message list.

## Interactions

- Bottom nav and room cards navigate between screens.
- Right-side flow chips navigate directly to each room.
- Countdown ticks once per second.
- Map Wall vote buttons update score/counts in place using: yes +1, weak yes +0.5, no -1, abstain not counted.
- Crew rows open person detail rooms.
- Kitty repayment button toggles expense list vs repayment plan.
- Unread dots appear on action-needed rooms and chat entries.

## Design stance

Calm Editorial light mode, matching the existing Wanderaid direction:

- Warm paper background: #F7F2E8.
- Card surface: #FFFDF8 with #E6D9C6 hairline borders.
- Forest actions: #2F684E / #1F4F39.
- Sand and terracotta accents for highlights and owed states.
- Serif moments only for emotional numbers and room titles.
- Low-noise navigation; rows and cards are tappable surfaces rather than button-heavy layouts.

## Notes for app translation

- This is a design artifact, not production code.
- The prototype assumes first-release scope from `docs/product-brief.md`: basic in-app chat, live countdowns, grouped activity feeds, action-needed, weighted POI votes, schedule bookings, quick-add expenses, and guest book.
- It intentionally keeps visual polish inside the Calm Editorial system while surfacing the new information architecture clearly for review.
