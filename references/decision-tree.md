# Chart selection by structure and purpose

A compact adaptation of Data to Viz's input-format method, not a node-for-node copy of its twenty-format poster. Task-first refinements and additional business-chart cases are operational extensions.

## Entry questions

1. Are locations or connections essential? Use D or E.
2. Is ordered time essential? Use C.
3. Are numeric observations ungrouped? Use A.
4. Are there categories, groups, paired measures, or a hierarchy? Use B.

Branches combine: time + region may call for faceted lines, not a map. Semantic roles override storage types; consider variables used in the question rather than every file column.

## A. Numeric variables

| Data shape / question | Candidates | Decisive consideration |
| --- | --- | --- |
| One numeric variable; distribution | Histogram, density; dots for small samples | Counts versus smoothed shape; inspect bins/bandwidth |
| Two numeric variables; association | Scatterplot | Overlap may require opacity, small marks, bins, or density; no causal inference from association alone |
| Two coordinates + numeric grid value | Heatmap, contours; surface for physical shape | A spatial field differs from three interchangeable measures |
| Three numeric variables; relationship with magnitude context | Bubble scatterplot; pairwise panels | Put the main relationship on x/y; area supports context rather than precision |
| Many measures; pairwise relationships | Scatterplot matrix or correlation heatmap | A selected correlation measure can conceal nonlinearity; inspect missingness |
| Many measures; profiles by entity | Parallel coordinates or heatmap | Units, standardization, axis order, and crowding can dominate patterns |

Sources: [one measure](https://www.data-to-viz.com/story/OneNum.html), [three measures / grid case](https://www.data-to-viz.com/story/ThreeNum.html), [chart-family index](https://www.data-to-viz.com/). Follow a family page for an unfamiliar encoding.

## B. Categories and numeric measures

First distinguish raw observations from summaries. Multiple rows may be repeated measurements or duplicate joins, not independent samples.

| Data shape / question | Candidates | Decisive consideration |
| --- | --- | --- |
| Categories alone; frequency | Count then bars/dots | Aggregation creates the measure; retain meaningful unknown categories |
| One value per category; ranking | Horizontal bars, dots, lollipops | Preserve natural ordinal order; otherwise sort meaningfully |
| Several observations per group; distributions | Box + points, violin, strip/beeswarm, density panels | Sample size, multimodality, spread, and outliers |
| Crossed group/subgroup; one aggregate per cell | Grouped bars, faceted dots, heatmap | Which comparison should be easiest? Crossed groups differ from nested hierarchy |
| Two matched conditions per entity | Dumbbell, slope, paired difference plot | Preserve pairing; slopes emphasize trajectories/rank, differences emphasize change |
| Several repeated conditions | Lines/parallel coordinates, small multiples | Retain entity identity; avoid connecting unordered nominal categories as a trend |
| Nested categories; numeric leaf values | Treemap, sunburst, circle packing; grouped bars for precise leaf ranking | Hierarchical containment versus precision; parent totals must be coherent |
| Hierarchy without numeric sizes | Tree; dendrogram for actual clustering | Computed trees depend on distance/linkage definitions |

Sources: [category + measure](https://www.data-to-viz.com/story/OneNumOneCat.html), [groups / two-period alternatives](https://www.data-to-viz.com/story/OneNumSevCatSubgroupOneObsPerGroup.html), [hierarchy](https://www.data-to-viz.com/story/SevCatOneNumNestedOneObsPerGroup.html).

### Composition filter

Part-to-whole charts require a coherent, non-overlapping whole and explicit denominator:

- Exact comparison: aligned bars/dots, optionally with share labels.
- Mix across groups: 100% stacked bars; separately show totals when group size matters.
- Nested mix: treemap/sunburst for structure; a flat ranking for exact values.
- Pie/donut: conditionally useful for a few clearly different nonnegative shares when rough recognition suffices. Close comparisons/multiple groups favor bars.
- Overlapping sets: a legible Venn or an intersection table/UpSet-style view, not a 100% partition.

Conditional pie use and set handling are this skill's judgment. The [source pie guide](https://www.data-to-viz.com/caveat/pie.html) takes a stronger position against pies.

## C. Time

| Data shape / question | Candidates | Decisive consideration |
| --- | --- | --- |
| Time + one measure; trend | Line; bars for discrete totals | Real intervals, gaps, units, reporting frequency |
| Time + groups; compare trends | Labeled lines, panels, focus + context | Shared scales for magnitude; disclose free scales for shape comparison |
| Time + additive components; total and mix | Stacked area/bars | Non-baseline components are difficult to compare precisely |
| Two dates across entities | Slope/dumbbell | Matched endpoint coverage; no invented intermediate path |
| Seasonality/periodicity | Calendar or period heatmap, seasonal panels | Use the actual calendar/business cycle; show missing periods |

The seasonal row is an extension. Sources: [stacking](https://www.data-to-viz.com/caveat/stacking.html), [many series](https://www.data-to-viz.com/caveat/spaghetti.html).

## D. Geography

Country names alone do not require a map. A ranking may answer the question better.

| Data shape / question | Candidates | Decisive consideration |
| --- | --- | --- |
| Point locations | Point map; spatial bins/density if crowded | Projection, coordinates, overlap, aggregation unit |
| Polygons + rate/intensity | Choropleth | Relevant denominator, classification breaks, missing regions |
| Locations + absolute counts | Proportional-symbol map | Symbol area represents size; polygon size is not population |
| Origin/destination + quantity | Flow map if geography matters; matrix/Sankey otherwise | Direction, crossings, totals, observed versus schematic routes |

Cartograms/hexbin maps change geographic reading while reducing some size/density problems. Added safeguards: preserve boundary provenance and distinguish disputed/illustrative geography where material. Do not present schematic routes as measured travel.

Sources: [map families](https://www.data-to-viz.com/graph/map.html), [choropleth size bias](https://www.data-to-viz.com/graph/choropleth.html).

## E. Connections, flows, matrices

Determine node identity, direction, weights, self-links, stages, and hierarchy.

| Structure / question | Candidates | Decisive consideration |
| --- | --- | --- |
| Dense pairwise ties | Matrix heatmap | Ordering/clustering; observed zero versus missing |
| Sparse graph; topology | Node-link network | Layout is algorithmic, not measured geographic distance |
| Staged quantitative transfers | Sankey/alluvial | Width matches quantity; account for losses and incomplete coverage |
| Exchange among manageable groups | Chord or matrix | Broad exchange overview versus precise pairwise lookup |
| Many edges with spatial/hierarchical structure | Arc diagram or edge bundling, conditionally | Overview can hide individual paths; retain inspectability |

Source: [network and migration examples](https://www.data-to-viz.com/story/AdjacencyMatrix.html). Conservation/missing-data checks are extensions.

## Additional business cases — extensions

| Question | Useful chart | Validity condition |
| --- | --- | --- |
| Arithmetic opening-to-closing change | Waterfall | Signed contributions reconcile, including residual; no unsupported causality |
| Ordered-stage conversion | Funnel or aligned bars | Matched population/window and explicit denominators |
| Actual versus target | Dot/bullet-style chart, reference marks | Same units/period; target distinct from observation |
| Estimate precision | Points + intervals; time ribbon | Known interval type, level, method; no fabricated bounds |
| A few exact values | Table or annotated value | No useful relationship gained from a chart |

Final question: what comparison becomes easy, and what becomes harder or disappears? If the hidden aspect could change the interpretation, expose it or change the encoding.
