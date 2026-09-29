---
name: check-visual
description: Verify a UI change against its reference (Figma node, reference image, screenshot, or live site) before reporting it done. Use after any visual fix or build in a prototype, deck, or website, whenever the user asks "is it fixed", "does it match", or shares a reference, and before saying "done" on any visual work.
---

# Check visual

Never report a visual change as done from the code alone. The build passing doesn't mean it looks right.

## 1. Get the reference first
- Figma: screenshot the exact node (Figma MCP `get_screenshot`). Note its frame width.
- Image or screenshot from the user: use it as given. Ask for one if there's nothing to compare against.
- Live site or "production": open it in the browser at the same viewport.

## 2. Capture the result the same way
- Same viewport width as the reference. Same state (hover, open, scrolled position, slide number).
- Full resolution. For small details (icons, arrows, spacing, captions), zoom into that region.
- Look at the whole screen, not only the element you changed. Check for new breakage nearby.

## 3. Compare and list the differences
Write concrete deltas, not impressions:
- "Caption gap is 16px, reference is 24px"
- "Close icon 20px, options icon 16px, reference has both at 20px"
- "Arrow tip stops 6px short of the card edge"

If there are no differences, say what you compared ("slides 12–15 at 1440px against Figma frames").

## 4. Fix, then check again
Fix the listed deltas, then repeat steps 2–3. Only report when the list is empty.

## Two strikes
If the same element is still wrong after two attempts, stop changing it. Switch approach:
- Icons, arrows, connectors, illustrations: export them from Figma as SVG. Don't redraw them.
- Textures or images: ask the user for the source asset.
- Otherwise: tell the user what you tried and ask.

## Don't waste turns
Verify once, carefully, rather than in a loop of quick guesses. One full-resolution comparison beats five glances.

## Report format
- What changed
- What you compared, and at which viewport
- Remaining differences (if any)
- What you did NOT check (other breakpoints, states, browsers)
