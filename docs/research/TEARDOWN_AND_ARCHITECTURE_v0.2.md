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

### Specific v0.1 implementation findings

Code inspection of `prototype/context-selector-v0.1.html` shows that the form opens with **urge**, **a few minutes**, and **practical step** already selected. The result function hard-filters against each selected field, then takes the first three eligible cards in library order with `slice(0,3)`; it does not rank options by evidence or suitability. The human-support cards are tagged as “person” and “human,” so the default “practical” selection filters them out. This is observable from the code, not user research.

These defaults weaken the claim that the choices are user-selected and can hide support by default. Before any test, change the context and preference fields so users actively choose them or skip them, always leave a visible browse/support/exit route, and avoid presenting the first three library records as “best” matches. Keep the prototype expert-only until reviewed.

## Visual design exploration v0.3

The v0.3 page applies a restrained editorial design system: warm neutral surfaces, forest-green action color, a single clay accent, serif display typography paired with familiar system controls, consistent spacing, quiet borders, and no decorative imagery. These are high-level cues toward clarity, restraint, precise craft, and honest materials; the page does not imitate any named designer or studio.

The comparison remains unchanged: Guided choice and Browse toolkit use the same 12 draft cards. The prototype retains neutral defaults, full Browse all behavior, visible human-support routes in both views, a single explanation for why the set appears, local in-page state only, keyboard-operable tabs, and explicit review-only language. The design pass does not improve evidence quality or validate the content. It remains untested in a rendered browser and is not ready for participant exposure.

## Interaction refinement v0.4

The v0.3 registry was exhaustively evaluated over 192 combinations of the four ordinary inputs (situation, time, kind, and approach; Browse all was treated separately because it intentionally ignores other filters). One selected constraint produced a match in every case. With two constraints, 4/45 combinations were empty; with three, 28/81 were empty; and with all four, 36/54 were empty. The logic also classified three-minute cards as both “a few minutes” and “more time.” These are synthetic code-coverage counts, not user behavior or evidence about clinical fit.

The v0.4 design makes situation the primary choice and places time, kind, and approach behind a closed optional-refinements disclosure. “A few minutes” is defined as up to 3 minutes and “a longer option” as 4–5 minutes. The human-support route remains visible in both comparison views, and its explanation says that the user requested support options rather than implying they selected hidden filters.

Retesting the revised code shows 12/12 cards with no filters and Browse all, two human-support cards from each view, 9 short and 3 longer cards with no duration overlap, and a clear no-match fallback. Empty results remain possible when a person stacks incompatible optional refinements; the interface offers clear filters, Browse all, and exit. This does not establish that the filter model is intuitive or clinically appropriate. The browser-render, screen-reader, reviewer, and participant gates remain open.

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

### Synthetic coverage run on v0.1

I ran the existing prototype’s rule logic against the actual 12-card registry, reproducing its eligibility filters and first-three cap. This was a code-path check with synthetic inputs only; it did not execute participant content in a study or judge clinical fit.

| Synthetic input | Current output | Finding |
|---|---|---|
| Default form: urge / a few minutes / practical / no approach preference | C01, C04, C05 | The form’s preselected values shape the result before the user has actively chosen them. |
| Browse all / no other filters | C01, C02, C03 | Returns 3 of 12 cards; “Browse all” in the selector does not actually show the library. |
| Urge / no other filters | C01, C02, C03 | Returns 3 of 10 eligible cards in registry order; several eligible alternatives are hidden without an explanation that the list was capped. |
| Setback / default time and style | C08, C11 | A result appears, but the output is determined by the practical default. |
| Setback / reflective / a few minutes | No matches | C06 and C07 exceed the time threshold; the UI asks the user to loosen filters rather than surfacing a clearer route. |
| Urge / person / human connection | C09, C12 | Human support appears only when the user selects both matching filters. |
| Urge / person / values/acceptance approach | No matches | The interface allows incompatible filters and then produces an empty set. |

**Result:** the current selector implementation fails its own “browse all” expectation and can hide options based on default filters and content order. Correct these mechanics before considering a participant comparison: make defaults neutral/optional, ensure browse-all truly exposes all cards, keep support/exit visible, explain when a filter narrows choices, and do not imply the first three items are the best fit. The static toolkit remains the safer and clearer prototype condition until this is fixed.

### v0.2 correction and offline verification

The v0.2 prototype changes the selectors to neutral “any” defaults, shows every matching card without ranking or a three-card cap, makes Browse all show the full library, and adds a visible human-support/exit route. Clear filters resets all choices. No selection is persisted.

I checked the actual prototype JavaScript with synthetic state in an in-memory DOM stub and ran static source checks:

| Check | Result |
|---|---|
| Neutral defaults, no filters | 12 of 12 cards shown |
| Browse all | 12 of 12 cards shown |
| Human-support route | C09 and C12 shown |
| Contradictory narrow filters | Clear empty state with clear filters, Browse all, or exit routes |
| Script syntax | Pass |
| External dependencies / network calls / persistent browser storage | None found |

This verifies the selector mechanics and source-level data boundary only. It is not a browser-render/accessibility audit, security audit, content review, or evidence of participant benefit. The exact recovery exercises remain drafts and the page remains expert-review only.

### Source-level accessibility review

A focused source review found that the view controls declared ARIA tab roles without arrow-key navigation. v0.2 now uses roving tab focus and responds to Left/Right and Up/Down arrows plus Home/End; activation by click remains available. Sampled foreground/background pairs for body text, muted labels, tags, primary buttons, the alert, and the status badge exceed WCAG AA text contrast thresholds in a source-level calculation. This does not verify browser rendering, zoom/reflow, keyboard operation in an actual browser, or screen-reader announcements. Complete those checks before any participant exposure.

### Smallest meaningful user test (after review gates)

If the synthetic screen passes and exact content receives qualified review, run a formative within-person comparison with 8–12 adults who voluntarily identify a behavior-change goal. Use identical reviewed cards in a curated static index and the transparent selector; counterbalance condition order and use task-matched, non-graphic scenarios to reduce learning effects. Do not collect diagnoses, explicit histories, free-text journals, or longitudinal behavior data.

Measure time to an acceptable option, independent fit rating, ability to explain the selector and reject it, perceived agency, privacy comprehension, and shame/distress or other adverse reactions. Treat small-sample results as directional usability evidence, never clinical efficacy evidence.

#### Precommitted decision rule and scope

This comparison tests only whether the selector improves access to an acceptable next step. It does not test whether a person applies the step outside the session, improves behavior-change outcomes, or benefits clinically. A pass would justify only a later, separately reviewed feasibility test of trying a reviewed micro-step; it would not validate the product thesis or justify forming a company.

Use a small, counterbalanced within-person comparison: each participant completes two non-graphic scenario tasks in each condition, using matched scenario sets and varied condition/order assignment to reduce practice effects. Include the same reviewed cards in both conditions. The primary outcome is paired time to an acceptable choice; participants may instead choose “none of these,” which counts as a valid agency-preserving response. Also collect a brief fit rating, whether they can explain the match or why nothing fits, and short agency, burden, and privacy-comprehension ratings. Do not collect behavior histories, diagnoses, free-text accounts, audio/video, or longitudinal data.

Treat 8 completed participants as a kill-screen, not a powered efficacy study. Before starting, define a directional pass as at least 20% lower median time in the selector, with fit no more than 0.5 points worse on a 5-point scale and no repeated pattern of greater burden, reduced agency, or privacy misunderstanding. If that signal is absent or mixed after eight, retain the static index or stop; extend to at most 12 only to resolve a promising but ambiguous pattern. Pause or stop for concerning distress or a privacy/safety misunderstanding. These thresholds are decision aids for this formative screen, not validated clinical cutoffs.

**Falsify the selector thesis** if static browsing is as fast or faster with similar fit, people prefer the index, the selector’s questions feel intrusive or burdensome, or users cannot explain why an option appeared. Keep a static resource or stop; do not build a company around a mechanism that fails its comparison.

## Decision gates

1. **Now:** v0.2 corrects the selector defects found in the synthetic run and passes the recorded offline logic/source checks. Next, review accessibility and privacy/security mechanics; these can proceed without participant spend. Do not treat the prototype as participant-ready.
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
