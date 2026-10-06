# Week 06 — Connect the interface to the API

**Member:** Aadeshwar  
**Course week:** 6  
**Reporting window:** 6–12 October 2026  
**Course checkpoint:** Progress Monitoring  
**Workstream:** Frontend / user interface  

## Contribution record

The login component supports both sign-in and student registration. It uses required email and password inputs, a name field on registration, password length limits, a busy state, and an inline error area. It can also list fictional demo accounts and submit a `demoLogin` action. The `client.ts` helper routes requests either through the browser demo adapter or to the same-origin server API based on `VITE_BROWSER_DEMO`.

## Technical observations

The key integration boundary is consistent endpoint and payload naming: `/api/auth` handles account actions and `/api/campus` handles dashboard reads and application actions. Normal server requests include same-origin credentials so the browser can send the session cookie. The registration UI explicitly discloses that email ownership verification is not connected in this release.

## Verification boundary

The packet includes the login and client source files, but no server logs, live API response capture, or teammate integration review. The entry records the code-level contract and its limits without claiming an end-to-end test.

## Handover

Review the browser adapter and ensure the demo mode uses the same service rules and data model as the server-backed mode.
