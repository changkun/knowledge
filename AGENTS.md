# AGENTS.md

This file explains how to work on the `knowledge/` corpus.

## What This Corpus Is

- This is not a resume.
- This is not a blog index.
- This is not a neutral archive of everything ever written.
- This is a curated knowledge map: long-term domains, methods, problem consciousness, and the life/professional contexts that made them stable.

The target reading experience is:

- a clear overall map
- strong continuity between pages
- one narrative voice
- stable boundaries between major domains

## Reference Sources

- `knowledge/` is the source of truth for the corpus itself.
- When integrating research material, use the public research record as the main anchor:
  - research overview and publication list
  - theses
  - public talks / defenses
- Unpublished research plans or synthesis drafts can be used to identify where recent questions are moving, but they should be written as frontier directions or active lines of thought, not as settled results.

## Structural Logic

`README.md` defines the top-level map. It currently uses four layers:

1. Foundation layer
   Files:
   - `math-and-learning.md`
   - `systems-and-engineering.md`
   - `languages-platforms-and-products.md`

   Purpose:
   - Explain the deepest recurring habits: formalization, mechanism-first thinking, system building, language/platform/product judgment.

2. Research layer
   Files:
   - `doctoral-training-and-research-formation.md`
   - `human-systems.md`

   Purpose:
   - Show where the foundational tendencies become formal research training, empirical research programs, and the core human-in-the-loop problem space.

3. Output layer
   Files:
   - `teaching-and-course-design.md`
   - `open-source-and-public-output.md`
   - `writing-and-culture.md`

   Purpose:
   - Show how knowledge is reorganized outward into courses, OSS, public infrastructure, papers, talks, and writing.

4. Background layer
   Files:
   - `cross-cultural-life-and-media.md`
   - `long-tail-and-writing.md`

   Purpose:
   - Preserve the life world, edge zones, and non-core materials that shaped the main line without forcing them into the core.

## Page Responsibilities

Use these boundaries when editing:

- `math-and-learning.md`
  Focus on formalization, proof structure, learning theory, and mathematical modeling.

- `systems-and-engineering.md`
  Focus on runtime, OS, performance, deployment, infra, production systems.

- `languages-platforms-and-products.md`
  Focus on language design, platforms, product feel, interaction packaging, delivery.

- `doctoral-training-and-research-formation.md`
  Focus on doctoral formation, formal research training, research method, and the major empirical research clusters; graphics/geometry may appear as an important case domain, but not as the sole center.

- `human-systems.md`
  Focus on HCI, HITL, behavior modeling, adaptive systems, crowds, AI governance, preference, responsibility chains, and social systems.

- `teaching-and-course-design.md`
  Focus on pedagogy, course structuring, supervision, academic training, evaluation philosophy.

- `open-source-and-public-output.md`
  Focus on OSS, talks, community roles, public technical infrastructure, translation as public work.

- `writing-and-culture.md`
  Focus on writing method, reading structure, research taste, intellectual style, worldview.

- `cross-cultural-life-and-media.md`
  Focus on migration, multilingual life, German context, travel, media/cultural intake as lived background.

- `long-tail-and-writing.md`
  Focus on unstable, peripheral, exploratory, temporary, literary, and uncollapsed materials.

## Writing Rules

Maintain these rules unless there is a deliberate reorganization:

- Write as if the corpus was conceived as one work.
- Do not annotate the prose with source-layer commentary like:
  - “履历补出……”
  - “博客里没有，但简历里有……”
  - “这里再补一个正式坐标……”
- Instead, integrate formal education/work/teaching/OSS facts directly into the topic narrative.
- Prefer synthesized judgments over evidence dumping.
- Keep public references public:
  - use public links when citing published material
  - for unpublished drafts, keep only titles, not local file paths
- Treat research plans carefully:
  - use them to sharpen current direction
  - do not present them as already-finished publication records
- Avoid turning pages into CV bullet lists.
- Avoid turning pages into taxonomies with no temporal movement.
- Preserve temporal development when useful: early formation -> formalization -> institutionalization -> production reality.

## How To Modify

When editing content, decide first which kind of change it is:

1. Clarification
   - wording cleanup
   - smoothing transitions
   - improving consistency

2. Boundary correction
   - moving material from one page to another
   - removing duplicated ideas
   - making page responsibilities sharper

3. Structural change
   - changing the four-layer model
   - adding/removing top-level pages
   - redefining page responsibilities
   - changing how the corpus should be read

If the change is structural, update all of:

- `README.md`
- affected page intros
- this `AGENTS.md`

## Editing Checklist

Before finishing, verify:

- Does the edited page still fit its assigned layer?
- Does it overlap too much with a neighboring page?
- Does it still sound like the same corpus as the others?
- Did you accidentally reintroduce source-commentary language?
- If you changed organization logic, did you update `AGENTS.md` too?

## Permission To Edit This File

If the knowledge organization logic changes, you should update this file in the same change.

Do not treat `AGENTS.md` as immutable documentation. It is part of the corpus-maintenance contract and may need to evolve with the structure.
