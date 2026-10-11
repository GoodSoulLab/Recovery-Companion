# Recovery Companion — Reviewer and Formative Test Protocol v0.2

**Date:** 2026-10-11  
**Status:** Draft for independent review; not approved for participant use  
**Prototype under review:** [Context selector v0.4](../../prototype/context-selector-v0.4.html)  
**Decision:** Whether a transparent context selector improves access to an acceptable next step over a static toolkit containing the same reviewed options. This is a usability falsification study, not a clinical efficacy study.

## 1. Current gate

| Gate | Status | Required evidence before participant exposure |
|---|---|---|
| Exact exercise content and cautions | Open | Qualified clinical review plus paid lived-experience review of the exact rendered v0.4 cards and safety copy |
| Safety and referral boundaries | Open | Review of skip/stop language, adverse-reaction response, and any location-specific support sheet; prototype must not be presented as care or crisis response |
| Study ethics | Open | Determine whether IRB or other ethics oversight applies; document the applicable determination, consent, compensation, and incident process |
| Privacy and security | Partially specified; not independently verified | Inspect the exact delivered artifact and delivery path; test runtime network and storage behavior; approve research-data workflow and retention/deletion controls |
| Intellectual property | Open | Confirm provenance and rights for every exercise and linked resource; exclude copied proprietary worksheets or branded sequences |
| Accessibility | Open | Rendered browser, keyboard, zoom/reflow, and screen-reader review of the exact test build |
| Competitor comparison | Open | Direct walkthrough only where access is lawful and does not require invented histories, unnecessary sensitive disclosure, or unconsented community contact |

**Hard stop:** Do not recruit or expose prospective participants to exercise content until the clinical, lived-experience, ethics, privacy/security, IP, and accessibility gates have been resolved for the exact study build. An ethics determination may conclude that formal review is not required; document that determination rather than assuming it.

## 2. Review roles and sequence

1. **Clinical reviewer:** A currently licensed, practicing clinician with relevant experience supporting adults who voluntarily seek behavior change. Verify license and standing, scope, current practice, relevant population experience, conflicts, and paid scope. The reviewer checks foreseeable harms and boundaries; they do not certify efficacy.
2. **Lived-experience partners:** Two to four paid adults with varied self-chosen recovery goals. They review language, burden, agency, usability, and perceived safety. They are not asked to disclose detailed histories or certify clinical safety. Participation and compensation must not depend on favorable feedback.
3. **Privacy/security reviewer:** Reviews source and the exact delivery setup, host/device exposures, and proposed research-data workflow. Source inspection alone is insufficient.
4. **Accessibility reviewer:** Tests the rendered build with keyboard, zoom/reflow, and a screen reader; records blockers and severity.
5. **IP review:** Confirm original authorship or permission for each exercise, quotation, logo, and resource. Obtain specialist review if rights remain uncertain.
6. **Study owner:** Maintains a versioned issue log, records disagreement, implements changes, and freezes the study artifact only after blockers are resolved.

Do not treat an academic publication record as proof of licensure or current clinical practice. Do not appoint a reviewer from the public shortlist without checking fit, conflicts, availability, fees, and scope. Keep private reviewer identities, contact information, and compensation records outside this public repository.

For each card, record ID/version; reviewer role; approve, revise, reject, or escalate; rationale; required change; date; and unresolved disagreement. A material safety disagreement blocks that card. Lived-experience feedback can require a revision even when a clinician sees no clinical contraindication.

## 3. Decision question and hypotheses

**Question:** With identical reviewed content, does the selector help adults find an acceptable next step faster than a clear static index, while preserving fit, agency, and accurate privacy understanding?

**Falsifying outcomes:** The static index is as fast or faster; selector fit is materially worse; people prefer direct browsing; context prompts feel intrusive or burdensome; users infer diagnosis, surveillance, or authority the system does not have; or the selector creates a repeated pattern of reduced agency, shame/distress, or privacy misunderstanding.

The mechanism under test is routing. Do not infer that cross-modality integration is novel, that a person applied a tool outside the session, that behavior changed, or that clinical outcomes improved.

## 4. Smallest formative comparison

### Participants and task load

- Start with **8 completed participants** as a kill-screen, not a powered or representative study.
- Extend to **no more than 12** only when the eight-person pattern is promising but ambiguous under the precommitted rule below.
- Adults 18+ who voluntarily identify an interest in behavior change; no diagnosis, screening score, abstinence, or recovery label required.
- Use a counterbalanced within-person comparison: each participant completes two short, fictional tasks in each condition. Match task difficulty across conditions and rotate scenario/condition order to reduce practice effects.
- Conditions: (A) a well-organized static index and (B) the transparent selector. Both contain the same approved cards, wording, support route, and exit choices.

Use only non-graphic, fictional scenarios about a difficult moment, overwhelm, or reflecting after a choice. Ask participants to respond to the fictional person, not to disclose whether the scenario resembles their life. Do not ask about sexual acts, pornography, trauma, partners, consent violations, diagnosis, or personal relapse histories.

### Outcomes

Record only what is needed to compare the interfaces:

- Time from task presentation to an acceptable next step or explicit decision that none fits.
- Selected card or “none”; treat “none” as a valid agency-preserving response and report its frequency separately, not as a failure or artificially fast successful selection.
- Independent fit rating on a 1–5 anchored scale using the scenario and card text, with raters blind to interface condition where feasible.
- Whether the participant can explain why an option appeared and how to reject, change, or exit.
- Brief ratings of perceived agency, burden, and privacy understanding.
- Optional distress check with skip/stop option; accessibility blockers, confusion, adverse reactions, and protocol deviations.

These measures are usability signals only. Do not use symptom scales or collect free-text personal stories, diagnoses, detailed histories, audio/video, precise age, location, contacts, or longitudinal behavior data.

### Directional decision rule

Before the first session, timestamp and freeze the scenario set, content version, rating anchors, analysis sheet, and decision rule.

**Keep testing the selector only if** the first eight participants show all of the following:

1. At least **20% lower median time** to an acceptable next step in the selector condition across matched tasks.
2. Selector fit is no more than **0.5 points worse on a 5-point scale** than static browsing.
3. No repeated pattern of increased burden, reduced agency, or privacy misunderstanding; explicit “none fits” responses are reported and reviewed for condition imbalance.
4. No serious adverse event and no unresolved reviewer concern about any card shown.

If the pattern is absent or mixed after eight, retain the static index or stop. Extend to 12 only when the directional signal is promising but uncertain, not to search for a favorable result. Pause or stop immediately for serious distress, coercion, a material safety concern, or repeated belief that the prototype is monitoring/providing care. These thresholds are project decision aids, not validated clinical cutoffs. Report counts and distributions; do not use significance testing to imply efficacy.

## 5. Session safeguards

### Recruitment and consent

Describe the activity as research on two ways to browse draft self-help options, not therapy or treatment. State that the content may feel personal; participation is voluntary; participants may skip, stop, or leave without explanation; and the prototype is not monitored. Explain foreseeable discomfort, compensation, data access/retention, withdrawal limits after de-identification, researcher contact, and any applicable ethics determination in reviewed consent materials.

Do not recruit from support groups or contact group members without organizational permission and appropriate ethics review. Do not recruit based on another person’s concern or moral judgment. Do not represent the study as a way to receive help.

### Moderator opening (draft; requires review)

“We are comparing two ways to find a possible next step for a fictional situation. This is not treatment, diagnosis, or crisis support. The draft options have not been shown to improve outcomes. You do not need to share anything about your own life. You can skip a question, choose ‘none,’ take a break, or stop at any time. The page code is designed not to send or save your choices, but the device, browser, and hosting environment may leave traces. The study records only the limited coded measures described in the consent materials. What questions do you have before deciding?”

Do not promise anonymity or confidentiality beyond the approved protocol. The script does not replace a consent form or data notice.

### Neutral prompts

- “What do you think this screen is asking you to do?”
- “What makes this option seem like a fit or not a fit for the fictional situation?”
- “What do you think the prototype can see or remember?”
- “How would you reject, change, or leave this option?”
- “Would you prefer another way of viewing the choices?”

Do not ask why someone personally engages in a behavior. If personal details arise, do not probe; remind the participant that fictional responses are sufficient.

### Distress and stopping

A named study lead must be responsible for participant comfort, with an approved escalation plan and independently reviewed location-appropriate resources available before sessions. Pause immediately if a participant appears distressed, expresses pressure or shame, or asks to stop. Offer to close the prototype, take a break, or end the session. Do not counsel or press for an explanation. Follow the approved local safety protocol if immediate danger is disclosed. Document only minimal non-graphic incident details. Suspend sessions after a serious event pending independent review.

## 6. Data, privacy, and security

The prototype uses in-page state and is intended not to persist selector choices. That is not equivalent to anonymity or confidentiality. A hosted page request can expose connection metadata to its host; browser history, shared devices, extensions, screenshots, managed-device software, and visible screen content remain possible exposures.

Before the test:

- Inspect the exact release artifact; verify runtime requests and browser storage during load and interaction in a clean environment.
- Review the host’s logging, retention, cookies, and account context or use controlled local delivery consistent with the approved protocol.
- Keep consent, contact, and compensation records separate from coded usability data; restrict access and define retention, deletion, and incident response.
- Train the moderator not to record sensitive disclosures; audit notes for unnecessary details.
- Give participants accurate notice of page, browser/device, host, and study-data boundaries.

Collect only participant code, eligibility/consent status, condition order, fictional task ID, choice/none, time, fit/agency/burden/privacy ratings, and minimal interface observations. Avoid names and direct identifiers in task notes. Do not put study data, reviewer details, private correspondence, or participant information in this public MIT-licensed repository.

## 7. Intellectual property and content provenance

Maintain a card-level provenance record: author, source tradition, exact source/edition if applicable, original or licensed status, permission evidence, and changes made. “Inspired by” does not automatically clear copyright or trademark risk. Exclude copied worksheets, branded sequences, and third-party text unless rights are confirmed. Record unresolved items as blocked; do not ask participants to review blocked content.

## 8. Competitor benchmark (separate from the primary experiment)

The competitor task is a separate research activity, not a substitute for the static-versus-selector comparison. Proceed only when lawful access is available without fabricated personal history, unnecessary sensitive account data, or unconsented peer contact. Use the same fictional job story where the product permits it; record app/site version, date, actions, time to an actionable option, context requested, ability to skip/reject, support route, paywall, visible privacy controls, and accessibility blockers.

Label every note as **Observed**, **Publisher claim**, **Unknown**, or **Interpretation**. Inaccessible text views and untested app flows are unknown, not absent. Do not join or post in recovery communities without organizational permission, appropriate ethics review, and researcher disclosure.

## 9. Results and decision record

For each condition report participant count, task completion and “none” counts, median and range of time, fit distributions, agency/burden/privacy patterns, accessibility issues, distress/adverse events, protocol deviations, and missing data. Preserve null and negative results. Separate:

- what was directly observed;
- what participants reported;
- what independent reviewers rated;
- what remains unknown;
- whether the result changes the product decision; and
- plausible alternative explanations.

A positive usability result permits only a decision about whether to conduct a separately reviewed feasibility study of applying an approved micro-step. It does not establish clinical benefit, demand, retention, willingness to pay, competitive advantage, or venture viability. “No venture” and a static public resource remain valid outcomes.

## 10. Current next actions

1. Commission and complete the independent reviews for exact v0.4 content and procedures; no outreach has occurred.
2. Resolve clinical, lived-experience, privacy/security, IP, accessibility, and ethics gates; revise and version the artifact.
3. Conduct the synthetic mechanics and source/runtime checks on the frozen test build.
4. Freeze consent, scenarios, moderator materials, data plan, analysis sheet, and decision rule.
5. Recruit only after the applicable ethics determination and all preceding gates are documented.
