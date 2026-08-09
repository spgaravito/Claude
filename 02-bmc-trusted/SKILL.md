---
name: aifc-bmc
description: Map how a business creates, delivers, and captures value across the nine blocks of the Business Model Canvas, and hand it back as an editable AIFC canvas the user controls — a first-draft model, not a finished verdict. AI drafts each block as a labeled starting point; the user owns every cell and the gaps between blocks are the point. Use when the user types "/aifc-bmc", is mapping or rethinking a business model, says "business model canvas," "BMC," "how does this business work," "map our model," "where does the money come from," or is pressure-testing a venture, product line, or pivot. From AIFueledCulture.
---

# AIFC — Draft the business model, hand over the controls

You are running a **Business Model Canvas** the AIFueledCulture way. The tool (lay a whole business model on one page across nine blocks — Customer Segments, Value Propositions, Channels, Customer Relationships, Revenue Streams, Key Resources, Key Activities, Key Partners, Cost Structure) is from **Alexander Osterwalder and Strategyzer**. What is AIFC is the **method on top**: AI does not declare your business model sound. It drafts a **first draft** — each block populated and labeled by confidence — and hands over the controls, because the model is the user's to redraw and the value is in seeing where the blocks don't yet line up.

## The discipline (non-negotiable)

This skill is part of the AIFueledCulture **Controllable Canvas** family, and the discipline below *is* the product — a Trusted AI Culture is built by holding it, so do not drift:

1. **A first draft, never a verdict.** Offer a starting point the user owns and edits; never present the output as the answer, and never pick for them.
2. **Confidence on its face.** Mark every item evidenced (●) or assumption (○) so the user sees where to apply judgment; when unsure, mark assumption.
3. **The user holds the controls.** The canvas is theirs to change; the human stays in the loop by design.
4. **It ends in a move.** Always route to a next action — never stop at a static picture.

Never narrate the framework as prose instead of building the canvas, never fabricate the user's facts, and keep attribution accurate. Full contract: `AIFC_Canvas_Family_Doctrine.md`.

## How to run it

**1. Interrogate before you map.** Pin down:
- **The business** — whose model is this: a whole company, one product line, or a proposed venture? Name it; a canvas for a fuzzy "the business" is weak.
- **The purpose** — are we mapping the model as-is, or testing a change (a pivot, a new segment, a new revenue model)? That sets where to look hardest.

**2. Draft the nine blocks.** Start from the customer side and work in:
- **Customer Segments** — who you create value for.
- **Value Propositions** — the value that makes them choose you.
- **Channels** — how you reach and deliver to them.
- **Customer Relationships** — how you get, keep, and grow them.
- **Revenue Streams** — how the value turns into money.
- **Key Resources** — the assets the model needs.
- **Key Activities** — the things you must do well.
- **Key Partners** — who you rely on outside the business.
- **Cost Structure** — what running the model costs.

2–3 specific items per block, drawn from the real business — not textbook placeholders.

**3. Label every item by confidence.** Mark **evidenced** (grounded in what the user told you, or on the record) or **assumption** (your inference — check it). Revenue streams and customer relationships are where an outside AI guesses most; be candid and mark those as assumptions to validate.

**4. Render it as the canvas, not as prose.** Build the dashboard from `assets/aifc-canvas-engine.html` with `layout:"bmc"`, `family:"BUSINESS MODEL CANVAS"`, and a `bmc` object with the nine blocks (`partners`, `activities`, `resources`, `value`, `relationships`, `channels`, `segments`, `costs`, `revenue` — each `{items:[{text,evidenced}]}`). The rendered canvas is the classic nine-block grid, every cell editable. Save it as a standalone `.html` the user can open, redraw, and print.

**5. Hand over the next move:**
- **Find the gaps and mismatches** — a value proposition no channel delivers, a segment with no revenue stream, a cost with no matching activity. The misalignments between blocks are the real output.
- **Pressure-test the riskiest block** — usually Revenue Streams or the core Value Proposition; flag the assumptions to validate first.
- **Zoom into the offer** (hand to `/aifc-vpc`) to detail the fit between a segment and its value proposition.
- **Size up the position** (hand to `/aifc-swot` or `/aifc-porter`), or **stress-test the model** via `/aifc-mirror`.

## Producing the canvas

Take the engine file verbatim and replace **only** the `CANVAS_DATA = {…}` object; output the **entire** file otherwise unchanged, named `aifc-bmc-<subject-slug>.html`. If the environment has no filesystem to save to, output the complete HTML in a code block for the user to keep. Do **not** also narrate the framework as prose in chat — the canvas is the deliverable; a one-line framing note is enough. And if the user won't be drawn into the interrogation, draft from what they gave you and mark nearly everything **assumption (○)**, so the gaps stay visible.

## Rules

- Interrogate the business and the purpose first. One business model per canvas — not a market, not a product feature.
- Specific items over textbook block-labels; work from the real business; never fabricate its facts.
- The value is in the gaps between blocks — surface mismatches; never declare the model "validated."
- Label confidence accurately — revenue and relationships are usually assumptions until tested — and keep every cell the user's to redraw.

## Attribution

The Business Model Canvas is from **Alexander Osterwalder and Strategyzer**, shared under a **Creative Commons Attribution-ShareAlike (CC BY-SA)** license — **not** an AIFueledCulture invention, and **not** to be credited to Dr. Jules White. Attribute Strategyzer wherever the canvas is published. What AIFueledCulture adds is the method around it: a confidence-labeled first draft the user controls.

*AIFueledCulture — build a Trusted AI Culture: the Frameworks, Best Practices, and Internal Champions to work with AI intentionally. aifueledculture.com*
