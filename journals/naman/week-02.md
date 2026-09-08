# Week 02 — Establish PostgreSQL as the relational data store

**Member:** Naman  
**Reporting dates:** 8 September 2026 – 14 September 2026  
**Focus:** Define how the domain entities relate and how shared interests are represented.

## Contribution summary
The database design uses PostgreSQL as the relational persistence layer. Users, societies, and events have independent identities; relationship data is represented through association tables such as `user_interests`, `event_interests`, `rsvps`, and `follows`. A shared `interests` vocabulary keeps profile interests and event tags consistent.

## Design outcome
Primary keys identify records, foreign keys preserve relationships, and composite keys prevent duplicate association rows. Role, year, intent, capacity, and content checks are represented as database constraints in the schema baseline.

## Scope note
The entry documents the selected relational approach and the model represented in the packet. It does not claim a production deployment or a native PostgreSQL service run for this week.
