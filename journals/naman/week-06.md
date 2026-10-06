# Week 06 — Review database access and transaction behavior

**Member:** Naman  
**Reporting dates:** 6 October 2026 – 12 October 2026  
**Focus:** Review migration, role boundaries, and transaction-sensitive operations.

## Contribution summary
The database review focuses on the boundary between relational constraints and application-level authorization. The schema assigns role values through a constrained field; society administration is scoped through `society_admins`; messages belong to a match and sender; and reports retain reporter, target, reason, and review state.

The documented transaction design wraps actions in database transactions. RSVP processing locks the event row before counting registrations, preventing two requests from both consuming the last seat. Reciprocal connection operations acquire user-pair locks in a stable sorted order to reduce deadlock risk; message and block operations use the same pair-level coordination model.

## Design outcome
The review distinguishes database-enforced invariants from checks performed by the API. The available project notes describe the transaction strategy, but do not claim a local multi-connection native PostgreSQL concurrency run.
