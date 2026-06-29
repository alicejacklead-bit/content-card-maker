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
7. If the chosen platform is Xiaohongshu, read `XHS_CARD_SYSTEM.md` and
   enforce Xiaohongshu-native card behavior before production.
8. Read `PROMPT_ENGINE.md` and convert the card plan plus visual strategy
   into page-level prompts.
9. Detect whether an image generation tool is available in the current
   environment.
10. If an image tool is available, generate final cover, content cards,
   and ending card directly.
11. If no image tool is available, generate a complete HTML content page,
    open it in a browser, and export the rendered cards as PNG images.
12. If a preview sample, style sample, or first-pass reference image was
    generated earlier in the same task, align the final outputs to that
    reference before delivery.
13. Read `OUTPUT_FORMAT.md` and format the final answer using the fixed
    delivery structure.
14. Read `QUALITY_CHECK.md` and review the package before returning it.
15. If the package does not pass the quality gate, improve the visual
    delivery and re-run the review before returning it.

---

## Workbuddy Execution Contract

When this skill runs inside Workbuddy or any similar agent shell, do not
take the easiest generic rendering path just because it is faster.

For Xiaohongshu visual packages specifically:

1. The output must be treated as platform-native content cards, not a
   generic HTML page, not a dashboard, not a slide screenshot, and not a
   document-style checklist.
2. The package must include a real cover card, real body cards, and a real
   ending card.
3. The visual result must be judged against Xiaohongshu reading behavior:
   stop-scroll cover, save-worthy usefulness, strong Chinese readability,
   and clean card-by-card pacing.
4. If the current production path only yields a flat or utilitarian result,
   revise the composition, hierarchy, and card system rather than shipping
   the weak version.
5. Do not stop after creating one acceptable card. Ensure the full series
   remains consistent and complete.
6. If a preview sample exists, lock that direction and expand it into the
   full series. Do not switch visual systems midway.
7. If no preview sample exists and the platform is Xiaohongshu, the cover
   card should be treated as the first style-locking card for the series.
8. Do not silently downgrade to plain text, plain prompt output, or
   low-fidelity HTML when richer production is possible.

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
- For Xiaohongshu, prioritize native content-card feeling over generic
  cleanliness.
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
- Do not ship a Xiaohongshu package that looks like a dashboard, admin panel,
  document screenshot, productivity app screen, or plain slide deck.
- Do not treat large Chinese text blocks as acceptable design by default.
- Avoid uniform card composition across the whole series.
- For Xiaohongshu, the cover must have a stronger hook than the body cards,
  and the body cards must be more practical and easier to scan than the cover.
- If the visual output feels internationally polished but not platform-native,
  revise toward Xiaohongshu-native Chinese content-card behavior before delivery.
- A package that is merely "clear" but not "platform-fit" is not complete.

---

## Module Responsibility

- `CARD_PLANNER.md`: decides page-by-page content structure and narrative sequence.
- `VISUAL_ENGINE.md`: decides the visual strategy.
- `STYLE_LIBRARY.md`: defines style preset details.
- `LAYOUT_LIBRARY.md`: defines layout structures.
- `PLATFORM_RULES.md`: defines platform-native constraints.
- `XHS_CARD_SYSTEM.md`: defines what Xiaohongshu-native card behavior looks like and what should be rejected.
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
- `XHS_CARD_SYSTEM.md`
- `PROMPT_ENGINE.md`
- `OUTPUT_FORMAT.md`
- `QUALITY_CHECK.md`
