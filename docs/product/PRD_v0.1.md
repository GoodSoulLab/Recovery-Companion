# Recovery Companion — Product Requirements Document v0.1
Date: 2026-10-11
Status: Discovery hypothesis; not a clinical product specification or validated treatment.

## Problem
Adults voluntarily seeking change in unwanted sexual behaviors may need to select and apply practical skills across multiple recovery approaches in moments of difficulty. Existing products already combine lessons, tracking, community, and support. The unproven opportunity is safer, more appropriate, user-directed selection across approaches with minimal data collection.

## Intended user
Adults (18+) who self-identify a need for behavior change. Do not equate pornography use, high libido, moral disagreement, or a screening result with CSBD. No diagnosis required. Support varied recovery preferences and goals.

## Jobs to be done
1. In a difficult moment, identify a suitable next action quickly.
2. Choose among reviewed skills, voluntary connection, or professional support.
3. Preserve self-chosen values, boundaries, and recovery traditions.
4. Learn from optional feedback without generating a sensitive behavioral dossier.

## Non-goals (v0)
No diagnosis; no automated trauma processing; no passive monitoring or prediction; no automatic sponsor/partner alerts; no unrestricted generative therapy; no compulsory abstinence or 12-step identity; no explicit sexual-history intake; no clinical effectiveness claims.

## User journeys
1. Urge: user-initiated entry -> optional context -> two or three reviewed options -> user chooses -> short exercise or voluntary connection -> optional usefulness feedback.
2. Overwhelm: grounding/distress-tolerance options -> no trauma probing -> stop or seek human support.
3. Setback: nonpunitive reflection -> revisit self-chosen plan -> optional support.
4. Isolation: trusted-connection options without automatic messaging.
5. Values/meaning: choose one practical action outside the app.

## Functional requirements
P0: Accessible mobile-first interface; quick exit; neutral notification defaults; no account required for core prototype; static toolkit comparator with identical content; transparent rule-based selection; explanation of each suggestion; easy decline/change; safety boundaries; no automatic external actions; local ephemeral state by default.
P1: User-created favorites and opt-in recovery preferences; approved tool metadata; optional offline support-plan card; optional manual contact shortcuts requiring user action.
Later only after evidence: adaptive recommendations, AI wording adaptation, integrations with clinicians or peer groups, longitudinal outcome monitoring.

## Intervention metadata schema
Each item: unique ID; title; functional purpose; source tradition; original/licensed content status; evidence level and citations; intended scenario; eligibility/cautions; contraindications; duration; step-by-step script; user-choice alternatives; escalation boundary; reviewer; version; review date.

## Proposed starter library (candidates, not yet clinically approved)
ACT-informed: noticing thoughts/urges; values-to-next-action; acceptance and willingness.
DBT-informed: grounding; distress tolerance; emotion naming; interpersonal effectiveness preparation.
CBT/behavioral: functional chain reflection; environment adjustment; implementation intention.
Voluntary recovery: self-chosen boundaries/Three Circles reminder; meeting or sponsor contact option; nonpunitive post-setback review.
Integration: meaningful-life micro-action; review what helped.
Use original exercises and check intellectual-property/licensing rights for branded curricula, including Facing the Shadow.

## Safety requirements
Age 18+ for initial research. Clinical and lived-experience review before participant exposure. Distinguish moral incongruence from impairment. No coercive disclosure. No instruction to conceal wrongdoing. No AI-generated diagnosis or PTSD processing. Clear limits and professional/emergency pathways where relevant. Assess adverse reactions, shame, compulsive use, false reassurance, and dependency. Independent privacy/security review before collecting sensitive real-world data.

## Privacy requirements
No advertising targeting or data sale. No passive collection of browser history, precise location, contacts, or sexual behavior. No explicit sexual-history intake. No user text in third-party analytics. No default cloud journals or account. Clear deletion and retention. Neutral app/notification presentation. Consent-based, granular, revocable sharing. Threat model shared devices, screenshots, logs, backups, crash reports, vendor access, and account recovery. Assess HIPAA applicability and state consumer-health privacy laws rather than assuming coverage.

## Evaluation design
Compare identical reviewed content in (A) static toolkit and (B) context-sensitive selector. Randomized order; standardized non-graphic scenarios. Initial expert safety review, then formative adult usability sample (~8–12), then larger within-person comparative sample (~24–36) if warranted. Measures: blinded fit ratings, time to appropriate action, ability to decline, perceived relevance, usability, shame/distress, privacy comprehension, preference, adverse events. No efficacy claims from usability tests.

## Decision gates
Advance only if users experience a meaningful advantage over static tools and a relevant competitor workflow; independent reviewers find selections appropriate; safety and privacy requirements are met. Pivot if static tools perform as well, if human support dominates the value, or if clinician-led support is needed. Stop if serious unresolved harms or no meaningful unmet need.

## Open questions
Which segment benefits most? Is rule-based selection better than search? How much contextual information is necessary? Is connection more valuable than content? What should be local-only? What is a viable payer without exploiting vulnerability? Which competitors already provide equivalent functions? What evidence is needed for eventual clinical claims?
