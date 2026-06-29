# Quality Check

## Purpose

This file defines the final review system for `content-card-maker`.

It is used after the card package is assembled and before the final
result is returned.

The goal is not only to check wording, but to verify that the content
package is visually coherent, platform-native, mobile-readable, and
ready for production.

If the user asked for a visual package, the review should assume the work
is incomplete until an actual deliverable exists as images or rendered
exports.

---

## Review Rule

Run this check after:

1. Visual strategy is chosen.
2. Card plan is drafted.
3. Card structure is drafted.
4. Image prompts are written.
5. Caption and hashtags are prepared.

---

## Pass Standard

The package passes only when:

- The visual system is internally consistent.
- The structure fits the selected platform.
- The card plan is narratively sound.
- The cover is strong enough to stop or attract attention.
- The content is readable on mobile.
- The CTA matches the platform and the user goal.
- The prompts are complete enough to generate a coherent series.
- Actual deliverables have been generated, or a browser-rendered fallback
  export has been created.

---

## Review Dimensions

### 1. Visual Consistency

Check:

- Does the selected style preset remain stable across all cards?
- Do background, color, typography, and illustration directions belong to the same system?
- Does the ending card still feel like part of the same series?
- If a preview sample was shown earlier, do the final cards remain close to
  that sample in overall quality and aesthetic direction?

Fail Signals:

- Cover and content cards feel like different brands.
- One page becomes overly decorative while others are minimal.
- Typography direction changes without reason.
- The preview sample feels premium, but the delivered cards feel like a
  different and weaker production system.

### 2. Platform Consistency

Check:

- Does the structure match the selected platform behavior?
- Is the page count appropriate for the platform?
- Does the pacing fit how users consume content there?

Fail Signals:

- Douyin output feels like a slow article.
- Xiaohongshu output lacks save-worthy practicality.
- WeChat Feed output is too shallow or too noisy.

### 3. Title Quality

Check:

- Is the cover title clear, specific, and useful?
- Does it communicate benefit, outcome, or a strong hook?
- Is it short enough for mobile scanning?

Fail Signals:

- Title is vague.
- Title sounds generic or templated.
- Title is too long to land at a glance.

### 4. Card Planning Quality

Check:

- Does each page have one main point?
- Does the cover have a clear hook?
- Is the content order logical?
- Is there a summary page or ending CTA when needed?
- Is each page sized appropriately for phone reading?

Fail Signals:

- Multiple equal-weight points are forced onto one page.
- The cover lacks a concrete reason to continue.
- The sequence feels random or repetitive.
- There is no closure at the end.
- Several pages are too dense for a phone screen.

### 5. Image Readability

Check:

- Can the text be read comfortably on a phone?
- Does each card contain one main idea?
- Is information chunked clearly enough for quick scanning?

Fail Signals:

- Tiny text.
- Dense paragraphs inside a card.
- Too many visual elements fighting for attention.

### 6. Mobile Reading Experience

Check:

- Is the hierarchy obvious without zooming?
- Are lines, modules, and section breaks clear?
- Does the sequence feel smooth from card to card?

Fail Signals:

- Weak hierarchy.
- Cards require effort to understand.
- The reading path feels confusing or inconsistent.

### 7. Cover Attractiveness

Check:

- Does the cover communicate one strong promise?
- Is the focal point obvious within one glance?
- Does the cover fit the platform's attention pattern?

Fail Signals:

- Cover feels flat or informational only.
- No immediate reason to tap, save, or read.
- Title and visuals compete instead of reinforcing each other.

### 8. Ending CTA

Check:

- Does the ending card invite a natural next action?
- Does the CTA match the platform and content goal?
- Is the CTA aligned with the tone of the series?

Fail Signals:

- No CTA.
- CTA is hard-sell and breaks trust.
- CTA asks for the wrong action for the platform.

### 9. Prompt Quality

Check:

- Is there a clear global art direction?
- Do all page prompts inherit the same series style?
- Does each page have differentiated composition?
- Are text zones and visual hierarchy clearly instructed?
- Is there a negative prompt on every page?

Fail Signals:

- Prompt set has no unified series identity.
- Every page uses nearly the same composition.
- Text placement and hierarchy are vague.
- Negative prompt is missing.

### 10. Prompt Completeness

Check:

- Is there a global art direction?
- Does every card have a prompt or equivalent visual instruction?
- Do the prompts include subject, composition, style, and readability intent?

Fail Signals:

- Prompts are too generic.
- Card-specific visual differences are missing.
- Prompt language does not preserve series consistency.

### 11. Delivery Completeness

Check:

- Was a real asset package produced?
- If an image tool was available, were final images generated?
- If no image tool was available, was an HTML page rendered and exported to PNG?
- Does the final reply prioritize the deliverable over internal analysis?

Fail Signals:

- Only analysis or planning text was returned.
- Only prompts were returned even though production was possible.
- No final asset links or files were surfaced to the user.
- The reply is dominated by process explanation instead of deliverables.

### 12. Sample-to-Output Consistency

Check:

- If a style sample or preview image was shown, does the final set match it
  closely enough in polish, palette, hierarchy, and mood?
- Does the final output feel like a full expansion of the same sample
  rather than a different fallback style?
- Was the production path adjusted if the current rendering method could
  not preserve the sample quality?

Fail Signals:

- The sample and the final cards look like two unrelated systems.
- The sample has much stronger finish quality than the actual deliverable.
- The fallback method visibly degrades the promised style without warning.

---

## Final Review Output Format

Use the following structure inside the `Quality Review` section defined by
`OUTPUT_FORMAT.md`:

- Visual Consistency: Pass / Revise
- Platform Fit: Pass / Revise
- Card Planning Quality: Pass / Revise
- Title Quality: Pass / Revise
- Readability: Pass / Revise
- Mobile Experience: Pass / Revise
- Cover Strength: Pass / Revise
- CTA Strength: Pass / Revise
- Prompt Quality: Pass / Revise
- Prompt Completeness: Pass / Revise
- Delivery Completeness: Pass / Revise
- Sample-to-Output Consistency: Pass / Revise
- Final Risk Notes: brief note on remaining weakness or `None`

---

## Revision Rule

If two or more dimensions return `Revise`, the package should be improved
before delivery.

If only one dimension returns `Revise`, revise that part and keep the rest
of the structure stable.
