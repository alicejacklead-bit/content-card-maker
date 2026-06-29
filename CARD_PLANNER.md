# Card Planner

## Purpose

`CARD_PLANNER.md` turns source material into a page-by-page card plan.

It is a content structure module, not a visual style module.

It does not choose the final style preset.

It does not write the final image prompt.

It decides:

- total page count
- cover hook strategy
- page-by-page topic allocation
- narrative order
- where to summarize
- how to end with a CTA
- how much information each page should carry

The main rule is simple:

One page should carry one main point.

---

## Responsibilities

`CARD_PLANNER.md` is responsible for:

- analyzing the source material
- selecting a content mode
- deciding total cards
- deciding sequence logic
- planning cover, body, summary, and ending roles
- controlling per-page information density
- keeping the card series mobile-friendly

It is not responsible for:

- choosing the final style preset
- choosing detailed palette or typography
- generating final image prompts

---

## Supported Content Modes

- list
- tutorial
- workflow
- comparison
- framework
- case-study
- product-intro
- insight
- myth-busting

---

## Planning Workflow

```text
Source Material
    ↓
Identify Core Topic
    ↓
Identify Content Mode
    ↓
Estimate Audience Knowledge Level
    ↓
Estimate Total Useful Points
    ↓
Choose Card Count
    ↓
Set Sequence Logic
    ↓
Design Cover Hook
    ↓
Assign One Main Point Per Page
    ↓
Add Summary Or CTA If Needed
    ↓
Generate Card Plan
```

---

## Card Count Rules

Use page count based on both platform and content volume.

### Xiaohongshu

- short practical topic: 5 to 7 cards
- standard knowledge post: 6 to 9 cards
- denser educational content: 7 to 10 cards if readability remains strong

### WeChat Feed / 小绿书

- structured summary: 4 to 7 cards
- denser framework content: 5 to 8 cards

### Douyin

- compact image post: 3 to 6 cards
- compress to high-impact pages only

### Compression Rule

If there are too many points:

- merge small related points
- move low-priority detail into supporting text
- keep one strong point per page

### Expansion Rule

If there are too few points:

- add context page
- add myth correction page
- add summary page
- add CTA page

Do not add filler pages.

---

## Sequence Logic Rules

Choose the sequence that best helps the audience understand and keep
reading.

Common sequence patterns:

- Hook -> Key Points -> Summary -> CTA
- Hook -> Problem -> Method -> Result -> CTA
- Hook -> Step 1 -> Step 2 -> Step 3 -> Summary
- Hook -> Myth -> Truth -> Method -> Reminder -> CTA
- Hook -> Feature Overview -> Feature Details -> Recommendation -> CTA

The sequence should feel progressive, not repetitive.

---

## Cover Strategy Rules

The cover should do one of the following:

- promise a useful outcome
- frame a problem people care about
- package a list into a save-worthy promise
- summarize a complex topic into a simpler payoff
- create curiosity without becoming vague

Good cover behavior:

- obvious value in one glance
- short main message
- specific topic framing
- strong mobile readability

Bad cover behavior:

- too many claims
- generic motivational language
- no concrete value

---

## Ending Strategy Rules

The ending card should do at least one job:

- summarize the core takeaway
- reinforce a practical next step
- invite save or comment
- invite the audience to reflect or compare experience

Good ending behavior:

- low cognitive load
- clear wrap-up feeling
- CTA aligned with platform and topic

Bad ending behavior:

- introducing a brand-new topic
- hard-selling without context
- ending abruptly with no closure

---

## Information Density Rules

Each page should be assigned one of the following:

- Low: hero message, short takeaway, single hook
- Medium: one main point with one support line
- High: one structured point with short sub-parts only if the layout supports it

Do not put multiple equal-weight ideas on one page unless the page is
explicitly a summary or comparison page.

---

## Content Mode Planning Patterns

### list

Default sequence:

- Cover
- Point 1
- Point 2
- Point 3
- Point 4
- optional additional points
- Summary / CTA

Best for:

- practical saves
- concise educational posts

### tutorial

Default sequence:

- Cover
- Why it matters
- Step 1
- Step 2
- Step 3
- Summary / CTA

### workflow

Default sequence:

- Cover
- Workflow overview
- Stage 1
- Stage 2
- Stage 3
- Key reminder
- CTA

### comparison

Default sequence:

- Cover
- Comparison frame
- Side A
- Side B
- Verdict / How to choose
- CTA

### framework

Default sequence:

- Cover
- Framework overview
- Part 1
- Part 2
- Part 3
- Summary / application
- CTA

### case-study

Default sequence:

- Cover
- Starting problem
- What changed
- What was done
- Result
- Transferable lesson
- CTA

### product-intro

Default sequence:

- Cover
- Product promise
- Feature 1
- Feature 2
- Feature 3
- Who it is for
- CTA

### insight

Default sequence:

- Cover
- Core thesis
- Supporting idea 1
- Supporting idea 2
- Counterpoint or nuance
- Takeaway
- CTA

### myth-busting

Default sequence:

- Cover
- Myth statement
- Truth statement
- Why people misunderstand it
- What to do instead
- Summary / CTA

---

## Output Format

```md
## Card Plan

- Total Cards:
- Sequence Logic:
- Cover Strategy:
- Ending Strategy:

### Card 1
- Role: Cover
- Page Goal:
- Main Message:
- Supporting Message:
- Visual Need:
- Information Density:

### Card 2
- Role:
- Page Goal:
- Main Message:
- Supporting Message:
- Visual Need:
- Information Density:
```

Repeat until the sequence is complete.

---

## Planning Checklist

Before finalizing the card plan, confirm:

- each page has one dominant point
- the cover has a real hook
- the order is logical
- there is closure near the end
- the CTA fits the platform
- the total page count matches attention span
