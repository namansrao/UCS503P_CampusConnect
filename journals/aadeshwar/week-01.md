# Week 01 — Understand student and society-head journeys

**Member:** Aadeshwar  
**Course week:** 1  
**Reporting window:** 1–7 September 2026  
**Course checkpoint:** Introduction and Pleasantries  
**Workstream:** Frontend / user interface  

## Contribution record

The initial frontend scope is organized around the two main roles: students and society administrators. The student path starts with event discovery, moves through event details and RSVP, then supports people discovery and mutual connection. The society-head path needs society information, event publishing/management, and visibility into event participation. The interface needs a distinct moderation/safety path rather than exposing administrative actions to every user.

## Technical observations

The core product decision is to make the user journey visible and role-oriented. Shared navigation can keep the experience coherent, while the available actions change according to role and resource ownership. Mutual connection is represented as a separate step; seeing a suggested profile does not itself create a connection.

## Verification boundary

The packet defines screen scope and role journeys; it contains no browser captures or dated commit proof for this week. The record therefore documents the product scope, not a claim of a completed visual walkthrough.

## Handover

Carry the student and society-head screen inventory into a single typed React interface and align field names with the API/data model.
