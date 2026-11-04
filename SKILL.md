---
name: data-to-viz
description: "Use for charts and data visualization in reports, slides, dashboards, spreadsheets, infographics, and maps. Choose, create, revise, or critique quantitative visuals using Data to Viz's decision tree and caveats, alongside the requested rendering tool. Excludes decorative imagery, pure conceptual diagrams, and tasks that only mention charts."
---

# Data to Viz

Use this as the chart reasoning and quality layer whenever data visualization is part of the task. Start from the reader's question, inspect the actual data structure, choose an encoding, create the requested artifact, and check what it might conceal or distort. Scale the work to the request: an ordinary bar chart does not need a design ceremony.

Adapted from [From Data to Viz](https://www.data-to-viz.com/) by Yan Holtz and Conor Healy. Local references are an original operational synthesis, not a verbatim poster reproduction or an official exhaustive implementation. Creation, tool routing, and verification guidance extends the source method.

## Select the mode

- **Choose / explain:** recommend a chart, the relationship it makes legible, and its decisive tradeoff. Create an artifact only when requested or necessary to answer.
- **Create / revise:** complete preparation, rendering, inspection, and delivery in the requested format. Code alone does not complete a request for a usable chart.
- **Review:** inspect the rendered chart and underlying data when available; prioritize misleading conclusions, hidden evidence, then readability. With a screenshot alone, separate visible findings from unverified data concerns.

## 1. Establish the question and data contract

Infer reasonable defaults from the task and project. Ask only when an unknown could materially change the chart or interpretation. Determine:

- The relationship: distribution, ranking, association, change, composition, hierarchy, flow, or geography.
- Exploration versus explanation; audience, destination, dimensions, interaction, export, and editability.
- Row grain, variable roles and units, group cardinality, raw observations versus aggregates, pairing/repeated measures, and nested versus crossed categories.
- Source/date, coverage, denominators, missing versus zero, duplicates, and necessary filtering/aggregation. Inspect actual values when accessible; names alone are insufficient.

For examples, use visibly labeled illustrative data. Never fabricate observations, intervals, or sources to fill a real-data gap. Continue independent useful work while a necessary input is missing.

## 2. Traverse data shape, then choose by purpose

Read [the decision tree](references/decision-tree.md) when choosing or materially changing a chart. Use the matching branch. Record the branch and reasoning briefly in working notes; expose only what helps the user.

Structure determines feasible candidates; purpose, semantics, and reading burden determine the choice. A numeric year can be time, coordinates are spatial, and a numeric ID is usually categorical. Do not choose merely by counting columns.

For a nontrivial choice, compare a primary option with one credible alternative using the same data and scope. Render both when it resolves uncertainty, not as a compulsory deliverable. Prefer aligned positions for precise comparison; justify area, angle, radial, or 3D encodings by their analytical purpose.

Honor a suitable explicit user choice with relevant caveats. If an encoding cannot truthfully represent the data, explain the specific problem and offer an alternative. A table or single value can be the best result.

## 3. Create through the appropriate delivery tool

Read [creation and verification](references/create-and-verify.md) for implementation or substantial revisions. Honor the requested tool, stack, format, and destination; otherwise choose the lightest available implementation that meets the need.

When installed visualization skills overlap, read [desktop routing](references/desktop-routing.md) before choosing the presentation owner. A filter on existing observations remains a standard chart; a control that changes assumptions and recalculates modeled outcomes belongs to an interactive tool. Choose one presentation workflow for the artifact rather than combining competing renderers, checkers, or wrappers.

Coordinate with installed capabilities:

- Data chart components own supported standard quantitative charts and their ordinary filters where applicable; load their current family and delivery instructions.
- Visualize owns an in-conversation calculator or interactive explainer as a whole, including any chart inside it. This skill still checks encoding, calculations, and caveats.
- Web visualization skills own browser implementation, responsive interaction, and performance when needed.
- Spreadsheet and presentation skills own native workbook/deck artifacts and requested editability.
- Standard plotting tools suit scientific figures and standalone exports; format skills own document/PDF packaging.
- Storytelling skills can own the argument and page sequence; this skill checks whether charts support their claims.

Discover actual installed skills/tools. Do not hardcode plugin version paths or assume a capability exists. If unavailable, state the limit and use an authorized suitable fallback. Do not turn a static chart into a dashboard or require publication, a paid service, installation, or a new framework just to draw it.

## 4. Apply relevant caveats

Read [caveats](references/caveats.md), selecting relevant rows. Before delivery check:

- **Meaning:** correct metric, population, period, unit, denominator, aggregation, and strength of claim. Correlation and arithmetic contribution do not establish causation.
- **Encoding:** faithful position, length, area, scale, date spacing, and comparisons; missing remains distinct from zero.
- **Information loss:** hidden distribution, sample size, uncertainty, subgroup reversals, overlap, or misleading smoothing/binning.
- **Reading:** visible units, labels, source, and material limitations; accessible encodings; legibility at the destination.

Apply conditional checks rather than blanket bans. Keep uncertainty intervals when estimate precision is the question; raw observations answer a different question. Novelty alone does not disqualify a chart, and attractiveness does not establish suitability.

## 5. Verify and deliver

Independently reconcile decisive displayed values with the source or reviewed transformation. Inspect actual marks at intended size. Exercise authored controls and meaningful missing/empty states where relevant. Inspect the saved/exported result when it is the deliverable.

Use documented renderer guarantees where applicable, keeping numerical verification separate. If visual or interaction inspection is unavailable, report the specific unchecked part; file existence and source inspection do not prove rendering.

Deliver the requested chart/artifact, concise choice rationale, material caveat, and actual verification status. Include reproducible code/specification when requested or useful for reuse, without unnecessary packaging. Never infer audience comprehension or business effect from a rendering check.

## Maintenance

Source review date: 2026-11-04. Local guidance supports offline use. Open relevant primary sources for unusual branches, conflicting guidance, or changing implementation details; do not recrawl the website for every chart. Use current renderer documentation for APIs. Improve from demonstrated failures rather than accumulating speculative rules.
