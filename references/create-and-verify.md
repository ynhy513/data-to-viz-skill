# Create and verify

An operational extension of Data to Viz. Use only what the artifact needs.

## Compact chart contract

For nontrivial work record in existing notes/code, not a mandatory separate file:

```text
Question / audience / exploration or explanation:
Source / scope / date / row grain:
Metric / units / denominator / variable roles:
Decision branch / chart / credible alternative:
Encoding / ordering / scale / transformations / exclusions:
Material caveats / uncertainty:
Destination / dimensions / interaction / export / editability:
Numerical and rendered checks:
```

Use a finding title only after examining evidence. An exploratory chart can use a descriptive title.

## Prepare

- Inspect samples, relevant totals/ranges, distinct entities, missing counts, and duplicate keys at the intended grain.
- Define aggregation. Averages of averages, duplicated joins, unmatched periods, and unweighted rates can yield convincing wrong charts.
- Keep transformations reproducible in code, formulas, or native configuration; avoid manually transcribing many values into marks.
- Reconcile selected groups and totals where composition/filters/top-N matter. Record material exclusions.
- Preserve supplied uncertainty. Calculate new intervals only with an appropriate method and supported sampling assumptions.
- Label synthetic/scenario data visibly in the artifact.

## Construct

Honor requested surface/format/editability and existing stack. Load the available delivery skill; it owns current APIs, components, packaging, and runtime-specific checks. Supply reviewed data, encodings, and caveats.

When unspecified, use established plotting for scientific/export figures, installed Data components for native inline standard charts, the project chart library for browser work, and native workbook/deck charts when editability matters. A custom encoding can justify specialized drawing. A standard chart rarely justifies a new framework.

Never use image generation for measured chart marks. A generated concept image cannot establish numerical fidelity.

Put the main relationship on strong channels, usually x/y position. Assign color/area supporting roles. Show scope, units, references, and material caveats. Use restrained emphasis, stable entity colors, non-color cues, and legible labels. Keep essential findings available without hover. For chart collections coordinate semantics/scales/order; separate overview/detail when one view becomes overloaded.

## Verify numerical meaning

Independently reconcile decisive values: leaders, exceptions, endpoints, totals, shares, denominators, missing counts, or transforms as relevant. Do not simply repeat the plotting code's assumptions.

Useful invariants, only when applicable:

- Waterfall endpoint = opening + signed contributions + disclosed residual.
- Complete shares sum to 100% within rounding tolerance and use the intended denominator.
- Bubble area ratios track value ratios.
- Missing periods show gaps or a disclosed treatment rather than observed zeros.
- Joins preserve expected key cardinality; paired IDs match the intended conditions.

Use checks capable of catching a material error, not a broad suite for a simple chart.

## Inspect actual output

Inspect rendered marks at intended size: bounds, clipping, labels, glyphs, source/caveat notes, color readability, and panel scale/order. A nonempty container or successful save alone is insufficient.

For authored interaction, exercise each distinct behavior where practical, including meaningful filter combinations and empty/missing state. Confirm marks/readouts/labels/caveats update together. Check narrow-screen behavior only when it is an intended delivery state; fixed print figures do not need mobile QA.

Follow documented standard-renderer guarantees where applicable instead of adding redundant checks; numerical checks remain separate. Inspect the exported result when it is the deliverable.

Distinguish **generated**, **numerically/render checked**, and **tested with actual audiences**. A render pass does not establish comprehension or business effect. Report the specific unavailable check when necessary.

## Deliver

Return the usable artifact on the requested surface with concise choice rationale, material caveat, and actual verification status. Include reproducible source/configuration when requested or useful for reuse. Do not package temporary QA or exploratory alternatives as deliverables without a purpose.
