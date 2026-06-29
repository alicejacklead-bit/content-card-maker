# Prompt Engine

## Purpose

`PROMPT_ENGINE.md` converts the content and visual decisions into stable,
series-consistent image prompts.

It combines:

- Visual Strategy
- Style Library
- Layout Library
- Card Planner
- Platform Rules

Its job is not to re-plan the content.

Its job is to translate the chosen direction into prompt language that
is consistent, readable, and production-ready.

Its output is not the final stopping point when the user asked for a
visual package.

The prompt set should be used to produce actual images when an image tool
is available, or to drive a rendered HTML-to-PNG fallback when no image
tool is available.

---

## Inputs

Use all of the following:

1. `Visual Strategy`
2. selected style definition from `STYLE_LIBRARY.md`
3. selected layout definition from `LAYOUT_LIBRARY.md`
4. page-by-page sequence from `CARD_PLANNER.md`
5. platform behavior from `PLATFORM_RULES.md`
6. any approved preview sample or style reference already shown to the user

---

## Core Prompt Rules

Every prompt set must include:

- one Global Art Direction block
- one prompt per card

For Xiaohongshu, every prompt set must be written as a content-card series
rather than a generic poster set or generic product page.

Every card prompt must include:

- Global Art Direction reference
- Page Role
- Page Goal
- Main Text
- Supporting Text
- Layout Preset
- Composition
- Typography
- Color Palette
- Illustration Direction
- Background
- Visual Hierarchy
- Mobile Readability
- Consistency Rule
- Negative Prompt

---

## Series Consistency Rules

- Keep one dominant primary style across the full series.
- Let the secondary style influence accents only when needed.
- The cover, content pages, and ending page must look like one family.
- Do not repeat the exact same composition on every page.
- Vary composition while preserving the same palette, type direction, and illustration family.
- For Xiaohongshu, preserve series unity while letting each card feel like
  a native card in a carousel rather than cloned slides.
- If a preview sample exists, inherit its finish level, visual energy,
  polish, and overall aesthetic direction.
- Final assets must not feel like a downgrade from the preview sample.
- The preview sample and the delivered set should look like they belong to
  the same campaign, not two different rendering systems.

---

## Role-Based Prompt Rules

### Cover Page

The cover prompt must be stronger than the body pages.

It should emphasize:

- one clear hook
- strongest hierarchy
- highest stop-scroll value
- simplest immediate read
- Xiaohongshu-native hook language with large Chinese title blocks
- stronger contrast and more visible save-worthy value framing

### Content Pages

The content prompt must be clearer than the cover.

It should emphasize:

- one core point per page
- strong text organization
- easy scan path
- large readable Chinese text
- practical, save-worthy structure over decorative layout
- visually varied but still recognizably part of the same Xiaohongshu series

### Ending Page

The ending prompt must provide closure.

It should emphasize:

- summary or CTA
- emotional resolution
- lighter cognitive load
- still visually consistent with the series
- a clear reason to save, follow, or reference later when platform fit calls for it

---

## Mobile Readability Rules

Every prompt should explicitly protect mobile readability:

- large Chinese typography
- short visible text blocks
- strong contrast between text and background
- obvious title area
- clear safe area for text
- avoid crowding the edges
- avoid long paragraph blocks that feel like article screenshots
- keep visible Chinese copy short enough to scan without zooming

If the page has multiple text layers, the hierarchy must still be obvious
at phone size.

---

## Composition Rules

Composition should be chosen from the selected layout preset, then tuned
to page role.

Examples:

- Cover: stronger hero focal point
- Middle content page: more modular sections
- Comparison page: balanced split structure
- CTA page: cleaner closing layout

Do not use identical module placement on every page.

For Xiaohongshu:

- do not default to flat checklist software UI
- do not default to dashboard modules
- do not default to presentation slide composition
- do not default to generic productivity-app framing
- prefer card-like visual blocks, stronger hook typography, and obvious
  value cues such as summary chips, emphasis strips, quick labels, or
  highlighted takeaways when they fit the content

---

## Negative Prompt Rules

Every card prompt should include a negative prompt section.

Common negative goals:

- no tiny unreadable Chinese text
- no overcrowded layout
- no excessive paragraphs
- no random mixed styles
- no low-contrast text
- no distorted anatomy or irrelevant decorative objects
- no repeated identical composition across all cards
- no document screenshot feeling
- no app UI mockup feeling unless the content explicitly requires software UI
- no plain PowerPoint or meeting-note feeling

Add more negative constraints if the chosen style or platform has a
clear failure mode.

---

## Production Rule

After prompts are assembled:

- if an image generation tool exists, generate final cover, content cards,
  and ending card directly
- if no image generation tool exists, build a complete HTML visual page
  from the card plan and visual strategy, render it in a browser, and
  export PNG screenshots

When using HTML fallback for Xiaohongshu:

- build actual high-fidelity vertical social cards
- render one card per page role
- do not render a generic long page and treat it as enough
- do not ship raw checklist visuals without card-level art direction
- revise the fallback output if it looks flat, plain, or obviously utilitarian

Do not stop at prompt text alone unless the user explicitly asks for
copy-only output.

If a preview sample has already been shown and the fallback rendering path
cannot stay reasonably close to that sample, revise the production path
instead of silently shipping a mismatched result.

---

## Prompt Assembly Workflow

```text
Read Visual Strategy
    ↓
Load Style Preset Definition
    ↓
Load Layout Preset Definition
    ↓
Load Card Plan
    ↓
Load Platform Rules
    ↓
Write Global Art Direction
    ↓
Write Cover Prompt
    ↓
Write Content Page Prompts
    ↓
Write Ending Prompt
    ↓
Check Consistency + Readability + Negative Prompt
```

---

## Global Art Direction Template

```md
## Global Art Direction

Create a cohesive [platform] visual card series in a 3:4 vertical social
media format.

Primary style:
Secondary style:
Overall feeling:
Layout system:
Color palette:
Typography direction:
Illustration direction:
Background treatment:
Consistency rule:
Mobile readability rule:
```

---

## Card Prompt Template

```md
## Card 1 Prompt

Create a 3:4 vertical social media card for [platform].

Page role:
Page goal:
Main text:
Supporting text:
Layout preset:
Composition:
Typography:
Color palette:
Illustration direction:
Background:
Visual hierarchy:
Mobile readability:
Consistency rule:
Negative prompt:
```

Repeat for every card.

---

## Prompt Quality Standard

A good prompt set should:

- preserve one coherent series identity
- make the cover more attention-grabbing
- make content pages more legible
- make the ending page feel conclusive
- adapt the same style to different page roles
- explicitly instruct large, clear, readable Chinese text

If the prompts only describe style and do not describe page role,
composition, hierarchy, and readability, they are incomplete.
