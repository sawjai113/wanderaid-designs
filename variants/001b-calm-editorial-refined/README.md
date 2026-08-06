## Variant: Calm Editorial Refined

### Design stance
This keeps Variant 1 as the north star, but makes it more product-real for Wanderaid: warm travel-journal visuals with clearer app actions, collaboration cues, and a dashboard hierarchy that can translate into SwiftUI.

### What changed from Round 1
- **Hero became more actionable:** primary `Open trip` and secondary `Invite people` CTAs now sit directly under the featured current trip.
- **Stats became quieter and more app-like:** compact `People / Places / Notes / Shared` strip replaces the earlier heavier metrics block.
- **Dashboard got a daily anchor:** `Today at a glance` makes the home screen useful immediately, not just pretty.
- **Collaboration is present but calm:** `Shared journal` borrows the activity-feed idea from Variant 3 without becoming chatty or colorful.
- **Trip actions are explicit:** sticky `Join by invite` and `Create trip` actions preserve the real dashboard needs.
- **Past trips remain secondary:** still collapsible, avoiding a dense archive feel.

### Key choices
- **Layout:** featured trip → quiet stats → today → upcoming → shared journal → past trips → sticky actions.
- **Typography:** serif wordmark/display title; system sans for UI readability.
- **Color:** paper/ink foundation, forest-green primary, sand/sky supporting tones.
- **Interaction:** collapsible past trips; obvious app actions; full-screen mobile review.

### Trade-offs
- Strong at: warmth, brand distinctiveness, immediate dashboard usefulness, smooth SwiftUI translation.
- Weak at: power-user density and heavy multi-trip management.

### SwiftUI implementation notes
- Good candidate for a `TripDashboardFeaturedCard`, `TripStatStrip`, `DashboardSectionHeader`, and reusable card shell.
- Keep shared journal/activity purely presentational until real activity data exists.
- The sticky action bar can map to existing create/join flows without changing auth/data behavior.
