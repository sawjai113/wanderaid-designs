## Variant: Calm User Dashboard

### Design stance
The main page is no longer only a trip landing page. It is the current user’s dashboard: what needs their attention, what they owe or are owed, and the fastest path into the current/next trip or the full trip archive.

This keeps the Calm Editorial visual direction — paper tones, serif display type, forest-green accent, quiet cards — while changing the information hierarchy around the user.

### What changed from Round 2
- **Removed upper-left W logo:** the header now starts with the Wanderaid wordmark and sync/greeting context.
- **Moved create/join actions:** `Create trip` and `Join by invite` now live inside the top-right profile dropdown.
- **Added bottom navigation:** three primary destinations: `Dashboard`, `Current`, and `All Trips`.
- **Reframed the page around the user:** the headline, surfaced metrics, money summary, and attention list are user-centered instead of trip-centered.
- **Removed the oversized dashboard intro:** the page now starts directly with the current/next trip card to preserve space.
- **Shrunk the featured trip card:** the card keeps visual prominence while leaving more room for dashboard content above the fold.
- **Anchored the bottom nav:** the nav is attached to the bottom edge instead of floating above content.
- **Changed “spent” semantics:** the money module now shows the user’s net outstanding balance, with drill-in rows for “owed to you” and “you owe.”
- **Kept the large current/next trip card:** the current trip still visually anchors the page, but its surfaced detail is about what the user needs to do next.
- **Kept past trips easy to find:** past trips stay on the dashboard as a collapsible section, and there is a permanent All Trips bottom-nav entry.

### Key dashboard modules
1. **Featured current/next trip card** — still prominent and emotional, but more compact and with a user task/decision CTA.
2. **Your money across trips** — net outstanding, owed-to-you, and you-owe rows.
3. **User metrics** — decisions, invites, and next-trip countdown.
4. **Needs your attention** — actionable cross-trip tasks.
5. **Current & next trip list** — direct entry points into active travel.
6. **Past trips** — easy access without dominating the screen.
7. **Profile dropdown** — create/join/account actions.
8. **Bottom nav** — dashboard/current/all trips.

### Open UX questions
- Should the money card show net outstanding first, or split “You owe” and “Owed to you” equally?
- Should the dashboard include unread messages/activity, or only actionable items?
- Should “Current” in the bottom nav mean the current trip only, or current/next trip depending on trip state?
- Is “All Trips” enough for past-trip discovery, or should past trips remain visible on the dashboard long-term?

### SwiftUI implementation notes
- Dashboard data should probably be backed by a user-focused view model/derived summary, not raw trip totals.
- Money rows should deep-link into an expense/balances view filtered by trip or participant.
- The profile dropdown can map to existing create/join flows while avoiding persistent bottom CTAs.
- Bottom nav likely means a small navigation architecture decision before implementation.
