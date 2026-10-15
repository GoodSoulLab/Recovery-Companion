# Recovery Companion — UX direction decision v0.2

**Date:** 2026-10-15  
**Status:** Working prototype and testable design hypothesis; not clinical approval or user validation  
**Prototype:** [`resource-bank-v0.8.html`](../../prototype/resource-bank-v0.8.html)  
**Previous direction:** [`RESOURCE_BANK_UX_DECISION_v0.1.md`](./RESOURCE_BANK_UX_DECISION_v0.1.md)

## Decision

Advance a **moment-led pocket guide** as the next prototype, while keeping the full resource shelf one tap away. The opening screen offers four self-chosen starting points, not a diagnosis, score, personalized recommendation, or prescribed recovery path. People can browse everything, expand a card to inspect its evidence and limits, and optionally keep resource IDs in the browser.

This is a design direction to test, not a conclusion that this interaction improves recovery. The current content remains draft material for clinical, lived-experience, privacy, accessibility, and intellectual-property review before any participant-facing study.

## Design intent

The brief's references to MetaLab, Dieter Rams, and Jony Ive are interpreted as a quality bar around clarity, restraint, coherence, tactility, and careful detail. No named person or studio designed, endorsed, or reviewed this prototype; its work and recognizable visual signatures are not copied.

The interface aims to feel calm without making the topic cute or minimizing distress. Short labels and optional steps reduce the first decision. Quiet visual hierarchy distinguishes user action from evidence context. Movement is decorative, slow, and disabled under reduced-motion preference. The work is code-native and uses no remote fonts, trackers, accounts, or network-loaded assets.

## What changed from v0.7

- The first screen presents four plain-language situations, followed by a direct route to browse the entire shelf.
- The opening screen distinguishes three kinds of support—practice, people, and care—without implying that one should replace another.
- The resource shelf remains directly available, with category filters, search, expandable cards, evidence explanations, cautions, and source links.
- Optional saving is renamed “My pocket” and persists only saved resource IDs. It does not collect notes, contact details, histories, searches, choices, or behavior records. The interface states that local storage is not encrypted and can be visible to someone using the same browser profile or device.
- The sponsor resource preserves choice and pacing; it frames sponsors as peer guides and separates their role from licensed clinical care.
- IFS-inspired content is explicitly optional and exploratory. It does not invite trauma memory work and is not presented as established care for this use.

The four entry choices are routes to content, not clinical triage. No recommendation is generated from a person's answers. Every route can be bypassed, and no recovery goal is assumed.

## Options and trade-offs

| Direction | Benefit | Cost or risk | Decision |
|---|---|---|---|
| **A. Flat resource shelf** (v0.7) | Lowest interaction complexity; evidence and scope stay visible; strongest simple comparator | Makes a person scan and classify nine items before acting; may feel like homework during a difficult moment | Keep as the control experience and always-available browse route |
| **B. Moment-led pocket guide** (v0.8) | Gives a low-effort starting choice while preserving access to the shelf; no profile or algorithm required | Situation labels may not fit, imply the person is in crisis, or sort them into a recovery narrative; added navigation can hide content | Test next, with an explicit browse-all route and easy exit |
| **C. Personalized recovery map** | Could better reflect a person's chosen fellowship, clinician, boundaries, and support gaps | Requires sensitive preference/contact data, more setup, and assumptions about “fit”; risks turning a private guide into tracking, pseudo-clinical matching, or a substitute for human care | Defer; no evidence currently justifies the added data and risk |

The moment-led route is a reversible interface hypothesis. If it does not outperform the flat shelf on findability without lowering agency or increasing shame, return to the simpler shelf.

## Challenge to the product thesis

A curated, private resource bank may reduce the work of finding an appropriate next step. That is plausible, but unproven. A clean interface cannot establish clinical value, and a list of named modalities is neither a novel capability nor a defensible advantage by itself.

The strongest potential differentiation is an **operating capability**, not a visual moat: transparent provenance for each resource; disciplined review and revision; clear boundaries between peer and clinical support; and respectful pathways across a person's chosen recovery supports. Whether this curation is meaningfully more useful than a reputable directory, a printed handout, or a well-organized static web page is still an open question. Privacy can be a trust requirement without being a unique selling point.

The current browser-local save is also a trade-off, not a complete privacy solution. It avoids a service-side record, but another user of the same device/browser can see saved IDs. The prototype should not imply encrypted, anonymous, or universally safe use.

## Falsifiable next experiment

### Question

Compared with the same resources in a flat, well-organized shelf, do moment-led entry choices help adults who are themselves seeking change find an acceptable resource faster, without reducing perceived agency or increasing shame, distress, or misunderstanding of evidence and privacy?

### Smallest useful study

After clinical/lived-experience and privacy/accessibility review, run **eight moderated, paid formative sessions** with adults (18+) who self-identify as voluntarily exploring change in unwanted sexual behavior. Do not screen for diagnosis or collect explicit behavioral details. Use fictional, non-graphic scenarios; participants may skip any task or stop. Counterbalance which interface is seen first. Compare the moment-led prototype with a stripped-back flat shelf containing identical resources and evidence language.

Tasks should cover: finding an optional in-the-moment exercise; locating sponsor-fit guidance without treating a sponsor as a clinician; and explaining what “early” or “exploratory” evidence does and does not mean. Include a brief privacy teach-back about local saving. Do not ask participants to disclose their own behavior, trauma history, fellowship status, or clinician.

### Pre-registered decision signals

Treat the moment-led hypothesis as **not supported** if any of these occur:

- Fewer than 7 of 8 participants independently reach a resource they consider acceptable within 90 seconds on the moment-led screen; or it does not improve paired findability versus the flat shelf.
- Two or more participants interpret an entry choice as a diagnosis, mandated abstinence path, or crisis assessment.
- Two or more believe an evidence label proves the card itself is clinically validated, or believe a sponsor is a licensed care provider after using the relevant content.
- Two or more believe local saving is encrypted, invisible to other device users, or transmitted to a clinician/service.
- Any participant experiences notable shame or distress plausibly caused by the framing; pause and review before further sessions.

These thresholds are screening signals for design failure, not statistical evidence of effectiveness. Keep task success, time, navigation errors, comprehension, agency, distress, and participant suggestions separate in the readout; do not combine them into a recovery score.

### What this experiment can establish

It can identify whether the interaction is understandable, usable, and acceptably framed for a small group. It cannot demonstrate behavior change, clinical benefit, safety across populations, superiority to therapy/fellowship, or commercial demand. If moment-led routing does not improve findability, remove the routing layer and retain the well-organized shelf. If the content itself fails evidence or safety review, redesigning navigation cannot rescue it.

## Review gates before participant exposure

1. Clinical review of each card's wording, scope, contraindications, and evidence characterization.
2. Lived-experience review with people from more than one recovery orientation; include people who reject diagnostic or abstinence framing.
3. Privacy and security review of browser storage, shared-device language, and data-flow claims.
4. Accessibility review including keyboard, screen reader, zoom, color contrast, reduced motion, and mobile layouts.
5. IP review to confirm all practice text is original and source links are not presented as endorsement.
6. Ethics review of recruitment, consent, distress handling, compensation, data minimization, and retention.

## Verification status

Source-level checks cover JavaScript syntax, all four routes, resource/filter mappings, the saved-ID-only persistence path, the no-network behavior, and reduced-motion handling. These checks do not validate clinical content, actual assistive-technology behavior, all browser privacy properties, usability, or outcomes. The private preview is for product review and is not approved for public distribution or participant use.
