# Recovery Companion — Resource Bank evidence brief v0.1

**Date:** 2026-10-14  
**Status:** Discovery draft; not clinical guidance, treatment, or an approved intervention library  
**Companion prototype:** [Resource Bank v0.7](../../prototype/resource-bank-v0.7.html)

## Decision

Build the first useful product slice as a small, browsable resource bank for adults voluntarily seeking change in unwanted sexual behavior. Organize by what a person wants help with right now; give each resource its source, evidence limits, steps, cautions, and an easy save option. Keep professional care and voluntary fellowship alongside self-help resources, with their different roles stated plainly.

Use **evidence-informed** for this bank. “Evidence-based tools” would overstate what we know: evidence usually concerns a full treatment program and a specific population, while these short, adapted cards have not themselves been tested. The evidence gap is especially large for short DBT- or IFS-inspired exercises used for sexual-behavior recovery.

## The user problem this slice addresses

The experience described for this work points to three practical barriers:

1. **No obvious first step:** a large set of modalities, books, programs, and recovery language can make a hard moment harder to navigate.
2. **Finding reliable resources:** people need a usable starting shelf that distinguishes clinical research, broader skill evidence, and community guidance.
3. **Human support is unevenly available:** a person may not have a sponsor yet, may not know what sponsorship is for, or may be unsure whether a particular peer is a good fit.

The bank should help someone choose an option, not diagnose them, define their recovery goal, replace care, or grade their commitment.

## Evidence summary: what can and cannot be said

| Approach/resource | What the available evidence supports | What it does not support here | Prototype treatment |
|---|---|---|---|
| CBT / behavioral treatment | A preregistered review identified 24 CSBD/PPU treatment studies through 2021 and found early evidence for CBT. A 2026 scoping review of 11 CBT-based PPU protocols reported promising results but found limited standardization and methodological rigor. | These reviews do not establish that any single micro-exercise in this bank is effective, nor that every user has CSBD/PPU; the 2026 review calls for stronger methods and protocol standards. | Include original functional reflection and flexible planning cards; label the evidence as early and direct to the broader treatment literature. |
| ACT | A small randomized study tested a multi-session ACT intervention for problematic internet pornography use. This is a direct signal for further study. | One small study of a treatment program does not establish a brief ACT-inspired prompt, benefit for all unwanted sexual behaviors, or CSBD treatment efficacy. | Include optional noticing/choice and user-defined values prompts; state that the micro-tools are untested. |
| DBT | DBT has a broader evidence base for emotion regulation in other clinical populations. | We found no basis to imply that a short DBT-inspired card is a validated sexual-recovery intervention. | Include only low-risk, optional skills adapted in original wording; describe support as indirect. Do not reproduce proprietary worksheets or imply a complete DBT program. |
| IFS | Recent IFS studies include small feasibility or pilot work in other populations, often delivered as clinician-led treatment. | Such work does not establish self-guided “parts work,” trauma processing, or a brief card for sexual recovery. | Mark any parts reflection explicitly “exploratory—not established for this use.” Keep it outside the default quick-start pair and remove it if lived-experience or clinical review finds it destabilizing. |
| SAA / sponsor support | SAA's official page describes a sponsor as a fellow member who guides the Twelve Steps; says fit matters, temporary and long-distance sponsorship may be options, and changing sponsors is acceptable. | Fellowship guidance is not clinical-outcome evidence. A sponsor is not necessarily a trained or licensed clinician and should not be represented as one. | Link to SAA's own material rather than copying it. Add an original fit conversation checklist and normalize attending meetings before choosing a sponsor. |
| CSAT / therapist directory | IITAP describes CSAT as a certification for licensed mental-health professionals. | A directory listing or certification alone cannot establish current license standing, treatment fit, or quality. The app has not verified providers. | Link to a directory only as a starting point; tell users to verify the underlying license, scope, fit, cost, and approach independently. |

### Evidence language used in the UI

- **CSB treatment evidence · early** — broader treatment-level evidence directly related to CSBD/PPU, but limited and not evidence for this card.
- **Direct PPU research · early** — a relevant ACT study exists; the study tested a program, not this prompt.
- **Broader evidence · indirect** — a broader approach has evidence in other populations; application to sexual recovery is uncertain.
- **Very early · not established for this use** — exploratory content only, not a recommendation or treatment claim.
- **Fellowship guidance · not clinical evidence** — community resource linked to the fellowship source.

Avoid “proven,” “clinically approved,” “works for compulsive sexual behavior,” “CSBD treatment,” or implied risk prediction.

## Candidate resource set

The prototype carries nine original, short resources. The table records their role; the exact step wording and cautions are in the HTML.

| ID | Resource | Situation | Approach | Evidence/status | Reviewer question |
|---|---|---|---|---|---|
| r1 | Notice the urge; choose the next move | In the moment | ACT-informed | Direct PPU research, early; card untested | Does “notice” feel agency-preserving and not like pressure to suppress? |
| r2 | Pause and orient to the room | In the moment / overwhelm | DBT-informed grounding | Broader evidence, indirect | Does external orientation feel optional and safe across trauma histories and disabilities? |
| r3 | Make a small plan for a high-risk moment | In the moment / planning | CBT / behavior change | CSB treatment evidence, early; card untested | Is “high-risk” too presumptive? Do alternatives avoid mandatory abstinence? |
| r4 | Look at the pattern without a verdict | After a hard moment | CBT-informed reflection | CSB treatment evidence, early; card untested | Could even brief reflection prompt rumination, shame, or unwanted detail? |
| r5 | Choose one action that matters to you | In the moment / after | ACT-informed | Direct PPU research, early; micro-step untested | Does the wording leave room for non-abstinence goals, faith, culture, and not choosing a value? |
| r6 | A compassionate parts check-in | Optional reflection | IFS-inspired | Very early; not established for this use | Should this be omitted until a qualified IFS clinician and lived-experience reviewers assess dissociation/trauma risks? |
| r7 | A simple reach-out message | Connection | Original peer-support prompt | Not a clinical treatment claim | Does the suggested message overpromise another person's availability or safety? |
| r8 | Find a sponsor at your pace | Fellowship | SAA peer-recovery guidance + original fit questions | Fellowship guidance, not clinical evidence | Are sponsor role/limits clear and is there no pressure to select one? |
| r9 | Explore a meeting or professional | Connection / care navigation | SAA and IITAP links | Directory link, not endorsement | Are directories and credentials framed accurately, with user-led verification? |

No card asks for graphic detail, diagnosis, a sexual history, a disclosure, a streak, or a behavior log. The IFS-inspired card does not ask about trauma or memories and is clearly outside the evidence-supported core.

## Sponsor scarcity and fit: design recommendation

Support the user's autonomy and practical next steps:

- Say that someone can attend a meeting without choosing a sponsor that day.
- Explain that fellowship sponsors are peers who share experience and guide program work; they are not therapy or crisis care.
- Offer fit questions about the sponsor's experience, working style, boundaries, availability, and what they do when a need falls outside their experience.
- Normalize asking for a temporary or long-distance sponsor, continuing to attend meetings, taking time, or changing sponsors. Link users to the fellowship's current materials and ask reviewers to verify the page is still accurate.
- Keep licensed therapy, medical care, medication questions, trauma treatment, and crisis support in their own lanes.
- Never rank, certify, match, contact, or privately score sponsors. Do not collect names or disclosures.

This is a product design proposal based on the user's reported barrier and SAA's published description of its own program. It is not evidence that a sponsor-match feature improves recovery.

## Local storage: narrow, explicit use

The prototype stores only a set of saved resource IDs in `localStorage` on the current browser/device. It does not save search terms, chosen categories, opened cards, feedback, free text, sexual behavior, or contact details. There is no app account, analytics, remote database, or sync.

Local storage is **not encrypted** and does not protect the items from another person who can access the same browser profile or device. Browser backups and device configuration are outside the prototype's control. The UI explains this before meaningful use and provides a visible “Clear saved resources” action. If storage is unavailable, saving fails with a plain explanation and the bank remains usable.

For a later real product, conduct a threat model and user review before treating browser storage as a privacy feature. Consider a no-save mode, neutral saved-item labels, private-session behavior, export/deletion semantics, and shared-device risk. Do not store notes in v0.

## Safety, trauma-informed, and scope rules

- Adults who voluntarily seek change; no diagnosis required. High libido, pornography use, relationship conflict, or moral disagreement alone does not establish a disorder.
- Offer choice, predictable steps, permission to skip/stop, plain language, external grounding alternatives, and no forced breathwork, body scan, disclosure, confession, or abstinence goal.
- Avoid trauma narratives, memory processing, exposure, interpretation, or claims that trauma caused the behavior. Trauma-focused treatment belongs with qualified professionals.
- Do not imply a person failed, relapsed morally, or needs this app to stay safe. Do not create streaks, urgency nudges, automatic alerts, monitoring, or sponsor/partner disclosure.
- Keep peer support, therapy, medicine, and crisis help distinct. The bank is not monitored and must not masquerade as crisis response.
- Re-review each exact card with a qualified clinician and paid lived-experience reviewers before participant exposure. Any material safety disagreement blocks that card. Obtain accessibility, privacy/security, ethics, and IP review as well.

## IP and provenance

All exercise wording in v0.7 is original draft language written for this prototype. It is not copied from DBT manuals, ACT worksheets, IFS materials, Facing the Shadow, SAA literature, or another proprietary curriculum. Fellowship content is linked to the source rather than reproduced. Approach labels identify inspiration, not affiliation, endorsement, certification, or license to reproduce manuals. Re-check rights and link use before release.

## What would falsify the product thesis

The resource bank is the intentionally strong, low-complexity comparator. The current thesis should be narrowed or stopped if users and reviewers find that:

- a clear static shelf makes the next step just as easy as context-sensitive routing;
- people mainly need an actually available and suitable human, which links and tools cannot provide;
- evidence labeling increases confusion or reads as false clinical authority;
- local saving reduces privacy confidence for people sharing devices;
- users prefer existing SAA, SMART, clinician, or other resources when surfaced clearly;
- the cards are not safe or useful enough after independent review to justify software.

## Smallest decision-changing experiment

After qualified clinical, lived-experience, IP, privacy/security, accessibility, and ethics review of this exact build, conduct eight paid formative sessions with adults who voluntarily want behavior change. Use fictional, non-graphic vignettes; no diagnosis or detailed histories. Ask each person to (1) find an acceptable next step in the resource bank and (2) use a comparable current route they already trust (for example, a static list or chosen recovery resource). Counterbalance order. Measure time-to-find, fit, agency, shame/distress, privacy comprehension, and whether the saved-resource explanation is understood.

This is a kill-screen, not a clinical efficacy test. Stop or revise if people misunderstand the evidence labels, feel pushed toward diagnosis/abstinence/disclosure, are destabilized, or do not find the bank more useful than a direct link to existing resources. Do not claim treatment benefit from this study.

## Sources checked

1. Grubbs et al. (2023), *Treatments and interventions for compulsive sexual behavior disorder with a focus on problematic pornography use: A preregistered systematic review*, Journal of Behavioral Addictions. https://pubmed.ncbi.nlm.nih.gov/36083776/ (24 studies through 2021; early evidence, especially CBT; quality/specificity limitations).
2. Crosby & Twohig (2016), *Acceptance and Commitment Therapy for Problematic Internet Pornography Use: A Randomized Trial*. https://pubmed.ncbi.nlm.nih.gov/27157029/ (small randomized treatment study; not this micro-exercise).
3. Kells et al. (2020), *Dialectical Behaviour Therapy for Emotion Regulation Difficulties: A Systematic Review*. https://doi.org/10.1017/bec.2019.9 (broader evidence, not specific to sexual recovery).
4. Ally et al. (2025), *A pilot study of an online group-based Internal Family Systems intervention for comorbid posttraumatic stress disorder and substance use*. https://pubmed.ncbi.nlm.nih.gov/40212833/ (N=10 pilot in another population; not evidence for self-guided sexual-recovery tools).
5. International Service Organization of SAA, *Sponsorship*. https://saa-recovery.org/our-program/sponsorship/ (current fellowship description; reviewed 2026-10-14).
6. IITAP, *Certifications Explained*. https://iitap.com/page/Certifications_Explained and therapist directory https://iitap.com/page/TherapistDirectory (provider claims source; not independently verified).
7. Zwielewski et al. (2026), *Cognitive behavioral therapy-based interventions for problematic pornography use: a scoping review*. https://pubmed.ncbi.nlm.nih.gov/42044011/ (11 CBT-based protocols from 2019–2024; promising reported results, but limited standardization and methodological rigor).
8. WHO (2024), *Clinical descriptions and diagnostic requirements for ICD-11 mental, behavioural and neurodevelopmental disorders*. https://www.who.int/publications/i/item/9789240077263/ (diagnostic guidance; use to preserve distinction between self-chosen goals and disorder).

## Change log

- v0.1 (2026-10-14): First evidence-labeled resource bank proposal and source/caution framework.
