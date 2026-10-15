# UX simplification notes v0.2

**Date:** 2026-10-11  
**Prototype:** [Context selector v0.6](../../prototype/context-selector-v0.6.html)  
**Status:** Design proposal for expert review; untested

## What changed after v0.5

Owner feedback was direct: v0.5 felt “not delightful at all.” The issue was not just choice count. v0.5 reduced visible controls but produced a generic form-like page with little warmth, visual character, or rewarding interaction. That qualitative critique is design feedback from one owner, not user research.

v0.6 keeps the simplified information architecture and reworks the experience:

- Editorial two-part hero, with a small code-native path illustration to give the page a distinct visual anchor.
- Four moment choices presented as a balanced 2×2 set with restrained iconography and tactile hover/press states.
- A two-step progress cue, so the user can see the shape of the short interaction.
- Two starter tools shown as designed cards, followed by optional expansion and the complete library.
- A lightweight, optional response with immediate confirmation. It remains in page memory and is not transmitted.
- Warm paper, forest, and clay tones; system typography; consistent rounded surfaces; reduced-motion behavior.
- Expert-review status and the unreviewed-content warning remain visible.

The design references are translated into broad principles—clarity, restraint, precision, material warmth, hierarchy, and interaction craft. No Apple, Rams, Ive, or MetaLab trademarks, assets, or exact interface patterns are used.

## Hypothesis and counter-risk

The visual system and short guided path may make the first action easier to understand and more pleasant to explore. That is untested. Visual polish may also imply clinical authority that the content has not earned. The visible expert-review status, draft labels, and non-care statement must remain present. No efficacy or clinical claim is added.

## Decisions held constant

- The same 12 original draft exercises and cautions are used.
- One self-chosen moment is the only routing input.
- Starter pairs are fixed, explainable, and not ranked.
- People can change their choice, show more matches, or browse all tools.
- No account, tracking, browser storage, passive monitoring, or automatic contact.
- Participant exposure remains blocked pending all review and ethics gates.

## Verification status

Source checks confirm one HTML document, 12 draft items, valid JavaScript syntax, no page-level network/storage APIs, and reduced-motion handling. Rendered browser, keyboard, zoom/reflow, and screen-reader checks remain open. The hosted environment may receive ordinary connection metadata.

## Next test

First obtain independent clinical and lived-experience review of the exact v0.6 content and interaction mapping. Then test the static and guided routes with the same approved content. Retain v0.6 only if people understand the choices, feel free to reject them, and prefer the experience without a repeated burden, shame, privacy, or false-authority signal. A static index remains the stronger option if selection adds no meaningful value.
