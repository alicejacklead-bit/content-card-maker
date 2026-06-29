# Output Format

## Purpose

This file defines the final delivery structure for `content-card-maker`.

The final output must always use the same section order so the skill is
predictable, easy to maintain, and easy to extend to new platforms later.

Do not change the top-level section names.

`Content Analysis` is an internal step by default and should not be shown
to the user unless they explicitly ask for analysis-only output or want to
inspect the reasoning.

---

## Fixed Section Order

1. Final Assets
2. Visual Strategy
3. Card Plan
4. Card Structure
5. Image Prompt
6. Publishing Caption
7. Hashtags
8. Quality Review

---

## Output Template

```md
## Final Assets

- Delivery Mode:
- Style Reference Used:
- Cover:
- Content Cards:
- Ending Card:
- Preview Link or File:
- Export Notes:

## Visual Strategy

- Visual Goal:
- Primary Style Preset:
- Secondary Style Preset:
- Layout Preset:
- Color Palette:
- Typography Direction:
- Illustration Direction:
- Strategy Reason:

## Card Plan

- Total Cards:
- Sequence Logic:
- Cover Strategy:
- Ending Strategy:
- Card 1:
  - Role:
  - Page Goal:
  - Main Message:
  - Supporting Message:
  - Visual Need:
  - Information Density:
- Card 2:
  - Role:
  - Page Goal:
  - Main Message:
  - Supporting Message:
  - Visual Need:
  - Information Density:
- Card 3:
  - Role:
  - Page Goal:
  - Main Message:
  - Supporting Message:
  - Visual Need:
  - Information Density:

Repeat until the sequence is complete.

## Card Structure

- Total Cards:
- Card 1:
  - Role:
  - Page Title:
  - Main Text:
  - Supporting Text:
  - Visual Focus:
- Card 2:
  - Role:
  - Page Title:
  - Main Text:
  - Supporting Text:
  - Visual Focus:
- Card 3:
  - Role:
  - Page Title:
  - Main Text:
  - Supporting Text:
  - Visual Focus:

Repeat until the sequence is complete, including cover and ending card.

## Image Prompt

- Global Art Direction:
- Card 1 Prompt:
- Card 2 Prompt:
- Card 3 Prompt:

Repeat until the sequence is complete.

## Publishing Caption

[Write one platform-native publishing caption.]

## Hashtags

- #tag1
- #tag2
- #tag3

## Quality Review

- Visual Consistency:
- Platform Fit:
- Card Planning Quality:
- Title Quality:
- Readability:
- Mobile Experience:
- Cover Strength:
- CTA Strength:
- Prompt Quality:
- Prompt Completeness:
- Delivery Completeness:
- Sample-to-Output Consistency:
- Final Risk Notes:
```

---

## Formatting Rules

- Keep the eight top-level sections in the exact order above.
- Do not add extra top-level sections.
- `Final Assets` comes first and should point the user to the real output.
- If a preview sample was shown earlier, `Final Assets` should state whether
  that sample was used as the visual reference.
- `Card Plan` defines page roles and narrative rhythm.
- `Card Structure` must describe each card separately.
- `Card Structure` is for the final readable page copy, not planning logic.
- `Image Prompt` must include both a global art direction and page-level prompts.
- Do not merge `Card Plan`, `Card Structure`, and `Image Prompt`.
- `Quality Review` must be evaluative, not decorative.
- Do not expose `Content Analysis` by default.
- If images or exported pages exist, prioritize links, previews, or file paths
  before any long explanation.
- If the source content is incomplete, keep the same output structure and
  mark assumptions clearly inside the relevant fields.
