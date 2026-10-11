# Prototype Privacy Threat Model v0.1

**Status:** Source-level assessment of prototype v0.4; not a security audit, privacy review, or claim of confidentiality.  
**Scope:** Static prototype in `prototype/context-selector-v0.4.html` and the later study boundary.  
**Purpose:** Make the data boundary concrete before any participant exposure.

## Decision

The prototype has a small data footprint: the user makes no account, types no personal story, and the JavaScript does not intentionally send or persist selector inputs. That is a useful design constraint, but it does **not** make use anonymous or confidential. When served from a public host, the page request can expose ordinary connection metadata to that host. A shared or managed device can also reveal use through browser history, screenshots, extensions, or observation.

Keep the demo expert-review only. Do not collect participant data or put personal, health, or confidential content in this public repository.

## Data-flow boundary

| Stage | Data or event | Current behavior | Residual exposure / status |
|---|---|---|---|
| Open prototype | Request for the static HTML document | Page source contains no external script, image, font, or stylesheet dependency. | The public host receives a document request and may process connection metadata under its own practices. Host logging, retention, cookies, and account state have not been inspected or verified here. |
| Use selector | Situation, time, format, and approach selections | Held in page memory; no account, backend, analytics, free-text input, browser storage, or outgoing request API found in source. | Visible to someone with access to the open page, browser process, device, extensions, screen capture, or remote administration. Inputs are sensitive in context even if not saved by the page. |
| Change or leave | Clear filters, exit, or reload | Clear/exit removes displayed results; reload clears in-page state. | Browser history still shows the page. Clearing page state does not erase host request logs, screenshots, backups, or device-management records. |
| Review source | Public repository access | Prototype and draft product materials are in a public, MIT-licensed repository. | Anyone can read and reuse repository material within that license. Do not commit private narratives, reviewer identities, participant data, credentials, restricted curricula, or material intended to remain proprietary. |
| Future research | Task choices, timing, fit/agency/privacy ratings | Not collected by this prototype. | Any such record could reveal participation in a sensitive study. It needs a separate approved protocol, secure collection path, retention/deletion plan, and access controls. |

## Threat register

| Threat | Current control | Residual risk | Required response before participant use |
|---|---|---|---|
| Context selections are transmitted or retained by the page | No network APIs or persistent browser storage found; no free-text field or account. | A later code change, external script, or deployment wrapper could add collection. Source inspection is not runtime verification. | Test the exact delivered build in a clean browser; verify network activity during load and interaction; inspect storage before and after; repeat after material code changes. |
| Another person sees the page or selected options | No notification, sharing, or automatic contact behavior. User can clear/exit. | Shared devices, shoulder-surfing, browser history, screen capture, extensions, and managed-device software remain outside the page’s control. | Use neutral page title and copy; provide honest context before participant use; do not claim “private,” “anonymous,” or “confidential.” Allow the person to decline or close the page. |
| Public hosting exposes access metadata | Static page has no embedded third-party assets or intentional telemetry. | Host request records and associated account/browser/network metadata are outside this prototype’s control and have not been verified. | Review the selected host’s current logging, retention, cookies, and privacy terms before a study; choose a host and setup consistent with the approved protocol. |
| Drafts or product IP are copied from the public repository | Current exercises are labeled as original drafts; competitor curricula are not reproduced. | The repo’s MIT license permits broad reuse of its covered materials. Rights to future content may differ. | Check provenance and rights for every card. Revisit repository licensing before adding content that must remain proprietary or is third-party/restricted. |
| Future study records create a sensitive behavioral dossier | No study collection is implemented. Prior test plan excludes diagnoses, histories, free-text accounts, recordings, and longitudinal logs. | Even scenario responses, choice IDs, timing, or study participation can be sensitive when linked to identity. | Complete privacy, ethics, clinical, and lived-experience review. Keep consented study data separate from the product; minimize fields, unlink identity, restrict access, and define deletion/retention before recruitment. |

## Minimum controls for the next phase

Before any participant-facing test:

1. Have a privacy/security reviewer inspect the exact release artifact and hosting path.
2. Verify runtime requests and browser storage on the delivered artifact; do not rely on source scans alone.
3. Provide an accurate plain-language data notice that distinguishes page behavior from host and device behavior.
4. Approve a separate study data-flow map, consent/debrief, collection method, access list, retention schedule, deletion method, and response plan.
5. Confirm the public repository license and all content rights are acceptable for the intended use.
6. Complete the required clinical, lived-experience, accessibility, and ethics review of exact content and procedures.

## Verification completed

A source-level scan of v0.4 found no `fetch`, `XMLHttpRequest`, `sendBeacon`, WebSocket, local/session storage, IndexedDB, or remote script/image/font/style references. The card registry and interaction code are static. This finding does not inspect browser runtime traffic, GitHub host logs, cookies, device telemetry, extensions, or security controls.
