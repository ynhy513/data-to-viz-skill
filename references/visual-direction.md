# Visual direction and design-pack mapping

Use this workflow when a project supplies visual evidence or the user wants a designed chart. First establish the chart's data, encodings, scale, comparisons and caveats. Use the design pass to shape how the reader encounters that evidence.

## 1. Read the reference and choose a visual direction

- Start with the supplied source. For a design pack with a machine-readable system, read `STYLE.md` together with `design-system.json` when both exist. Identify the pack version and selected family from `primary_family` and `families`. Use `patterns` to find page roles and their referenced rules. Read `rules` with the corresponding `evidence` pages, regions or object IDs. Resolve token values through `tokens` and their provenance through `token_rules`.
- For a single-page `style-pack.json`, use `style.heading`, `style.surface`, `style.layout`, `style.panel`, and `style.frame` as applicable. Read the corresponding rule and evidence entries. Respect the different field shapes and source units in the two formats.
- For a deck, screenshot, or gallery sample, record the visible page or region that supports each rule. Mark interpretations as inferred. With no usable source, apply an existing house style or choose a relevant gallery example and identify it as the reference.
- Use one coherent family. Pick the pattern whose reading role fits the chart, such as comparison, sequence, or detail. When no pattern fits, inspect rules with evidence in the chosen family even when no pattern references them. Build and label a chart-specific composition from the applicable rules. Skip rules tied to excluded families, imagery, or slide geometry with no corresponding chart role. Preserve meaningful style constraints and record any target-specific adjustment.

## 2. Turn visual choices into a render spec

Keep the spec in working notes or chart configuration. Add a separate artifact only if needed for handoff.

- **Reading order.** State the reader's task, the focal evidence and the reading sequence. For explanation, write a finding title supported by the chart. For exploration, label the task and specify the initial view. Put the chart in the primary visual area and size supporting modules according to their role.
- **Composition.** Allocate title, chart, direct annotations, details and source notes. Carry over alignment, grouping, figure-to-text hierarchy, whitespace and density from the reference where they support the task. Record how the layout folds for the actual destination. Keep independent units and scales explicit when chart modules align.
- **Visual roles.** Assign palette and typography to canvas, primary text, secondary text, data, context, benchmark and selection. Preserve the semantic meaning of data colors. Use a second cue where color alone would make a state or series hard to distinguish. Adapt deck-relative sizes to the target and test the actual glyphs, including CJK where relevant.
- **Annotation and interaction.** Specify which evidence gets a direct label, where precise readouts go, and what a selection updates. Use a stable entity key for linked marks, labels and details. For highlight-only controls, keep data positions, ordering and scales stable. For true filtering or scenario changes, specify which data or scales recompute and how the UI signals the change.
- **Provenance.** Record each material choice as source rule or reference region → chart component → acceptance check. Mark design choices introduced for the chart as adaptations. Map a few consequential rules before adding any decorative styling. Where the reference leaves the composition open, choose by reading task: a focal comparison can use paired annotations, a trend can anchor its turning point with a direct note, and a dense exploration can move detail into an aligned secondary panel.

Use the [public chart examples and design recipes](visual-references.md#按设计任务组合图样) when turning a general rule into specific marks, labels, or states. For each selected example, identify one technique to reuse and the conditions under which it serves the new chart. Use the reference's data and quantitative encoding only when they fit the reader's question.

Keep data positions, units, denominators, uncertainty, missingness and accessibility governed by the chart contract. Translate the purpose of a deck rule into the target renderer. If a renderer lacks a required slot or state, preserve the reading task with a supported alternative and record how the result differs. Keep the render spec portable across HTML, native slide charts and static output.

## 3. Inspect the render

- **Thumbnail.** Identify the first focal point from the actual image. Check that the most salient mark and headline lead to the same evidence. If a frame, panel, detail or control wins attention, change the relative size, weight or placement and render again.
- **Delivery size.** Inspect label collision, alignment, text/background contrast, line weight, type fallback, clipping, legend mapping and axis units. Test long labels or dense states relevant to the task. Check both the intended screen and the export when both are deliverables.
- **Interaction.** Exercise default and changed states. Check keyboard access and focus where supported, visible state, synchronized values and correct positional behavior. Inspect any state that adds a series, changes a scale or wraps the layout.
- **Data.** Reconcile the key values and verify the chart-specific encoding invariant independently. For example, confirm zero-based bar lengths, chronological spacing or bubble areas proportional to values.

For an aesthetic revision, compare before and after at the same size with the same data and selection. For a design-pack transfer, compare the applied rule against its source region and use a second chart or substantially different content when testing reuse. Record the observed result and any material gap between the intended and actual render.
