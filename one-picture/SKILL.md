---
name: one-picture
description: Create a single, technically accurate visual that gives an immediate mental model of a complex computer-science or AI topic. Use when the user asks for a one-picture explanation, visual overview, system map, architecture or flow diagram, memory layout, lifecycle, state machine, timeline, comparison, or concept relationship. Do not use for decorative illustrations, image-only artwork, or a comprehensive multi-page tutorial.
---

# One Picture

Compress one CS or AI topic into one visual whose main value is a correct, clear mental model. Optimize for structure and comprehension, not decoration.

## Establish the Model

Before drawing, identify the one sentence the viewer should understand after seeing the picture. Select only the relationships needed to support that sentence.

Determine which one or two questions matter most for the topic:

- Who participates, and who calls whom?
- How does data move?
- How does state change?
- What is the time order?
- What is contained in, above, or below what?
- How is input transformed into output?

Verify technical claims from the user's material, the workspace, authoritative sources, or direct inspection when needed. Distinguish established behavior from simplification or inference. Do not make a clean diagram at the cost of correctness.

If the topic is too broad, keep the first picture as the global map and reduce detail. Suggest follow-up pictures for important submodels only when useful; do not turn the first picture into a poster-sized encyclopedia.

## Choose the Visual Grammar

Choose the form from the dominant relationship, not from habit:

| Dominant relationship | Prefer |
| --- | --- |
| Transformation or branching steps | Flowchart |
| Ordered interactions between participants | Sequence diagram |
| Components, boundaries, and dependencies | Architecture diagram |
| Containment, abstraction, or ownership | Hierarchy diagram |
| Producers, stores, transformations, consumers | Data-flow diagram |
| Addresses, regions, references, and object placement | Memory-layout diagram |
| Creation, use, transition, and teardown | Lifecycle diagram |
| A small set of meaningful differences | Comparison diagram |
| Events and valid transitions | State machine |
| Change across time | Timeline |
| Definitions and typed semantic relationships | Concept-relationship diagram |

Do not default to a mind map. Combine visual grammars only when the secondary grammar makes the same mental model clearer rather than adding another model.

## Design the Picture

1. Define the visual boundary: what is inside the model, what is external, and what is intentionally omitted.
2. Choose a clear entry point and a consistent reading direction.
3. Lay out the primary path first. Add only the branches, feedback loops, stores, layers, or states needed to explain it.
4. Give nodes short, concrete labels. Put meaning on edges with verbs or data names when an unlabeled arrow would be ambiguous.
5. Encode different relationships differently. For example, do not use the same arrow style for data flow, control flow, ownership, and time unless the distinction is irrelevant.
6. Use grouping, alignment, whitespace, and restrained color to expose structure. Never rely on color alone; keep the picture understandable in monochrome.
7. Add a small legend only when the notation is not self-evident.

Prefer fewer meaningful elements over exhaustive detail. Avoid crossed edges, ornamental icons, unexplained acronyms, long prose inside nodes, tiny text, and false symmetry. When one diagram would need multiple unrelated reading directions or several independent legends, reduce scope or split the topic.

## Select the Output Technology

Choose the simplest format that reliably expresses and renders the model in the current environment:

- **Mermaid:** standard flows, sequences, state machines, timelines, and portable Markdown.
- **SVG:** precise custom layouts, memory diagrams, dense annotation, and a self-contained final visual.
- **HTML/CSS:** responsive or interactive explanation when interaction materially improves understanding.
- **Graphviz:** dependency-heavy graphs where automatic layout is valuable.
- **ASCII:** terminals, plain text, quick drafts, or environments without reliable rendering.
- **Other formats:** only when they better fit the relationship or the requested destination.

If the environment can render reliably, generate the final visual file and inspect the rendered result. Otherwise provide portable source and clearly state how it should be rendered. Fall back to a simpler technology when the preferred renderer is unavailable or produces an unreadable layout.

## Validate Before Delivering

Check the final picture at two levels:

- **Technical:** participants, arrows, order, states, boundaries, labels, and transformations are correct; simplifications do not reverse causality or erase a decisive condition.
- **Visual:** the entry point is obvious, the main path dominates, labels are legible, edge routing is traceable, groups are distinct, and the diagram works at the intended viewing size.

Inspect the actual render when one is produced, not just its source. Revise if the viewer must read the explanation before understanding where to start.

## Deliver

Lead with the picture. After it, provide only:

1. **Reading order** — a short instruction for traversing the visual.
2. **Key observations** — three to five concise points that reveal the model's most important relationships.
3. **Most common misunderstanding** — exactly one misconception and its correction.

Do not repeat the diagram as a long tutorial. Mention deliberate omissions only when they materially affect interpretation.
