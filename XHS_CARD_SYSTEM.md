# XHS Card System

## Purpose

`XHS_CARD_SYSTEM.md` defines what a Xiaohongshu-native content card series
should look like inside `content-card-maker`.

This file exists to prevent generic output.

It does not replace:

- `CARD_PLANNER.md`
- `VISUAL_ENGINE.md`
- `STYLE_LIBRARY.md`
- `LAYOUT_LIBRARY.md`

Instead, it constrains them for Xiaohongshu execution.

Its job is to answer:

- what makes a card feel like Xiaohongshu
- what makes a card feel wrong for Xiaohongshu
- how cover, body, and ending cards should behave
- how Chinese content should be arranged for mobile reading

---

## Core Rule

For Xiaohongshu, the goal is not only visual cleanliness.

The goal is:

- stop-scroll cover
- save-worthy usefulness
- strong Chinese readability
- clear card-by-card pacing
- platform-native emotional tone

If a result is merely clean, minimal, or modern but does not feel like a
Xiaohongshu content card set, it is not complete.

---

## System Position

For Xiaohongshu output, apply this file after:

1. `CARD_PLANNER.md` decides page roles
2. `VISUAL_ENGINE.md` decides style direction
3. `STYLE_LIBRARY.md` provides the dominant style preset
4. `LAYOUT_LIBRARY.md` provides structural patterns

Then use this file to translate all of the above into Xiaohongshu-native
card behavior.

---

## Xiaohongshu Success Definition

A strong Xiaohongshu card set usually has all of these traits:

- The cover can be understood in one glance.
- The headline feels useful, specific, and worth saving.
- The body cards are easier to scan than the cover.
- Each page has one obvious point.
- Text is large enough for phone reading.
- The series feels practical, not abstract.
- There is enough visual pull to feel like platform content.
- The ending card gives closure, summary, or a natural CTA.

---

## Xiaohongshu Fail Definition

The result should be treated as failed if it looks like any of these:

- a dashboard
- a software interface
- a slide deck
- a meeting note screenshot
- a document page
- a generic web section
- a poster series with no practical structure

Even if the output is readable, it fails if it does not feel like a
native Xiaohongshu content package.

---

## Card Roles

### 1. Cover Card

The cover card is not a summary slide.

It is a hook card.

Its job is:

- stop the scroll
- state the promise clearly
- frame the topic fast
- create a reason to keep swiping

The cover should usually include:

- one dominant Chinese headline
- one strong outcome, warning, or curiosity angle
- one clean supporting line if needed
- one focal visual anchor or strong visual block

The cover should not:

- explain too much
- contain many equal-weight bullets
- look like a software UI
- look like a plain title slide

### 2. Body Card

The body cards are the utility core of the set.

Their job is:

- deliver the information clearly
- make the content easy to save or reference
- keep one main point per page
- maintain visual consistency without repeating one rigid template

Each body card should usually include:

- one page title
- one key takeaway
- one chunked explanation
- one practical support structure

Support structures may include:

- short bullets
- numbered modules
- comparison blocks
- highlights
- labeled zones
- emphasis strips
- warnings
- do / do not pairings

The body card should not:

- use long article paragraphs
- use tiny secondary text
- hide the main point
- become more decorative than informative

### 3. Ending Card

The ending card is not filler.

Its job is:

- close the sequence cleanly
- summarize the mindset or action
- provide a natural next step

Common ending card roles:

- summary reminder
- final principle
- quick checklist recap
- CTA to save, follow, comment, or reference later

The ending card should feel lighter than a dense body page while still
belonging to the same series.

---

## Headline System

### Cover Headlines

Cover headlines for Xiaohongshu should usually be:

- short
- concrete
- high-contrast
- easy to scan
- visually dominant

Good cover headline patterns:

- `X 个...`
- `真正有用的...`
- `别再...`
- `先搞清...`
- `新手最容易忽略的...`
- `开播前先做这几步`
- `这套方法我现在一直在用`

Cover headline behavior:

- one dominant line or two stacked lines
- strongest type size in the series
- strongest contrast in the series

### Body Headlines

Body headlines should be:

- more practical than dramatic
- directly related to the page point
- shorter than the explanation copy

### Ending Headlines

Ending headlines should be:

- summarizing
- decisive
- easy to remember

---

## Chinese Typography Rules

For Xiaohongshu, Chinese readability must be treated as a primary design
constraint.

Rules:

- Use visibly large Chinese titles.
- Prefer short text blocks over dense paragraphs.
- Let key phrases carry more weight than full sentences.
- Break text into chunks that can be scanned in seconds.
- Keep line lengths comfortable on a 3:4 phone-oriented card.
- Use hierarchy through size, weight, contrast, and spacing.

Avoid:

- tiny supporting text
- narrow, compressed text columns
- paragraph-heavy explanation
- too many equal-weight text blocks
- pale text with low contrast

---

## Composition Rules

For Xiaohongshu, card composition should feel like a content card, not a
desktop layout.

Preferred composition behaviors:

- clear top hook area
- obvious focal zone
- large text-safe area
- modular information blocks
- comfortable edge padding
- one dominant path through the card

Allowed variety across the series:

- some pages can be more title-led
- some pages can be more module-led
- some pages can use comparison or flow structures

But the series should not:

- use exactly the same block positions on every page
- swing between unrelated systems
- become visually rigid like copied slides

---

## Information Density Rules

Xiaohongshu cards are not posters, but they are also not article pages.

Recommended density by role:

- Cover: low
- Body: medium
- Ending: low to medium

Density should feel:

- compact enough to be useful
- open enough to be readable

Too little density creates:

- empty design-board feeling
- weak usefulness

Too much density creates:

- document screenshot feeling
- low save value because the card is hard to use

---

## Visual Devices That Often Help

When they match the content, these often improve Xiaohongshu-native feel:

- emphasis strips
- quick labels
- numbered blocks
- summary chips
- warning markers
- short comparison zones
- highlighted takeaway boxes
- one strong accent phrase

These are useful because they make content feel immediately actionable.

Do not overuse them to the point of visual noise.

---

## Visual Devices To Avoid By Default

Avoid these unless the content truly requires them:

- dashboard panels
- fake software UI framing
- heavy table layouts
- dense spreadsheet structures
- full-slide presentation rhythm
- long checklist pages without hierarchy
- generic app mockup blocks
- purely decorative floating cards with little information value

---

## Cover Patterns

Common valid Xiaohongshu cover patterns:

### Big Hook Cover

- one large headline
- one supporting line
- one dominant visual cue
- one strong accent block

### Checklist Cover

- one promise headline
- one quick framing line
- one visible value cue like `收藏备用` or `新手先看`

### Warning / Myth Cover

- one problem-based headline
- one contrast phrase
- visually stronger tension than a body page

---

## Body Patterns

Common valid Xiaohongshu body patterns:

### Practical Note Card

- one title
- one explanation block
- one support block such as tips or examples

### Comparison Card

- one comparison question
- left-right or top-bottom contrast
- one conclusion zone

### Step Card

- one step title
- one action line
- one small caution or support note

### Framework Card

- one framework name
- one breakdown structure
- one takeaway block

---

## Ending Patterns

Common valid Xiaohongshu ending patterns:

### Final Principle Card

- one memorable principle
- one summary support line
- one light CTA

### Save Reminder Card

- one recap headline
- one reason to keep the card
- one clear CTA

### Summary Checklist Card

- one wrap-up title
- three to five short memory points
- one closing prompt

---

## Topic Adaptation

Xiaohongshu is not one single visual mood.

Adapt the card system by topic:

### Knowledge / Tutorial

- clearer structure
- stronger usefulness
- more save-worthy framing

### Lifestyle / Beauty / Daily Notes

- more emotional softness
- more aesthetic warmth
- still keep readability first

### Tech / Workflow / Tooling

- cleaner systems
- stronger logic blocks
- avoid turning into software screenshots

### Business / Growth / Product

- more confidence
- clearer hierarchy
- stronger cover promise
- do not drift into pitch deck style

---

## Production Rules

For Xiaohongshu delivery:

1. Produce vertical social cards, not a generic web document.
2. Produce one real cover card.
3. Produce one or more real body cards.
4. Produce one real ending card.
5. Ensure every exported card can stand alone visually while still feeling
   part of the same series.
6. If using HTML fallback, design every card as a finished card, not as a
   block inside one long page.

---

## Review Gate

Before delivery, confirm all of the following:

- Does the cover feel like a hook?
- Does each body card carry one main point?
- Does the output feel like Xiaohongshu content instead of a dashboard or PPT?
- Is the Chinese text large enough?
- Is the card sequence save-worthy and practical?
- Does the ending card provide closure?

If the answer to any of these is no, revise before delivery.
