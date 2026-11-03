# Week 10 — Consolidate the MST data-model review

**Member:** Naman  
**Reporting dates:** 3 November 2026  
**Focus:** Close the reporting window with a concise data-model explanation and known limitations.

## Consolidated data-model notes
The database uses independent records for users, societies, interests, and events, with association tables for shared interests, event tags, registrations, and follows. Unique and composite keys prevent duplicate identities and relationships. Check constraints restrict roles, years, intent values, capacities, and invalid self-relations. Triggers protect RSVP capacity, event-capacity changes, reciprocal matches, and message eligibility.

## Current limitations at the cutoff
Email verification is not implemented. The prepared test record does not establish a local native PostgreSQL 16 concurrency run, Docker Compose execution, manual browser QA, deployment-scale behavior, load-test results, user-study outcomes, or recommender accuracy. Backup/restore practice and query-plan measurements remain outside the verified implementation record. These are recorded as scope limitations rather than fabricated results or open journal fields.

## Cutoff
This journal package is complete through 3 November 2026. Later course weeks are intentionally excluded from this dated bundle.
