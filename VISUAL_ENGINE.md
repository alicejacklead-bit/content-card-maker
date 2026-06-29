# Visual Intelligence Engine (VIE)

## Purpose

Visual Intelligence Engine (VIE) is the visual decision system for
`content-card-maker`.

Its responsibility is to analyze source content and determine the most
appropriate:

- Visual strategy
- Primary style preset
- Secondary style preset when helpful
- Layout preset
- Color palette
- Typography direction
- Illustration direction

The user should not manually choose a style in normal cases.

VIE acts as a content-aware Art Director, not a static topic mapper.

---

## Core Rule

Never choose styles randomly.

Never choose styles only by topic.

Always make decisions based on:

1. Topic
2. Secondary Topic
3. Platform
4. Audience
5. Content Type
6. User Goal
7. Information Density
8. Emotional Tone

---

## Decision Workflow

```text
Content
    ↓
Analyze Source Material
    ↓
Identify Primary Topic
    ↓
Identify Secondary Topic
    ↓
Identify Platform Intent
    ↓
Identify Audience
    ↓
Identify Content Type
    ↓
Identify User Goal
    ↓
Estimate Information Density
    ↓
Estimate Emotional Tone
    ↓
Determine Visual Goal
    ↓
Choose Primary Style
    ↓
Choose Secondary Style (optional)
    ↓
Choose Layout Preset
    ↓
Choose Color Palette
    ↓
Choose Typography
    ↓
Choose Illustration
    ↓
Generate Visual Strategy + Reason
```

---

## Decision Dimensions

### Topic

Topic identifies the main subject domain.

Examples:

- Health
- Fitness
- Beauty
- Education
- AI
- Business
- Product

### Secondary Topic

Secondary Topic adds context that changes the visual behavior inside the
same large category.

Examples:

- Health + fat loss
- Health + medical science
- AI + workflow
- AI + system architecture
- AI + product launch
- Product + comparison
- Business + founder story

### Platform

Platform changes the pacing, contrast, page count, and attention logic.

- Xiaohongshu: save-worthy, practical, card-friendly
- Douyin: fast, bold, instantly readable
- WeChat Feed / 小绿书: structured, knowledge-first, summary-friendly

### Audience

Audience changes the visual level of abstraction.

Examples:

- General consumers
- Creators
- Students
- Developers
- Founders
- Professionals
- Parents

### Content Type

Content type changes structural logic.

Examples:

- list
- tutorial
- workflow
- comparison
- framework
- case-study
- product-intro
- insight
- myth-busting

### User Goal

User goal changes the strength and tone of the visual system.

Examples:

- get saves
- build trust
- explain clearly
- look premium
- drive comments
- show proof
- simplify complexity

### Information Density

Information density determines whether the system should be more minimal,
more note-like, or more diagram-driven.

- Low: one big idea, hero-led, poster-like
- Medium: modular sections, light explanation
- High: note system, framework, diagram, structured density

### Emotional Tone

Emotional tone changes warmth, sharpness, restraint, and visual energy.

Examples:

- calm
- practical
- premium
- serious
- playful
- energetic
- reflective

---

## Baseline Topic Map

Use this only as a starting point, not the final answer.

| Topic | Baseline Primary Style |
| --- | --- |
| Health | Health Clean |
| Fitness | Active Clean |
| Beauty | Xiaohongshu Beauty |
| Fashion | Editorial Magazine |
| Food | Warm Lifestyle |
| Travel | Lifestyle Magazine |
| Education | Study Notes |
| Productivity | Notion Clean |
| AI | Apple Tech Minimal |
| Technology | Tech Blueprint |
| Business | Business Editorial |
| Finance | Finance Minimal |
| Career | Professional Notes |
| Parenting | Warm Parent |
| Pets | Cute Sticker |
| Psychology | Calm Wellness |
| Marketing | Growth Playbook |
| Product | Product Showcase |

---

## Decision Engine

### Rule 1: Topic Sets The Baseline

Start from the baseline topic map above.

Then adjust using the next rules.

### Rule 2: Secondary Topic Can Override The Baseline

If Secondary Topic changes the communication job, it can override the
default style.

Examples:

- `AI + workflow + creators`:
  Primary style tends toward `Notion Clean` or `Apple Tech Minimal`.
- `AI + system architecture + developers`:
  Primary style tends toward `Tech Blueprint`.
- `AI + product launch + business audience`:
  Primary style tends toward `Product Showcase` or `Business Editorial`.
- `Health + fat loss`:
  Primary style tends toward `Health Clean`.
- `Health + medical science`:
  Primary style tends toward `Health Clean` with `Professional Notes`
  as secondary restraint.
- `Fitness + training execution`:
  Primary style tends toward `Active Clean`.

### Rule 3: Audience Changes Abstraction Level

- For general consumers, prefer approachable and instantly understandable styles.
- For creators, prefer practical systems with clear card readability.
- For developers, prefer diagrammatic and systems-oriented styles.
- For business users, prefer credible, premium, or decision-oriented styles.
- For students, prefer note-based and study-friendly styles.

### Rule 4: Platform Changes Contrast And Pace

- Xiaohongshu favors practical, save-worthy, warm clarity.
- Douyin favors large type, higher contrast, stronger visual hooks.
- WeChat Feed favors cleaner structure and slightly higher knowledge density.

Platform can shift the same topic into different styles:

- `AI + workflow + Xiaohongshu` may lean `Notion Clean`.
- `AI + workflow + Douyin` may lean `Apple Tech Minimal` with stronger contrast.
- `AI + workflow + WeChat Feed` may lean `Tech Blueprint` if the goal is
  understanding system logic.

### Rule 5: Content Type Changes Layout And Visual Weight

- `list` favors clear modular scanning.
- `tutorial` favors progressive step hierarchy.
- `workflow` favors flow or pipeline logic.
- `comparison` favors split structure and contrast.
- `framework` favors diagram or note clarity.
- `case-study` favors transformation narrative.
- `product-intro` favors hero plus features.
- `insight` favors editorial or note-led commentary.
- `myth-busting` favors strong contrast and truth correction blocks.

### Rule 6: User Goal Changes The Final Tone

- If the goal is `save`, prioritize readability and utility.
- If the goal is `trust`, reduce visual noise and increase clarity.
- If the goal is `premium perception`, increase polish and restraint.
- If the goal is `instant stop-scroll`, increase contrast and headline dominance.
- If the goal is `explain complexity`, increase structure and diagram clarity.

### Rule 7: Information Density Changes Style Tightness

- Low density content can support hero-driven and editorial presentation.
- Medium density content fits modular card systems.
- High density content should favor study, notes, grid, or blueprint logic.

Typical density adjustments:

- High density + education -> `Study Notes`
- High density + workflow -> `Notion Clean` or `Tech Blueprint`
- High density + professional guidance -> `Professional Notes`

### Rule 8: Emotional Tone Changes Surface Treatment

- Calm -> softer palette and lower contrast
- Practical -> clean utility-first treatment
- Premium -> restrained typography and polished spacing
- Serious -> more disciplined hierarchy, fewer playful elements
- Playful -> rounder forms and lighter illustrations
- Energetic -> bold type and stronger accents

---

## Primary And Secondary Style Logic

### Primary Style

Primary Style is the dominant visual system.

It controls:

- Background logic
- Main palette direction
- Typography family direction
- Illustration family
- Overall composition behavior

### Secondary Style

Secondary Style is optional.

Use it only when the content has a second communication need that the
Primary Style alone does not fully express.

It may influence:

- accent modules
- diagram treatment
- supporting icons
- secondary color accents
- page-specific refinements

It must not replace the Primary Style.

### Style Blending Rule

Style blending is allowed only when:

1. one Primary Style remains dominant
2. the blend serves a clear communication reason
3. the final package still feels like one series

Good blending examples:

- `Health Clean` + `Professional Notes` for health education that must feel
  both gentle and credible
- `Apple Tech Minimal` + `Notion Clean` for creator-friendly AI workflows
- `Business Editorial` + `Product Showcase` for a premium product launch
- `Study Notes` + `Growth Playbook` for actionable educational marketing content

Bad blending examples:

- mixing `Cute Sticker` with `Finance Minimal` without a strong reason
- changing the whole style every page
- using Secondary Style as a second unrelated brand system

---

## Content Type To Layout Guidance

| Content Type | Recommended Layout Direction |
| --- | --- |
| list | Numbered List / Checklist / Grid Cards |
| tutorial | Step-by-Step / Timeline / Notebook |
| workflow | Flowchart / Pipeline / Step-by-Step |
| comparison | Comparison / Before vs After / Matrix |
| framework | Pyramid / Matrix / Mind Map / Notebook |
| case-study | Problem -> Solution -> Result |
| product-intro | Hero + Features / Feature Grid |
| insight | Editorial / Quote + Breakdown |
| myth-busting | Comparison / FAQ Cards / Numbered List |

---

## Color Direction Rules

Color should follow the chosen Primary Style, then be tuned by platform
and tone.

Examples:

- `Health Clean` -> white, light green, muted yellow
- `Apple Tech Minimal` -> white, black, electric blue
- `Notion Clean` -> white, warm gray, beige
- `Business Editorial` -> navy, white, muted gold
- `Study Notes` -> cream, light blue, highlight green
- `Warm Lifestyle` -> cream, beige, terracotta

Adjustment rules:

- Douyin can push higher contrast
- Xiaohongshu can add warmth and softness
- WeChat Feed can reduce decoration and increase structural clarity

---

## Typography Direction Rules

Choose the typography direction that best matches both style and content
job:

- Bold Minimal
- Clean Sans
- Notebook
- Magazine Editorial
- Tech UI

Examples:

- `Study Notes` -> Notebook
- `Tech Blueprint` -> Tech UI
- `Editorial Magazine` -> Magazine Editorial
- `Health Clean` -> Clean Sans
- `Growth Playbook` -> Bold Minimal

---

## Illustration Direction Rules

Choose the illustration direction that supports clarity rather than
decoration:

- Flat Icons
- 3D Soft Objects
- Photo Editorial
- Hand-drawn Notes
- UI Mockups
- Cute Stickers

Examples:

- health education -> Flat Icons
- AI workflow -> UI Mockups
- fashion story -> Photo Editorial
- study summary -> Hand-drawn Notes

---

## Final Output Format

```md
## Visual Strategy

- Topic:
- Secondary Topic:
- Platform:
- Audience:
- Content Type:
- User Goal:
- Information Density:
- Emotional Tone:
- Visual Goal:
- Primary Style Preset:
- Secondary Style Preset:
- Layout Preset:
- Color Palette:
- Typography:
- Illustration:
- Strategy Reason:
```

---

## Decision Examples

### Example 1

Input:

> AI 视频工作流，发给小红书创作者

Output direction:

- Topic: AI
- Secondary Topic: workflow
- Platform: Xiaohongshu
- Audience: creators
- Content Type: workflow
- User Goal: save + understand quickly
- Information Density: medium
- Emotional Tone: practical
- Primary Style Preset: Notion Clean
- Secondary Style Preset: Apple Tech Minimal
- Layout Preset: Pipeline
- Color Palette: white + warm gray + muted blue
- Typography: Clean Sans
- Illustration: UI Mockups
- Strategy Reason: creators need practical clarity more than engineering abstraction

### Example 2

Input:

> AI 系统架构说明，发给开发者

Output direction:

- Topic: AI
- Secondary Topic: system architecture
- Platform: WeChat Feed
- Audience: developers
- Content Type: framework
- User Goal: explain complexity
- Information Density: high
- Emotional Tone: serious
- Primary Style Preset: Tech Blueprint
- Secondary Style Preset: Apple Tech Minimal
- Layout Preset: Flowchart
- Color Palette: navy + blue + white
- Typography: Tech UI
- Illustration: UI Mockups
- Strategy Reason: the audience needs structured system logic and high-density clarity

### Example 3

Input:

> 减肥核心 8 点，发小红书

Output direction:

- Topic: Health
- Secondary Topic: fat loss habits
- Platform: Xiaohongshu
- Audience: general consumers
- Content Type: list
- User Goal: save + trust
- Information Density: medium
- Emotional Tone: practical
- Primary Style Preset: Health Clean
- Secondary Style Preset: Active Clean
- Layout Preset: Numbered List
- Color Palette: white + light green + muted yellow
- Typography: Clean Sans
- Illustration: Flat Icons
- Strategy Reason: the topic needs credibility and friendliness, while the fat loss angle benefits from light energy accents without losing trust
