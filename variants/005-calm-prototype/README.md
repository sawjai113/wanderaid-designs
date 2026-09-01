# Variant 005 — Calm Trip Clickable Prototype

## What this is

A single self-contained HTML prototype for the Wanderaid v1 product brief and trip information architecture. The basecamp/room metaphor remains internal design language; the visible UI now uses plain user-facing page names.

Open locally:

```sh
open /Users/sawjai/Documents/wanderaid-designs/variants/005-calm-prototype/index.html
```

## Included screens and flows

- Home — user lens with live ticking countdown, action-needed calls, grouped feed, and personal money glance.
- Trip Overview — per-trip landing page with photo hero, compact single-box countdown, place/date, people avatars, group chat entry, trip sections, and activity.
- Places — map-like POI surface, filter chips, weighted votes, call-for-vote item, and locked-in marker linking to Itinerary.
- Itinerary — fixed-size monthly calendar view with event markers, selected-day details, participant chips, and undated backlog.
- People — traveler list; tapping a person opens their detail view with role, money status, arrival/departure, places/expenses/bookings/votes summary, and message button.
- Money — expenses, user-first balances, quick-add affordance, and toggled repayment plan.
- Memories — guest-book entries, external album link, and chat link.
- Chat — trip channel thread plus cross-trip direct message list.

## Interactions

- Bottom nav and trip-section cards navigate between screens.
- Right-side flow chips navigate directly to each page.
- Countdown ticks once per second.
- Places vote buttons update score/counts in place using: yes +1, weak yes +0.5, no -1, abstain not counted.
- People rows open person detail views.
- Money repayment button toggles expense list vs repayment plan.
- Unread dots appear on action-needed items and chat entries, vertically centered in list rows.

## Design changes from the first 005 pass

- Replaced internal room names in the visible UI with normal page names: Trip Overview, Places, Itinerary, People, Money, Memories, and Chat.
- Added a photo hero to the trip landing page so each trip can carry its own visual feel.
- Added visible image affordances for both supported cover-image inputs: upload photo and use image URL.
- Reworked Home’s “Needs your attention” and “Grouped feed” into shared list containers with toned-down rows and hairline dividers, so each header reads as one section containing multiple items.
- Applied the same grouped-list treatment to Trip Overview’s activity feed.

## Design changes from this feedback pass

- Center-aligned the red unread/action dots on list rows, especially in “Needs your attention.”
- Changed countdowns from four separate cards into one shared compact countdown box with four units inside.
- Removed the persistent invite-code row from Trip Overview and moved it to the top of People, where inviting participants naturally lives.
- Reduced the bottom navigation bar height and padding so it takes up less vertical space.

## Design changes from the Itinerary calendar pass

- Replaced the top Itinerary day-by-day timeline with a fixed-size monthly calendar.
- Added day markers for travel/stay, activities, and needs-input items so longer trips do not expand the primary overview vertically.
- Kept detailed plans in a selected-day list below the calendar, plus the existing undated backlog.

## Design stance

Calm Editorial light mode, matching the existing Wanderaid direction:

- Warm paper background: #F7F2E8.
- Card surface: #FFFDF8 with #E6D9C6 hairline borders.
- Forest actions: #2F684E / #1F4F39.
- Sand and terracotta accents for highlights and owed states.
- Serif moments only for emotional numbers, trip names, and major page titles.
- Low-noise navigation; rows and cards are tappable surfaces rather than button-heavy layouts.

## Notes for app translation

- This is a design artifact, not production code.
- The prototype assumes first-release scope from `docs/product-brief.md`: basic in-app chat, live countdowns, grouped activity feeds, action-needed, weighted POI votes, calendar-based itinerary bookings, quick-add expenses, and guest book/memories.
- The app should keep using user-facing labels in product surfaces while preserving the basecamp/room metaphor as internal design framing.
