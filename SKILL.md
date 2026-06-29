---
name: content-card-maker
description: Turn any article, notes, product, video, tutorial, workflow, or case study into a publish-ready visual content package for Xiaohongshu, WeChat Feed, or Douyin using a modular visual strategy, layout system, platform rules, output template, and quality review workflow.
---

# Content Card Maker

`content-card-maker` is a modular skill for creators who need
publish-ready visual content assets rather than text only.

This skill is an orchestrator.

It should not re-implement the logic that belongs to other modules.

---

## Use This Skill When

Use this skill when the user wants to turn source material into:

- Xiaohongshu image posts
- WeChat Feed / 小绿书 visual knowledge cards
- Douyin image-based content packages
- cover + content cards + ending card
- a full visual posting package instead of text-only copy

Typical inputs include:

- article
- notes
- product explanation
- tutorial
- workflow
- case study
- video topic
- creator draft

---

## Workflow

Follow this sequence exactly:

1. Read the user's source material and perform content analysis as an
   internal step.
2. Read `CARD_PLANNER.md` and use it to determine:
   - content mode
   - total cards
   - sequence logic
   - cover strategy
   - ending strategy
   - page-by-page roles and information density
3. Read `VISUAL_ENGINE.md` and use it to determine:
   - Topic
   - Secondary Topic
   - Audience
   - Platform intent
   - Content type
   - User goal
   - Information density
   - Emotional tone
   - Visual goal
   - Primary style preset
   - Secondary style preset
   - Layout preset
   - Color palette
   - Typography direction
   - Illustration direction
4. Read `STYLE_LIBRARY.md` and apply the selected style preset as the
   dominant visual system.
5. Read `LAYOUT_LIBRARY.md` and apply the selected layout preset as the
   structural logic for the card sequence.
6. Read `PLATFORM_RULES.md` and adapt the package to the chosen platform.
7. Read `PROMPT_ENGINE.md` and convert the card plan plus visual strategy
   into page-level prompts.
8. Detect whether an image generation tool is available in the current
   environment.
9. If an image tool is available, generate final cover, content cards,
   and ending card directly.
10. If no image tool is available, generate a complete HTML content page,
    open it in a browser, and export the rendered cards as PNG images.
11. If a preview sample, style sample, or first-pass reference image was
    generated earlier in the same task, align the final outputs to that
    reference before delivery.
12. Read `OUTPUT_FORMAT.md` and format the final answer using the fixed
    delivery structure.
13. Read `QUALITY_CHECK.md` and review the package before returning it.

---

## Operating Rules

- Do not ask the user to manually choose a style unless they explicitly
  require an override.
- Treat `Content Analysis` as an internal reasoning step by default.
- Keep one coherent visual system across the entire card package.
- If a style sample or preview image has already been shown to the user,
  the final output must remain visually close to that sample in palette,
  typography feel, composition energy, and finish level.
- Do not use a preview sample that looks significantly more polished than
  the final delivered cards.
- A sample image is a style commitment, not just inspiration.
- Prioritize mobile readability over decorative complexity.
- Compress messy input into a card-friendly structure before drafting.
- Keep one main point per page unless the page is explicitly a summary or comparison page.
- When the user asks for a visual content package, do not stop at text analysis.
- By default, continue through cover, body cards, ending card, layout plan,
  and image prompts.
- Only allow pure text output if the user explicitly says `只要文案`,
  `只要文字`, or an equivalent instruction.
- In the final reply, prioritize actual deliverables, previews, or links to
  generated assets over long process explanation.
- If the source is incomplete, make reasonable assumptions and label them
  clearly in the output.

---

## Module Responsibility

- `CARD_PLANNER.md`: decides page-by-page content structure and narrative sequence.
- `VISUAL_ENGINE.md`: decides the visual strategy.
- `STYLE_LIBRARY.md`: defines style preset details.
- `LAYOUT_LIBRARY.md`: defines layout structures.
- `PLATFORM_RULES.md`: defines platform-native constraints.
- `PROMPT_ENGINE.md`: converts card plan and visual strategy into consistent image prompts.
- `OUTPUT_FORMAT.md`: defines final response structure.
- `QUALITY_CHECK.md`: defines final review and pass criteria.

Do not duplicate module logic across files unless a short reference is
necessary for orchestration clarity.

---

## Output Requirement

Always return the final result using the exact top-level section order
defined in `OUTPUT_FORMAT.md`:

1. Final Assets
2. Visual Strategy
3. Card Plan
4. Card Structure
5. Image Prompt
6. Publishing Caption
7. Hashtags
8. Quality Review

Do not show `Content Analysis` to the user unless they explicitly ask for
analysis, rationale, or internal planning details.

---

## File Map

- `VISUAL_ENGINE.md`
- `CARD_PLANNER.md`
- `STYLE_LIBRARY.md`
- `LAYOUT_LIBRARY.md`
- `PLATFORM_RULES.md`
- `PROMPT_ENGINE.md`
- `OUTPUT_FORMAT.md`
- `QUALITY_CHECK.md`
