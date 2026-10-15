# Recovery Companion — UX direction decision v0.4

**Date:** 2026-10-15  
**Status:** Design iteration for review; unvalidated and not cleared for participant use  
**Prototype:** [`resource-bank-v1.1.html`](../../prototype/resource-bank-v1.1.html)  
**Previous direction:** [`RESOURCE_BANK_UX_DECISION_v0.3.md`](./RESOURCE_BANK_UX_DECISION_v0.3.md)

## Decision

Reduce the opening screen from four situation cards to two useful actions: **Try a short practice** and **Find people & care**. Keep **Browse all resources** immediately available. Retain the path-map illustration, full searchable resource shelf, evidence and scope notes, external links, and optional local saving. Remove the visible saved-item count from navigation.

This is a testable interaction hypothesis, not evidence of clinical or recovery benefit. MetaLab, Dieter Rams, and Jony Ive are design references requested by the product owner; none has designed, reviewed, or endorsed this work.

## Why simplify

The v1.0 opening asks a person to distinguish among four overlapping situations before they can see the resources. The shelf then asks them to classify by five filters, and navigation repeats routes to the shelf and saved list. In a sensitive, possibly time-pressured moment, those decisions may feel like effort or imply that the person must label their state correctly. That is a design risk inferred from the interface, not a finding from users.

Two doors make the first decision more legible: a self-guided practice or human support. The complete shelf remains a single action away for people who do not want either suggested route. The “people & care” shelf filter still exposes separate meeting, peer sponsor, and professional-care resources; combining their entry point does not combine their roles.

## What changed

- Replaced four numbered situation cards with two plain-language actions and shorter explanations.
- Preserved a direct browse-all path, all resource content, filter/search behavior, citations, cautions, and official outbound links.
- Kept the illustrated path map and the existing calm, locally rendered Dojo-inspired visual language; no external fonts, imagery, or scripts were added.
- Removed the saved-resource count from the persistent navigation because a count on a shared screen can itself disclose engagement with this sensitive topic.
- Kept optional saving in browser storage. Only resource IDs are persisted; they are not encrypted and may be visible to other users of the same browser profile/device. The page does not claim that ordinary hosting metadata, browser history, or backups are under its control.
- Shortened the visible expert-preview status while retaining the boundary that drafts are not care and require clinical and lived-experience review before participant use.

## Verified implementation facts

The current source contains ten resource records; the two actions route to existing shelf filters rather than generating advice or ranking a person. Browse-all resets to the full shelf. The local save routine stores only resource IDs. Outbound resources remain direct links with `noopener noreferrer` and `no-referrer`; the page has no analytics or application backend requests. These are source-level observations, not independent runtime, privacy, or clinical validation.

## Hypotheses and open risks

| Hypothesis or risk | What could be wrong | Evidence needed |
|---|---|---|
| Two choices reduce decision effort | The four choices may better match distinct needs; “practice” may feel too narrow | Counterbalanced findability and navigation observations |
| The two actions cover the reasons people arrive | Some may want information, a personal recovery practice, or an immediate directory without either label | Observe the browse-all path and collect non-disclosing feedback |
| “People & care” is clear | Pairing these terms could blur peer support and clinical care | Ask participants to explain sponsor, meeting, and therapist roles after use |
| A hidden count improves discretion | The persistent “Saved” label still discloses interest; local storage remains discoverable | Privacy teach-back and shared-device review |
| The opening feels calmer | Strong primary-button styling may over-direct users toward a practice | Measure agency, perceived pressure, and task choice; remove visual primacy if it steers |

The resource curation, evidence provenance, careful boundary language, and maintenance discipline may make this more useful than a generic directory. That remains unproven. Visual polish, a modality list, and integration alone are not a defensible product thesis. A well-organized static page may be sufficient.

## Smallest useful falsification experiment

After the clinical, lived-experience, privacy, accessibility, IP, and ethics review gates in v0.3, run eight moderated formative sessions with adults who self-identify as voluntarily exploring change in unwanted sexual behavior. Use fictional, non-graphic scenarios, collect no explicit behavioral history, and let participants skip or stop. Counterbalance this version against a flat shelf with identical content.

Ask participants to find (1) one acceptable short practice, (2) official meeting or sponsor guidance, and (3) professional-care search resources. Record time, errors, route chosen, and whether participants felt pushed toward a practice. Test understanding of the distinction between peer and clinical support and of local saving. Do not combine these measures into a score or interpret task success as recovery benefit.

Do not advance the two-action home if it fails to improve paired findability versus the flat shelf, if two or more of eight participants mistake the labels for assessment or prescribed treatment, or if two or more misread sponsor and therapist roles. Pause and review if a participant experiences notable shame or distress plausibly caused by the framing. These are formative design stop signals, not statistical thresholds or evidence of effectiveness.

This experiment can falsify a navigation assumption. It cannot show behavior change, clinical benefit, safety across populations, superiority to therapy or fellowship, market demand, or whether the curation warrants a standalone product.

## Release boundary

The preview remains owner-only. It is for product review, not public distribution or participant use. Clinical and lived-experience approval, privacy/security review, accessibility review, link verification, IP review, and ethics/consent planning remain open gates. No company, diagnosis, abstinence goal, user account, sensitive profile, location collection, tracking, sponsor matching, or automated clinical recommendation is implied by this design.
