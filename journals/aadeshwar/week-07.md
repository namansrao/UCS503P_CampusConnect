# Week 07 — Review the first prototype interface

**Member:** Aadeshwar  
**Course week:** 7  
**Reporting window:** 13–19 October 2026  
**Course checkpoint:** Prototype (with Report Submission) – MST  
**Workstream:** Frontend / user interface

## Contribution summary

The supplied React interface brings the main Campus Connect journeys into one application shell. The event area supports search, society filtering, status/sort controls, event details, RSVP and attendee actions, event creation/editing, and calendar export. The profile area supports interest tags, while people discovery provides department and year filters. Society-management and safety/moderation views are also represented in the interface.

The paired stylesheet includes visible keyboard-focus styling, responsive breakpoints for narrower screens, and a reduced-motion rule. The calendar export builds an `.ics` file and escapes text fields before download.

The browser demonstration adapter uses PGlite with IndexedDB persistence, applies the initial SQL schema through a migration marker, seeds fictional demo accounts, and stores the selected demo persona in session storage. It routes demo login and campus actions through the shared dashboard/service functions so the browser demo follows the same application rules without calling the remote API.

## Design and integration notes

Keeping the demo adapter on the shared service functions avoids maintaining a separate set of business rules for the browser presentation. The adapter remains a local demonstration mechanism: fictional data and browser-local storage do not establish production deployment, real account verification, multi-user synchronization, or a production security boundary.

## Verification boundary

The supplied interface and demo-adapter snapshots are documented as dated 14 October 2026. The packet contains no browser walkthrough recording or independent reviewer notes. This entry therefore records source-visible interface scope and demo architecture, not a claim that every flow was manually tested, demonstrated, or accepted. No mobile, keyboard, accessibility, or user testing is claimed from source inspection alone.

## Handover

Use the source-based improvement plan to check keyboard navigation, narrow-screen behavior, focus visibility, reduced-motion handling, loading/error states, and role-specific controls in an actual browser walkthrough.
