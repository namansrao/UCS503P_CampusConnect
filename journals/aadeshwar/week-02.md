# Week 02 — Choose the web interface and assign screen ownership

**Member:** Aadeshwar  
**Course week:** 2  
**Reporting window:** 8–14 September 2026  
**Course checkpoint:** Group formation, Practise Project Pitch, Accommodate Outliers  
**Workstream:** Frontend / user interface  

## Contribution record

The frontend implementation direction is a single React and TypeScript web interface rather than separate student and administrator applications. The component split in the supplied baseline supports a main campus view, a login view, shared form/modal patterns, and one client request helper. This keeps navigation and interaction conventions consistent while allowing role-specific views.

## Technical observations

The frontend depends on a stable API shape. The shared dashboard response includes the current user, accounts, events, societies, discovery candidates, matches, reports, blocked profiles, and demo/storage mode. The UI can then render role-appropriate controls without duplicating the underlying campus data model.

## Verification boundary

No team meeting record or assignment approval was included in the source archive. The selected interface approach is documented as the packet's implementation direction; teammate agreement is not asserted.

## Handover

Define the visible screens, form fields, empty states, and role-specific controls before implementation.
