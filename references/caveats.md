# Conditional caveat checks

Select relevant rows. This is an original operational synthesis of linked guides, with added safeguards explicitly labeled; not a reproduced flashcard collection.

## Scale and encoding

| Condition | Check / response | Source |
| --- | --- | --- |
| Bars/filled areas encode magnitude | Use meaningful zero; place negatives properly. A narrower line/dot range can be valid if explicit and proportionate | [Baselines](https://www.data-to-viz.com/caveat/cut_y_axis.html) |
| Two measures share a plot | Independent axes can manufacture alignment; prefer panels or an explicit index. Exact unit-conversion axes are a different case | [Dual-axis example](https://www.data-to-viz.com/caveat/dual_axis.html); alternatives are extensions |
| Shapes encode size | Scale area, not radius: circle radius follows square root of value. Verify library size semantics and clipping | [Area/radius](https://www.data-to-viz.com/caveat/radius_or_area.html) |
| Stacks | Verify additive components/denominator. For individual changes use aligned lines, panels, or grouped bars | [Stacking](https://www.data-to-viz.com/caveat/stacking.html) |
| Pies/donuts/radial comparisons | Check complete nonnegative whole and readable labels; use bars for close/many-group comparison | [Pie guide](https://www.data-to-viz.com/caveat/pie.html); conditional use is an extension |
| Transformed/log axes | State transform/units; never silently discard zero/negative values. Log distances do not express absolute differences | Extension |

## Hidden information

| Condition | Check / response | Source |
| --- | --- | --- |
| Histogram/density | Try nearby reasonable bins/bandwidths before claiming peaks or thresholds; disclose consequential smoothing/exclusions | [Bins](https://www.data-to-viz.com/caveat/bin_size.html), [density](https://www.data-to-viz.com/story/OneNum.html) |
| Group summaries/boxplots | Inspect n, skew, outliers, multimodality; add points for small samples or distribution views | [Boxplot pitfalls](https://www.data-to-viz.com/caveat/boxplot.html) |
| Error bars/bands | Identify SD, SE, CI, credible interval, or range with level/method. Observation spread differs from estimate precision. Raw points alone do not replace inferential intervals | [Error bars](https://www.data-to-viz.com/caveat/error_bar.html); inferential clarification is an extension |
| Dense points | Check overlap before asserting absent structure; try size, opacity, bins, density, facets. Disclose sampling; jitter does not change measured values | [Overplotting](https://www.data-to-viz.com/caveat/overplotting.html) |
| Many lines | Focus + context, labels, or facets. Shared scales compare levels; disclose free scales used for shape | [Spaghetti plots](https://www.data-to-viz.com/caveat/spaghetti.html) |
| Repeated/paired values | Preserve entity IDs/pairing; do not treat repeats as independent or connect unrelated records | Extension |
| Aggregate trends support a strong claim | Check relevant subgroup/population changes; distinguish pooled rates from unweighted averages and association from causation | [Index: Simpson's paradox](https://www.data-to-viz.com/caveats.html); weighting checks are extensions |

## Maps and reading

| Condition | Check / response | Source |
| --- | --- | --- |
| Polygon color | Large regions dominate. Use relevant rates for intensity, symbols for counts when appropriate. Inspect joins, small regions, missingness | [Choropleth bias](https://www.data-to-viz.com/graph/choropleth.html) |
| Color | Discrete hues for categories; ordered palette for quantities; diverging scale around a meaningful midpoint. Stable entity colors and non-color cues | [Index: color/dashboard sections](https://www.data-to-viz.com/caveats.html) |
| Labels | Units, source, annotations near evidence; horizontal labels where practical. Avoid collisions/false precision; essential information must survive export | [Index: labels](https://www.data-to-viz.com/caveats.html) |
| Ranking | Preserve natural order or sort by meaningful metric. Explain top-N exclusions/remainder when the whole matters | [Ordering](https://www.data-to-viz.com/caveat/order_data.html) |

## Additional implementation safeguards

- Preserve meaningful distinctions among observed zero, unknown, unavailable, not applicable, and filtered out. Do not impute to draw continuity. A single-observation series needs a marker or explicit text.
- Calculate ratios from matched numerators/denominators when appropriate; do not average subgroup rates without a justified estimand. Keep percent change separate from percentage points.
- Preserve actual date spacing. Disclose rebasing, currency/inflation adjustment, normalization, and smoothing windows when material.
- Align panel units, scales, and order for comparisons. Filter-induced axis changes must not silently appear as data changes.
- Titles must match evidence; avoid causal claims for descriptive plots or accounting bridges.
- Reject or visibly explain values incompatible with an encoding; do not quietly force negatives into part-to-whole areas.

## Source limits

Reviewed 2026-11-04. Some pages are incomplete/inconsistent: `caveat/rainbow.html` currently contains unrelated single-variable content; the dual-axis guide is primarily demonstration code. Use the caveat index and sound encoding reasoning for these topics; a slug is not evidence. This skill qualifies the error-bar article's broad avoidance recommendation to preserve valid inferential uncertainty. Check example code against current libraries and data semantics before reuse.
