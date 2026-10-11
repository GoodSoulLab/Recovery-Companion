# Public Experience Teardown and Minimum Intervention Architecture v0.2

**Prepared:** 2026-10-11  
**Status:** Public-site walkthrough plus desk research. No authenticated app test, participant test, clinical approval, or security audit.  
**Purpose:** Update the competitor challenge and define what can safely advance before reviewer availability.

## Decision

Continue nonparticipant discovery and implementation work. Do not expose draft recovery exercises to participants yet.

The walkthrough weakens a broad “bring the tools together” thesis. Relay publicly presents a personalized plan, urge/trigger logging, therapist-designed lessons, accountability, and group support. SMART Recovery already pairs a categorized toolbox with detailed tool pages, printable worksheets, and free meetings. The remaining product hypothesis is narrower: **does an optional, explainable selector help someone find an acceptable next action faster or with better fit than a strong static index, without adding friction or reducing agency?**

No competitor app was installed or used after sign-in. Site copy and accessible onboarding are not evidence of clinical efficacy, actual data flows, or the experience after account creation.

## Method and evidence labels

- **Observed on public website:** Pages or screens directly opened on 2026-10-11 without signing in or submitting user data.
- **Publisher claim:** Text the vendor or organization makes about its product, service, privacy, or outcomes.
- **Inference / question:** A design implication to test, not a finding about users.
- **Not observed:** Authenticated app flow, account behavior, actual privacy/security controls, moderation, and clinical outcomes.

I did not provide an email, location, behavior history, or demographic information; join a meeting; choose a recovery path; install an app; or submit a form.

## Experience teardown

| Alternative | Public experience observed | Challenge to Recovery Companion | Important unknowns |
|---|---|---|---|
| **Relay** ([public site](https://www.joinrelay.app/)) | The home page leads with “quit pornography for life” and advertises a like-minded group, therapist-designed lessons, daily accountability, urge/trigger logging, and progress tracking. The page showed $149/year and a 7-day trial on the date checked. Its FAQ says members can use a first name or pseudonym and that shared material is not tied to public identity; this is a publisher claim, not a security verification. Clicking a public “Join today” link opened the first onboarding screen: “Select a path to begin,” with **Men’s path** and **Women’s path** choices and a three-step progress rail (“Select a path,” “Get to know your situation,” “Customize your recovery plan”). I stopped before choosing a path or continuing. | Strong evidence against novelty by integration. The public funnel already signals personalization, a plan, tools, and human connection. The entry screen makes gendered segmentation salient; whether users find it useful, limiting, or both is unknown. Its abstinence-forward public language may fit some goals and conflict with others; actual plan flexibility was not observed. | Whether the app supports user-defined reduction/moderation goals; how a situation changes recommendations; whether users can skip the path choice; actual screen count and sensitive-data requests; group matching/moderation; withdrawal/cancellation; storage, sharing, retention, deletion, and security; outcome evidence. |
| **SMART Recovery** ([toolbox](https://smartrecovery.org/toolbox), [meetings](https://smartrecovery.org/meeting)) | The public toolbox lists 14 participant tools. Each has a short description, a printable worksheet, and a “Read more” page. I opened the Cost-Benefit Analysis (CBA) page: it labels the tool “helpful with” motivation, gives a step-by-step exercise, examples, reflection questions, a worksheet download, and related links. The page was readable without signing in. The public meeting finder asks for a location; I did not enter one or join a meeting. SMART’s meeting information says meetings are free, facilitator-guided, and typically about 90 minutes. | A static index is already a meaningful, no-account route through practical tools; detailed pages supply more guidance than a simple card list. Its “helpful with” labels are a basic context taxonomy. Free peer connection is another strong substitute. A selector must beat this quality of static organization, not a deliberately weak list. | Fit for this product’s particular population and goals; actual usefulness at a moment of need; search/filter effectiveness; accessible time and location; group experience and privacy; outcomes. Public materials are SMART’s intellectual property and should not be copied. |
| **Brainbuddy** ([official site](https://www.brainbuddyapp.com/), [privacy policy](https://www.brainbuddyapp.com/privacy-policy)) | The public privacy policy describes collection of account data, check-ins/streaks, user-created content, feature-use data, wellness metrics, diagnostics, IP-derived region, and advertising identifiers where permission is granted. This is a document review, not an app walkthrough or data-flow verification. | Tracking, tailored plans, and privacy statements already exist. Recovery Companion would need a measurable data-minimization advantage and clear user control. | Actual defaults, what is required or optional, deletion/export, sharing/retention in practice, security, and current app flow. |
| **Fortify** ([official site](https://www.joinfortify.com/), [Google Play listing](https://play.google.com/store/apps/details?id=com.ftnd.fortify)) | Public materials advertise recovery content and, in current store/vendor materials, AI coaching. I did not install or open the authenticated product. App-store privacy summaries are developer disclosures, not an independent audit. | The space is actively evolving; “digital recovery companion” and “AI coach” are not differentiators. | Current feature behavior, coaching boundaries, what content is generated or reviewed, data needs and handling, user control, and outcome evidence. |

### What is established—and what is not

**Established by this limited walkthrough:** the publicly accessible SMART toolbox is a fairly rich static alternative, and Relay’s public proposition overlaps the broad product bundle. These facts narrow the product question to incremental selection value.

**Not established:** that Relay lacks flexible goals, that SMART cannot serve this population, that either product is unsafe, or that users want another selector. No conclusions about clinical quality, privacy/security, or outcomes can be drawn from this public-site pass.

## Minimum intervention architecture (reviewer-independent design boundary)

The smallest credible design is a **guided index**, not a diagnostic or adaptive engine.

1. **User starts:** neutral prompt such as “Find a next step.” No account, diagnosis, explicit sexual-history questions, inferred trigger, passive sensing, or free-text field.
2. **User may choose a broad situation:** urge, feeling overwhelmed, reflecting after a choice, seeking a person/resource, or browse all. Make skip, back, and exit equally visible.
3. **Optional narrowing:** time available and preferred kind of next step (practical, reflective, or human connection). Recovery tradition preference is optional and must not be a proxy for suitability.
4. **Rule-based retrieval:** apply reviewer-defined exclusions/cautions first; use only the options the person chose to provide. Match a small set of candidate cards and explain the match in plain language. No diagnosis, probability, “best” ranking, inferred risk, AI, or personalization based on history.
5. **Choice stays with the user:** open a card, change filters, browse the complete index, choose human/professional support, or leave. Never make contact automatically.
6. **No persisted session:** no backend, analytics, notifications, event history, or user-entered story. Clear temporary choices on exit/reload. Any later study data is a separate governed research system.

### Content and rule registry

Each card should have a stable ID, exact text, intended broad situation, duration, source/provenance and rights status, caution/exclusion rules, alternatives and stop option, version, and review state. Distinguish states such as **draft**, **rights checked**, **clinical review complete**, and **lived-experience review complete**. A card is not released to participants merely because its interface works.

Safety rules are exclusions and guardrails, not a clinical assessment. If nothing matches, show the full index and support/exit routes instead of inventing a match. Keep a human-support path visible even when the person has not selected it. No streaks, urgency prompts, shame language, accountability alerts, monitoring claims, or implied crisis response.

### Key architecture challenge

The v0.1 prototype is deterministic, but deterministic matching alone does not establish better help. The selector can become an extra questionnaire that filters out useful options. If an organized index with “helpful for” labels performs as well, use the index. A simpler, legible interface is the default until selection advantage is demonstrated.

## What can proceed without clinical/lived-experience review

**Proceed now:** public competitor/site teardown; rule and interaction design using synthetic examples; implementation and verification of local-only/no-network behavior; privacy threat modeling; accessibility review of prototype mechanics; checking licenses and avoiding copied curricula; drafting study materials and analysis code without recruiting.

**Wait:** showing draft exercises or recovery recommendations to participants; recruiting people around unwanted sexual behavior; collecting sensitive histories or behavior logs; describing the tool as safe, therapeutic, or effective. The project handoff and PRD set qualified review and privacy/ethics gates before participant exposure; this work does not waive them.

## Falsification plan

### Pre-review, no-participant screen

Run an internal, reproducible **synthetic coverage test** before spending on participant recruitment:

- Create 8–10 non-graphic, synthetic task cards that vary only broad user-selected situation, time, and preferred next-step type.
- For each, record what the static index presents and what the current selector presents; check whether the selector returns 0, 1, 2–3, or more than 3 choices, and whether its explanation accurately reflects only the entered choices.
- Add adversarial cases: no preference; browse all; conflicting filters; human support preference; context with no matching candidate; choose nothing.
- Fail the selector design if it hides the full index, returns no usable path without a clear fallback, produces a misleading explanation, or yields the same results as a simple category index with more inputs.

This can falsify poor retrieval mechanics and quantify coverage. It **cannot** show that recommendations are clinically appropriate or useful to people; no participant claim follows.

### Smallest meaningful user test (after review gates)

If the synthetic screen passes and exact content receives qualified review, run a formative within-person comparison with 8–12 adults who voluntarily identify a behavior-change goal. Use identical reviewed cards in a curated static index and the transparent selector; counterbalance condition order and use task-matched, non-graphic scenarios to reduce learning effects. Do not collect diagnoses, explicit histories, free-text journals, or longitudinal behavior data.

Measure time to an acceptable option, independent fit rating, ability to explain the selector and reject it, perceived agency, privacy comprehension, and shame/distress or other adverse reactions. Treat small-sample results as directional usability evidence, never clinical efficacy evidence.

**Falsify the selector thesis** if static browsing is as fast or faster with similar fit, people prefer the index, the selector’s questions feel intrusive or burdensome, or users cannot explain why an option appeared. Keep a static resource or stop; do not build a company around a mechanism that fails its comparison.

## Decision gates

1. **Now:** finish synthetic coverage, local privacy checks, and public competitor evidence. No reviewer or participant spend required.
2. **Before exposure:** obtain qualified clinical and lived-experience review of exact cards, scenario prompts, consent/debrief, stop rules, and resource language; complete privacy, IP, accessibility, and ethics determination.
3. **After the small test:** advance only if there is a clear directional fit or time advantage with preserved agency and no concerning harm signal. If not, prefer a static index, human-support navigation, or no product.
4. **Commercial thesis:** remain unproven. Do not infer demand, retention, willingness to pay, clinical impact, or venture viability from a site teardown or usability test.

## Source and scope notes

- Relay public site and first onboarding screen: https://www.joinrelay.app/ (screen reached through its public Join link; no path selected; no user information submitted; observed 2026-10-11).
- Relay privacy policy: https://www.joinrelay.app/privacy-policy (publisher statement; not audited).
- SMART toolbox and CBA: https://smartrecovery.org/toolbox and https://smartrecovery.org/cost-benefit-analysis (public pages opened and inspected 2026-10-11).
- SMART meetings and FAQ: https://smartrecovery.org/meeting (publisher information; no location supplied and no meeting joined).
- Brainbuddy privacy policy: https://www.brainbuddyapp.com/privacy-policy (publisher statement; not audited).
- Fortify current public materials: https://www.joinfortify.com/ and https://play.google.com/store/apps/details?id=com.ftnd.fortify (marketing/store disclosures; app not used).
- Existing baseline: [Project Handoff](../PROJECT_HANDOFF.md), [PRD v0.1](../product/PRD_v0.1.md), [Competitive Evidence Matrix v0.1](COMPETITIVE_EVIDENCE_MATRIX_v0.1.md), and [Decision Memo v0.1](DECISION_MEMO_v0.1.md).
- Reviewer sourcing and safeguards: [Reviewer Sourcing Brief v0.1](REVIEWER_SOURCING_BRIEF_v0.1.md) and [Review Protocol v0.1](REVIEW_PROTOCOL_v0.1.md).
