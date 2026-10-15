# Outbound support links — research and UX recommendation v0.1

**Reviewed:** 2026-10-14  
**Status:** Public-source review and prototype content; not a service-quality audit, endorsement, clinical review, or user validation.  
**Prototype:** [`resource-bank-v0.9.html`](../../prototype/resource-bank-v0.9.html)

## Decision

Present support links as three distinct jobs: **find a peer meeting**, **explore peer sponsorship**, and **explore professional care**. Each should use a short, descriptive action link, identify the organization and what it offers, and state the boundary that matters before the person leaves the guide. Do not put all three in one generic “find help” directory card.

Use official organizational directories as the first source for their own meetings, fellowship guidance, or credentials. State what the organization itself says the directory can establish, and what it cannot. Keep the guide’s own selection, search, and saved-item state out of outbound URLs; do not request location or identifying information in the guide. If a person chooses to provide details on another site, that site controls its own handling.

This is a **curated handoff hypothesis**, not evidence that the guide improves access, sponsor fit, therapy quality, or recovery outcomes. Directories and attractive link cards are easy to reproduce. The harder-to-copy work, if it proves valuable, would be careful source maintenance, fit-sensitive explanations, respectful boundaries, and tested link navigation.

## Source review

| Need | Primary source reviewed | What it verifies | What it does not verify | Prototype treatment |
|---|---|---|---|---|
| SAA meetings | [SAA meeting finder](https://www.saa-meetings.org/) | Current public directory offers filters including location, meeting type, access, gender, focus, language, and topic. | That a listing is active, safe for a particular person, or a good fit; directory alone is not a quality review. | Direct link; tell the user to review format and access details. No in-app geolocation or location prefill. |
| SLAA meetings | [SLAA Fellowship-Wide Services meeting finder](https://slaafws.org/meetings/) | Official page lists in-person, online, and phone meeting pathways and links to sponsorship resources. The page says FWS does not administer the listed meetings. | Meeting-level oversight or fit. | Present as a distinct fellowship option and use SLAA’s own language. |
| Broader behavior-change meetings | [SMART Recovery meetings](https://smartrecovery.org/meeting) | SMART describes free peer meetings for addictive/problematic behaviors, including online and in-person options. | A sex-behavior-specific program or proof that its meetings address each visitor’s concern. | Optional alternative with an explicit “broader, not sex-behavior-specific” label. |
| SAA sponsor guidance | [SAA sponsorship overview](https://saa-recovery.org/our-program/sponsorship/) and [“Getting a Sponsor” page](https://saa-recovery.org/literature/getting-a-sponsor/) | SAA says a temporary sponsor can be used while a newcomer gets to know the group, changing sponsors is acceptable, and fit matters. | Training, clinical competence, safeguarding, or a standardized sponsor vetting process. | Link to SAA’s own material. Keep original fit questions clearly labeled as this guide’s prompts, not SAA-approved literature. |
| SLAA sponsor guidance | [SLAA “How to Find a Sponsor”](https://slaafws.org/what-is-sponsorship/how-to-find-a-sponsor/) | SLAA suggests listening, asking potential sponsors questions, and considering temporary sponsors, co-sponsors, or recovery partners. | A guarantee of availability or suitability; standardized training or clinical competence. | Offer as another fellowship’s guidance, not as interchangeable with SAA’s approach. |
| CSAT search | [IITAP Therapist Directory](https://iitap.com/page/TherapistDirectory) | IITAP offers directory search related to CSAT and states that it is not a governing body over mental-health practice and that its directory is for search purposes. | Current independent licensure, standing, scope, quality, or fit. | Link with the limitation beside it; name its sex-addiction framing as optional language, and ask the person to verify the underlying license and evaluate fit. |
| Sexuality-focused therapy | [AASECT referral directory](https://www.aasect.org/referral-directory) and [credential scope](https://www.aasect.org/certification-types-distinguishing-sexuality-educators-counselors-and-therapists) | Directory allows country/state search. AASECT describes Certified Sex Therapists as licensed mental-health professionals with specialized sexuality training. | That a listed clinician specializes in unwanted sexual behavior, shares a person’s goals, or is currently licensed in the person’s jurisdiction. | Present as an additional route, not a substitute for a CSAT search or license verification. |
| Primary-source license check | [ASWB license lookup](https://www.aswb.org/licenses/protecting-the-public/look-up-license/) and [ASPPB licensing-board contacts](https://asppb.net/contact-licensing-board/) | These professional associations point users to social-work and psychology regulatory boards. | A universal lookup for every profession or jurisdiction; the provider must be checked against the regulator responsible for their license. | Label by profession; for other credentials, direct the person to the relevant state/provincial regulator. |

## Recommended link-card anatomy

1. **Action first:** “Find a meeting,” “Read how sponsorship works,” or “Search for a therapist.”
2. **Name the source:** organization name and the exact purpose of its page.
3. **One-line expectation:** what the person will find there and any important gap (e.g., “broad behavior-change meetings”).
4. **Fit and role boundary:** peer support is not clinical care; directories are not endorsements; a credential is not a guarantee of fit.
5. **External-site notice:** the guide does not send saved items or selections; details entered at the destination are handled by that organization. Avoid claiming anonymous or private browsing.
6. **Deliberate opening:** direct HTTPS link, visible external-link cue, accessible name, `noopener noreferrer`, and `referrerpolicy="no-referrer"`. Avoid redirectors, affiliate links, analytics parameters, and auto-passing search/location.
7. **Maintenance metadata:** source owner, URL, what it substantiates, review date, and next review date in the content register. Recheck links before each release; do not silently convert a stale link into a product recommendation.

## Product boundaries

- Do not rank people or meetings, create sponsor-matching claims, or accept applications for sponsors.
- Do not collect a visitor’s city, ZIP code, license search, meeting click, care interest, or sexual-behavior details.
- Do not copy fellowship literature or branded worksheets. Link to official pages and write original summaries/prompts.
- Keep SAA, SLAA, SMART, CSAT, and AASECT distinct. Each is a route someone may explore; none is the default path.
- The current prototype’s outbound choices are static and U.S.-oriented in places. Before broader distribution, add jurisdiction coverage or clearly scope the directory list; do not imply completeness.

## Falsifiable UX question

Do separate, labeled handoffs help people reach an option they would actually consider, compared with a single generic directory card, while preserving understanding of (a) peer versus clinical roles, (b) endorsement limits, and (c) what data leaves the guide?

Test with fictional scenarios and no location or personal behavior disclosure. Failure signals include a visitor believing the product vetted a specific sponsor/provider, believing a CSAT certificate is a government license, or thinking an external directory receives no browser/device data. A successful click-through is not evidence that the destination was useful or safe.

## References

Official source pages listed above; reviewed 2026-10-14. Link availability and directory content can change. No meeting, sponsor, clinician, or provider was contacted or assessed.
