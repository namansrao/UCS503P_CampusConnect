# Week 08 — Write the interface improvement plan

**Member:** Aadeshwar  
**Course week:** 8  
**Reporting window:** 20–26 October 2026  
**Course checkpoint:** Improvement Plan - CE  
**Workstream:** Frontend / user interface  

## Contribution record

A source-based improvement plan is included as a separate document. Priority areas are keyboard-only navigation through tabs, filters, dialogs and forms; verifying the 780px and 560px layouts; confirming visible focus and reduced-motion behavior; and checking empty, loading and error states. The plan also calls for testing that long event titles, bios, messages and validation errors remain readable on small screens.

## Technical observations

The existing CSS already contains focus-visible rules, responsive breakpoints and a reduced-motion media query, so the next step is verification and targeted fixes rather than assuming those rules are sufficient. The main app refreshes data after mutations and polls messages while the messages tab is active; these are interaction behaviors worth checking under slow or failed network conditions.

## Verification boundary

This is a proposed improvement plan derived from the supplied source. It does not claim that keyboard, mobile, accessibility or user testing has been performed.

## Handover

Use the plan to create a short, repeatable prototype walkthrough and record observations only after actually running it.
