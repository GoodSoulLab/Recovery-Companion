# Recovery Companion — Decision Memo v0.1

**Date:** 2026-10-11  
**Phase:** Product discovery; no clinical approval, participant findings, or commercial validation  
**Decision addressed:** Is a transparent, context-sensitive selector worth testing against a good static toolkit?  
**Evidence status:** Public competitor review completed; authenticated hands-on teardown not completed.

## Recommendation

Proceed only to a small, content-matched prototype comparison after qualified clinical and lived-experience review of the candidate exercises and participant materials. Do not yet build an account-based product, collect sensitive recovery histories, or make a venture case.

The falsifiable product claim is narrower than “integration helps”:

> For adults who voluntarily want to change a behavior, a transparent selector using only a moment they choose to name and a preference they choose to state will help them select an acceptable next action faster or with better fit than the same reviewed options in a well-organized static toolkit, without reducing agency or increasing shame/distress.

If selection does not materially improve fit or speed, the product thesis should shift to a static toolkit, human connection, or no product. A competent competitor may already solve this job adequately; the current public review cannot rule that out.

## 1. Competitive experience teardown: what the evidence says

This is a **public-facing evidence teardown**, not an app walkthrough. Sources were inspected on 2026-10-11. Marketing and privacy-policy statements below are attributed to their publishers. They do not establish clinical effectiveness, complete feature behavior, security quality, or user experience.

| Alternative | Publicly stated experience | Challenge to our thesis | Unknown until hands-on / independent verification |
|---|---|---|---|
| [Relay](https://www.joinrelay.app/) | Public site describes personalized plans, therapist-designed lessons, daily accountability, trigger/urge logging, progress tracking, and a private peer group. The site lists $149/year and a 7-day trial. Its therapist page describes plans around triggers, values, and goals, plus group support available at any hour. | Strongest direct challenge: the core bundle already combines skills, context, tracking, and optional human connection. “Putting recovery tools together” is not a defensible novelty claim. | Actual onboarding and urge flow; time/clicks to an appropriate next step; user control over goals and recommendation logic; group moderation and boundaries; demographic/goal fit; trial/paywall behavior; actual privacy/security architecture; outcome evidence. Public privacy copy says pseudonyms may be used and activity is not tied to public identity, while its policy describes retention; neither is a security audit. |
| [Fortify — Find Freedom](https://apps.apple.com/us/app/fortify-find-freedom/id1304648824) | Apple’s listing includes developer-provided app-privacy categories that may be linked to identity, including health, user content, identifiers, and sensitive information. Apple explicitly says these disclosures are developer-provided and not verified by Apple. | There is an established recovery app with a substantial user-facing proposition. Privacy differentiation cannot be asserted from category labels alone. | Current app screens and flow; what data each feature actually requires; collection, sharing, retention, deletion, and account behavior; accessibility; fit for varied goals; independent security and outcomes. Do not infer absence of a selector from the listing. |
| [Brainbuddy](https://www.brainbuddyapp.com/) | Current privacy policy says the service collects account data, in-app check-ins/streaks/content, feature-use data, wellness metrics, device diagnostics, approximate IP-derived region, and advertising identifiers where permission is granted; it says it does not collect precise location, contacts, or browsing history outside the app. | Tracking, tailored recovery plans, and privacy claims already exist in this category. A privacy-first proposition must mean a demonstrable data-minimizing design, not a slogan. | Actual app flows and defaults; what is necessary versus optional; how metrics are computed and used; current app-store disclosures; user comprehension and deletion/export; security controls and retention in practice; independent clinical evidence. |
| [SMART Recovery meetings and tools](https://smartrecovery.org/meeting) | SMART publicly offers free meetings, a meeting finder, structured check-ins, practical tool work, and mutual support. Its site says people may attend online or in person; meetings are generally around 90 minutes. | Free, secular practical tools and voluntary human connection are available without creating a new peer network. The alternative set includes established organizations, not only apps. | Whether available meetings and tools meet the specific moment-of-need job; access friction and wait/time fit; local meeting availability; user experience and fit for different sexual-behavior goals. SMART’s dedicated sex/addiction page contains diagnostic and causal language that should not be adopted as product evidence or framing. |

### Teardown conclusion

**Verified from public sources:** the category already has products and organizations offering combinations of plans, exercises, check-ins, peer support, and privacy statements. SMART offers free peer meetings and tools. Relay’s public proposition overlaps substantially with the proposed bundle.

**Not verified:** that any competitor lacks explainable moment-level selection; that its recommendations are clinically inappropriate; that its data practices are unsafe; or that users cannot find/use a fitting tool quickly. Those claims require direct observation, policy/data-flow analysis, and user research.

**Current implication:** do not compete on aggregation or “AI recovery.” Test only the incremental decision-support value of a low-data selector, and benchmark the complete job against both the static comparator and at least one accessible competitor workflow.

## 2. Minimum intervention architecture

### Product boundary

An adult user initiates a session and self-selects a broad situation. The prototype presents a few original, reviewed candidate actions. It does not assess whether the user has a disorder, infer a trigger, predict behavior, or treat a condition. A user can reject every suggestion, switch to the full library, exit, or choose a human-support route.

### Minimum flow

1. **Neutral entry:** “What would help right now?” No identity, diagnosis, sexual-history, or explicit behavior questions.
2. **User-selected situation:** “I’m facing an urge,” “I feel overwhelmed,” “I’m reflecting after a choice,” or “Browse all tools.” Use neutral labels and allow skip.
3. **Optional preference:** “A few minutes / more time,” and “practical step / reflection / contact with a person.” No free-text field in the first prototype.
4. **Transparent selection:** show up to three cards from the reviewed library. Each includes “Why this is shown” tied only to the user’s selections, estimated time, source tradition, and a clear “not for everyone” caution when relevant.
5. **User action:** open one card, choose a different one, browse all, or exit. No countdowns, streaks, persuasion loops, or auto-messaging.
6. **Optional feedback:** a single local, non-identifying question: “Was this useful enough to keep?” No journal text or event history retained in the prototype.

### Selection rules

- Apply reviewer-set exclusions and caution rules before ranking. A caution means omit the tool or show a plain-language caveat; never diagnose from a response.
- Match only the user-selected situation, time budget, preferred action type, and any explicitly selected recovery preference.
- Use deterministic rules, visible to reviewers and explainable to users. No machine learning or generative content.
- Return two or three different options where possible, including an action not framed as abstinence. Never present a single “correct” path.
- If nothing matches, show the full library and user-controlled human/professional support options. Do not improvise a recommendation.
- Do not use past behavior, app engagement, inferred emotions, location, contacts, or browsing activity.

### Minimum technical and data design

- Clickable local prototype; no account, backend, analytics SDK, notifications, or external messaging.
- Session state exists only in memory and clears on exit/reload. Research notes are stored separately under participant codes; do not collect sexual histories or record screen/audio by default.
- A privacy notice explains what is and is not collected in the usability study. Research consent and participation are separate from any clinical care.
- Emergency/professional support language is static, reviewed, jurisdiction-appropriate, and never represented as monitoring or crisis response.

## 3. Candidate exercise library for qualified review

These are **original draft candidates**, not treatment, approved scripts, or claims of efficacy. A licensed clinician with relevant expertise and people with lived experience must review wording, cautions, accessibility, and adverse-reaction risks before participant exposure. Do not copy branded worksheets or reproduce licensed curricula. The source traditions below describe inspiration only; they do not establish that an exercise is validated for this population.

| ID | Candidate / purpose | Possible user-selected situation | Guardrail for review |
|---|---|---|---|
| C01 | **Pause and orient** — take a brief pause; name a few neutral things noticed in the present environment; decide whether to continue or choose another option. | Urge; overwhelm | Keep eyes-open and stop options explicit. Do not prescribe breath focus or body scanning as universally calming. |
| C02 | **Name the experience lightly** — select a simple label such as “urge,” “stress,” or “uncertainty,” without explaining its cause. | Urge; overwhelm | No trauma probing or causal story. Offer “skip naming” and discontinue if labeling increases distress. |
| C03 | **Make room for a choice** — distinguish having an urge/thought from acting on it; identify one action available in the next few minutes. | Urge | Avoid implying that urges are harmless in every circumstance or that a brief pause guarantees control. |
| C04 | **Change one condition** — choose a small, reversible environmental adjustment the user considers helpful (e.g., move to a shared space, put device down, or change activity). | Urge; overwhelm | No surveillance, device blocking, coercion, or restriction as default. User decides whether any change is safe. |
| C05 | **Next-step intention** — finish a short prompt: “If [situation I chose] continues, I will try [my chosen action].” | Urge; overwhelm | User supplies choices from a menu; no compulsory abstinence goal. Avoid presenting implementation intentions as guaranteed prevention. |
| C06 | **Values-to-action micro-step** — choose one value from a neutral menu or skip, then select a small action that expresses it today. | Urge; setback; browse | Do not impose moral, religious, relationship, or abstinence values. Distinguish the person’s chosen values from others’ expectations. |
| C07 | **Nonpunitive review** — “What happened just before? What did I need? What is one adjustment I choose?” No graphic detail and no blame score. | After a choice the user wants to change | Stop if reflection becomes self-attack or rumination. Never imply one event proves a disorder or a failed recovery. |
| C08 | **Boundary reminder** — user privately reviews a boundary they wrote or selected in advance and may revise or set it aside. | Urge; setback | No imported Three Circles/branded text without rights review. Boundary is user-authored, flexible, and not a moral test. |
| C09 | **Contact menu** — choose whether to view links/phone shortcuts for an existing trusted person, independent peer meeting, clinician directory, or none. | Any, optional | Never send messages automatically, expose contacts, or imply peer support is clinical care. Verify resource links before use. |
| C10 | **Meaningful-life action** — choose a brief ordinary activity unrelated to monitoring or suppressing sexual thoughts. | Overwhelm; setback; browse | Do not frame activity as distraction that must eliminate an urge. Respect disability, environment, and user choice. |
| C11 | **Preference reset** — “Would you like a different kind of option?” then switch among practical, reflective, or human-support choices. | Any | A product correction path, not a therapeutic exercise. Never penalize declining. |
| C12 | **Stop / get support** — leave the flow and use reviewed, static routes to professional or emergency support when the user chooses or the research scenario indicates immediate danger. | Any | Qualified reviewers must set exact wording and applicable local resources. The prototype is not monitored and must say so. |

**Library release gate:** each card needs provenance and rights status, intended use, exclusions/cautions, duration, exact user-facing wording, alternative/stop option, reviewer names/credentials, review date, and version. No card is “clinically reviewed” until that record is completed.

## 4. Smallest falsification experiment

### Experiment

After clinical and lived-experience review, conduct a moderated, within-person prototype study with **8–12 adults (18+) who voluntarily identify a current behavior-change goal**. This is a formative usability test, not a clinical trial. Do not ask for diagnosis, explicit sexual history, or graphic scenario details. Use standardized, non-graphic scenarios and allow participants to skip or stop.

Each participant completes two counterbalanced tasks:

- **A — Static toolkit:** the same reviewed cards in a well-organized situation-labeled index.
- **B — Context selector:** the same cards surfaced by visible rules using only self-selected situation/time/action preference.

Then complete one matched task using the most comparable accessible competitor flow after lawful access is confirmed. If account/app access cannot be obtained without unnecessary sensitive disclosure, record the competitor comparison as unavailable rather than simulate it.

### Primary observations

- Time to select an acceptable next step.
- Fit of selected card for the scenario, rated independently by two reviewers blinded to interface condition, using a prewritten rubric.
- Whether the participant can explain why the option appeared and can decline/change it.
- Perceived usefulness, agency, shame/distress, privacy comprehension, and adverse reactions using brief scales plus optional debrief.
- Completion failures, misunderstandings, and accessibility barriers.

### Precommitted decision gates

**Proceed to a larger comparative usability test only if:**

1. The selector improves median fit by at least **one point on a 7-point scale** *or* reduces median time to an acceptable choice by at least **20%** versus static, with no meaningful worsening in the other primary measure.
2. At least 10 of 12 participants (or 7 of 8 if n=8) correctly explain why a suggestion appeared and know they can reject it.
3. No serious adverse event occurs; no repeated pattern of increased shame/distress, coercive interpretation, or false belief that the app is monitoring/providing therapy occurs.
4. Reviewers find no unresolved selection rule that presents an unsuitable exercise for a tested scenario.

**Pivot to static toolkit or a support directory** if speed/fit do not cross the threshold, participants prefer browsing, or human connection is consistently the wanted next step.

**Stop** if safety review identifies unresolved risk, a serious adverse reaction occurs, participants mistake the prototype for clinical care or live monitoring, or privacy expectations cannot be met.

These are product-screening thresholds, not statistical proof or clinical outcomes. With n=8–12, findings are directional; the main falsifier is a consistent lack of user-perceived fit/time advantage plus no strong usability explanation for why a selector should help.

### Why this is the smallest useful test

A questionnaire about stated preference would not reveal whether contextual selection beats an organized index. A content-matched prototype comparison isolates the proposed mechanism while holding the exercise set constant. The competitor task checks whether the job is already solved, but must not delay the static-versus-selector falsification if access is unavailable. No real-time deployment, longitudinal monitoring, sensitive-data collection, or clinical-outcome claim is needed to make this decision.

## 5. Pre-study gates and immediate work order

1. **Clinical/lived-experience review:** approve or reject exact card wording, inclusion/exclusion rules, debrief, and stop language. Do not recruit before this review.
2. **Direct competitor walkthrough:** test Relay, Fortify, and Brainbuddy with a research account only if lawful, accessible, and not requiring unnecessary disclosure; document screen-by-screen steps, time, friction, paywall, controls, and user-visible explanations. Do not create fake personal histories or contact peer groups as a researcher without consent.
3. **Privacy/security threat review:** inspect local storage, URLs, logs, analytics, crash reporting, clipboard/screenshot risk, shared-device context, backups, and researcher data handling. Verify that the implementation matches the “no backend/no analytics” claim.
4. **IP review:** verify original wording and avoid reproducing SMART, SAA, Facing the Shadow, or other branded/copyrighted materials.
5. **Prototype and preregistration:** freeze scenario text, conditions, counterbalancing, measures, rubric, thresholds, exclusions, and adverse-event response before first session.

## 6. Venture-level challenge

The current differentiation is not established. Relay appears to cover much of the functional bundle already, and free peer tools exist. “Privacy-first” may be a meaningful design constraint but is not, by itself, proof of demand or durable advantage. A rule-based selector may add cognitive overhead, communicate false authority, or create a new safety burden without improving selection.

The viable alternatives are:

1. **No standalone venture:** users are adequately served by existing apps, directories, clinicians, and peer groups.
2. **Small static resource:** if reviewed tools are useful but selector value is absent, publish a privacy-light, user-controlled toolkit or navigation resource.
3. **Context selector:** only if the test shows a clear choice-quality or time advantage without safety/privacy regression, then test persistence and real-world usefulness later.

There is no basis yet to choose option 3 as a company. The next decision should be whether the selector mechanism earns a larger test—not whether the integrated concept sounds compelling.

## Sources inspected

- Relay home page, product and pricing claims: https://www.joinrelay.app/ (vendor marketing; accessed 2026-10-11).
- Relay for therapists: https://www.joinrelay.app/for-therapists (vendor marketing; accessed 2026-10-11).
- Relay privacy policy: https://www.joinrelay.app/privacy-policy (publisher policy; updated 2025-10-26; accessed 2026-10-11).
- Fortify App Store listing: https://apps.apple.com/us/app/fortify-find-freedom/id1304648824 (developer disclosure surfaced by Apple; Apple says disclosures are unverified; accessed 2026-10-11).
- Brainbuddy privacy policy: https://www.brainbuddyapp.com/privacy-policy (publisher policy; accessed 2026-10-11).
- SMART meeting experience: https://smartrecovery.org/meeting (organization description; accessed 2026-10-11).
- SMART page on sex-related recovery: https://smartrecovery.org/sex-addiction (organization page; not adopted as clinical authority; accessed 2026-10-11).

## Status ledger

- **Verified:** provided Project Handoff, PRD v0.1, Competitive Evidence Matrix v0.1, and project instructions read; current official/public competitor pages inspected.
- **Not done:** authenticated app tests, interviews, participant sessions, clinical review, lived-experience review, security audit, IP review, or commercial validation.
- **Next decision:** whether the reviewed candidate library and prototype are safe and sufficiently distinct to expose in a formative comparison.
