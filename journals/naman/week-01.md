# Week 01 — Identify the persistent data

**Member:** Naman  
**Reporting dates:** 1 September 2026 – 7 September 2026  
**Focus:** Inventory the persistent information required by the campus community app.

## Contribution summary
The data scope is organized around users and roles, societies and their administrators, events and registrations, interests, follows, connection requests and matches, messages, blocks, reports, and login sessions. The model separates core entities from many-to-many relationships so the same interest vocabulary can be reused by people and events.

## Design outcome
The initial data inventory provides a clear boundary between identity, community activity, event participation, social connections, communication, and moderation. The relational table dictionary is consolidated in `docs/database.md` and the schema baseline is in `code/campus-connect/database/001_initial.sql`.

## Scope note
This entry records the database contribution scope; it does not invent a commit identifier, teammate review, or external approval.
