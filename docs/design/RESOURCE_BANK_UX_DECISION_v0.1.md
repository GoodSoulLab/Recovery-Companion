# Resource Bank UX decision v0.1

**Date:** 2026-10-14  
**Artifact:** [Resource Bank v0.7](../../prototype/resource-bank-v0.7.html)  
**Status:** Design proposal for review; owner critique is not user research

## Direction

Replace the moment-selector experience with a simple resource bank. The first screen names a few common jobs in plain language, then lets a person browse the same shelf, search it, or save a small set locally. The interaction should feel steady, human, and easy to scan when attention is limited.

The brief draws on broad design principles—clarity, restraint, humane language, craft, and fast feedback. It does not copy a named company's interface, artwork, or components.

## What changed

- Replaced four pictorial choice cards and the two-step fixed recommendations with four plain starting points that filter the bank directly.
- Added nine compact, expandable resources with provenance, time, approach, evidence limitations, cautions, and source links.
- Added an explicit SAA sponsor page: a person can begin with meetings and need not choose a sponsor immediately; peer role and clinical role are distinguished.
- Added a Saved view. Only resource IDs are persisted in browser local storage; no prompt, free text, choices, searches, contact, or behavioral record is stored.
- Disclosed that local storage is not encrypted and can be visible to someone using the same browser profile/device.
- Added a separate evidence and content brief so a qualified reviewer can inspect the claims and questions card by card.
- Retained warm paper/green/clay visual direction, a small abstract path motif, mobile-first layout, reduced-motion support, keyboard focus styles, and simple disclosure interactions.

## Why an evidence-labeled resource bank is the right next slice

The user barrier is starting, finding usable resources, and making human support navigable. A resource bank addresses all three without presuming an algorithmic recommendation is needed. It also provides the strongest static comparator for future testing. The novel part is not the addition of modalities; the product question is whether a carefully organized and transparently described shelf improves the path to an acceptable next step.

## Trade-offs and risks

- **Findable shelf vs long page:** nine items may still overwhelm. The first actions and four categories provide a starting point, but actual scanning needs usability testing.
- **Evidence labels vs false authority:** badges may look scientific even when they say “early.” The detail view qualifies every badge; reviewers should test comprehension.
- **Local persistence vs shared-device exposure:** favorites are useful, but the browser profile can be shared and local storage is not encrypted. Make clearing easy; do not store notes or histories.
- **Human connection vs availability:** the page can make sponsor/meeting options easier to understand but cannot provide a sponsor or guarantee a response.
- **IFS inclusion vs weak direct evidence:** kept as optional exploratory content for transparency, not a default recommendation. Remove it if reviewers judge even bounded self-reflection too risky.
- **Polished presentation vs unreviewed content:** “Preview for expert review” stays visible. Design quality must not imply clinical approval.

## Hypothesis

For adults voluntarily seeking change in unwanted sexual behavior, a short, evidence-labeled resource bank with optional local saving will help them identify one acceptable next step and understand the roles of skills, peer support, and professional care better than an unstructured search or resource list, without increasing shame, pressure, or privacy misunderstanding.

This is a usability and comprehension hypothesis, not a claim of clinical benefit.

## Verification status

Source code checks confirm nine resource entries, valid JavaScript syntax, local storage limited to saved resource IDs, no fetch/XMLHttpRequest code, and reduced-motion handling. Source checks do not verify actual browser privacy guarantees, screen-reader quality, visual behavior on devices, local storage exposure, or the clinical safety and usefulness of the drafted cards. Those gates remain open.
