# Week 11 — Consolidate the database contribution

**Member:** Naman  
**Course week:** 11  
**Reporting dates:** 4 November 2026 – 10 November 2026  
**Focus:** Consolidate the database workstream into a clear, repository-ready technical record.

## Contribution summary

The database contribution is organized around a normalized relational model for users, societies, interests, and events. Association tables represent shared interests, event tags, registrations, and follows. The supplied schema uses primary and foreign keys, unique constraints, composite keys, and check constraints to protect identity, relationship integrity, allowed values, capacities, and invalid self-relations.

## Database behavior and query coverage

The existing SQL artifacts cover representative joins and aggregations, event occupancy ranking with a window function, and a CTE-based matching query. Trigger logic is documented for RSVP capacity, event-capacity changes, reciprocal matching, and message eligibility. The notes distinguish database-level integrity rules from validation and authorization that belong in the application layer.

## Verification boundary

This consolidated record is based on the supplied schema, query, seed, testing, and design-note files. It does not claim a new database migration, a fresh local execution, or a successful concurrency test during this reporting window. Native PostgreSQL 16 concurrency behavior, Docker Compose execution, deployment-scale performance, load-test results, backup/restore practice, and measured recommender accuracy remain outside the evidence in the packet.

## Outcome

The database contribution is documented as a coherent set of source artifacts and technical explanations. No Git commit hash, pull-request URL, teammate approval, or assessor feedback is fabricated.
