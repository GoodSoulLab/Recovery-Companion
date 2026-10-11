# UX simplification notes v0.1

**Date:** 2026-10-11  
**Prototype:** [Context selector v0.5](../../prototype/context-selector-v0.5.html)  
**Status:** Design proposal for expert review; untested

## Decision

Replace the v0.4 first screen's visible choice stack with one plain-language question about the moment the person chooses to address. Offer two fixed starter drafts, explain the matching rule, and make the rest available on request. Keep the static toolkit one step away and use the same 12 exercise drafts in both modes.

This translates the requested design bar into principles rather than copying a specific company's interface: reduce simultaneous choices, make the primary action obvious, keep labels calm and concrete, use progressive disclosure, provide immediate control, and make the interface feel deliberate on mobile.

## What changed

| v0.4 friction | v0.5 response |
|---|---|
| Guided/static tabs, multiple controls, support strip, filters, and three primary actions competed on first screen | One prompt and four self-chosen moment options; full browse is a quieter secondary action |
| A user could stack situation, time, style, and approach filters before seeing anything | One moment routes directly to two fixed draft options |
| Results could produce a dense grid of many cards | Two options appear first; matching drafts expand only if requested |
| The selector explanation lived among other controls | The result names the chosen moment and states that no other information is used |
| Full toolkit used card grid and separate filters | Full toolkit is now a simple expandable list, using the same draft text |
| Visual system mixed serif display, amber alerts, several card treatments, and tight uppercase metadata | System sans typography, restrained palette, consistent rounded surfaces, clear spacing, and stronger mobile hierarchy |

The v0.4 artifact remains in the repository for comparison. No exercise wording was clinically approved by this visual redesign.

## Proposed mechanism

1. The person chooses one of four moments: urge, overwhelm, reflection after a choice, or human support.
2. The interface shows two fixed starter drafts for that moment.
3. It discloses that the pair was selected only from the person's choice and is not ranked.
4. The person may open steps, expand matching drafts, change the moment, or browse all 12 tools.
5. Nothing is saved or sent by the page; no account, analytics, or browser storage is used.

The fixed mappings are transparent rules for testing a selector concept, not a validated recommender. Their fit and perceived authority remain unknown.

## Trade-offs and failure modes

- **Lower initial complexity, more progressive taps:** fewer controls compete initially, but people may need extra taps to see alternatives.
- **Clearer choices, stronger framing effect:** the four moment labels could still prime self-interpretation or feel reductive.
- **Two options reduce scanning, but the starter pair has outsized influence:** a poor pair could bias the experiment. Static comparison and “show more” must remain equally visible in study materials.
- **Fixed mappings are explainable, but arbitrary until reviewed:** clinical and lived-experience reviewers must approve, revise, or reject each mapping before any participant exposure.
- **A quieter interface can hide safety information:** expert-review status remains visible; privacy and safety details stay available in the page. The page must not be represented as care or crisis response.
- **Polish can imply authority:** no efficacy or clinical language was added, and the interface continues to mark every item as an unreviewed draft.

## Verification status

Source-level checks confirm a single HTML document, 12 draft items, JavaScript syntax, and no page-level network, analytics, or browser-storage APIs. These are implementation checks only. The hosted site may receive ordinary connection metadata. Rendered browser, keyboard, zoom/reflow, and screen-reader review remain open, as do qualified clinical, lived-experience, privacy/security, ethics, and IP reviews.

## Decision-critical next check

Ask independent reviewers to compare the exact v0.5 guided path and static toolkit with the same exercise set. Before participant exposure, test whether the two starter mappings feel relevant, understandable, optional, and nonjudgmental. If a well-organized static list works as well or better, retain the static tool or stop the selector work.
