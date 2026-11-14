# Data to Viz: 132 visual references

**English** · [简体中文](visual-references.zh-CN.md)

## How to use the library

1. Identify the reader's task, data units, denominator and output size before choosing the encoding.
2. Use the recipes below to find up to three examples. Open the original pages and pick one useful technique per reference.
3. Record the example ID, visible technique, target mark or state and rendered check. For example, use 121 for signed end labels and 129 for selection that preserves position.
4. Redraw with the target data and check quantitative accuracy, annotation placement and interaction. At slide size, keep the evidence needed to read the main finding.

Links point to publicly available work and examples. The notes describe ways to adapt their design. Follow source licensing when reusing assets or code.

## Design recipes by reader task

| Reader task | Examples | Design implementation | Check |
|---|---|---|---|
| Rank items and compare gaps | 003, 009, 121, 129 | Sort horizontal bars, label ends and highlight selection in place. | Verify a common zero, signed label placement and stable order. |
| Compare a pair of periods | 001, 122, 125 | Connect matched entities. Switch to one row per entity when lines crowd. | Check entity IDs, time labels and units for endpoints and differences. |
| Locate a turning point | 013, 020, 123 | Use a time axis with local annotations, gaps for missing values and a separate forecast style. | Check intervals, gaps and the first projected period. |
| Explain a change in totals | 021, 028, 124 | Anchor contributions with subtotals. Aggregate the remainder if only the largest categories are shown. | Reconcile both closing values and the categories grouped into Others. |
| Find clusters, tails or outliers | 031, 126, 128 | Put the distribution first. Add a subdued mean reference or an aligned marginal histogram. | Check bin boundaries and verify the median or tail values when discussing skew. |
| Compare relationships across groups | 012, 127, 128 | Repeat a small chart per group with shared axes and selective annotations. | Verify that equal values appear at equal relative positions and group counts are available. |
| Read a network, flow or map | 041, 051, 061 | Highlight connected paths, use proportional flow widths or choose the spatial property to preserve. | Verify node IDs, balanced flows, geographic boundaries and denominators. |
| Interpret uncertainty or scenarios | 103, 106, 132 | Match the interval, sample trajectories or scenario baseline to the decision. Label the actionable threshold. | State interval meaning or scenario assumptions and check scales across states. |
| Open details from an overview | 107, 109, 130, 131 | Keep an overview for orientation and a linked panel for records or zoom. Expose the selected range, total and reset. | Test default, empty, reset and keyboard states. Label the exported selection. |
| Fit a half-slide or phone | 009, 111, 113, 117–120 | Keep one focal finding and reflow annotations. Put secondary detail in a caption or appendix. | Check actual-size glyphs, units, wrapping and long labels. |
| Design an editorial chart | 071, 081, 091 | Give custom marks defined data roles and connect evidence or interactions to those marks. | Check that the main finding is visible without interaction and provide access to exact values and sources. |

## Browse by topic

- [Ranking and direct labels](#ranking-and-direct-labels)
- [Time, rhythm and turning points](#time-rhythm-and-turning-points)
- [Composition, contributions and shares](#composition-contributions-and-shares)
- [Distributions and outliers](#distributions-and-outliers)
- [Relationships and networks](#relationships-and-networks)
- [Flows and paths](#flows-and-paths)
- [Maps and spatial comparisons](#maps-and-spatial-comparisons)
- [Editorial storytelling and evidence](#editorial-storytelling-and-evidence)
- [Interaction and simulation](#interaction-and-simulation)
- [Data art and static composition](#data-art-and-static-composition)
- [Probability, forecasts and decision paths](#probability-forecasts-and-decision-paths)
- [Linked exploration](#linked-exploration)
- [Static and interactive delivery](#static-and-interactive-delivery)
- [Interpretation and correction](#interpretation-and-correction)
- [Chinese-language editorial examples](#chinese-language-editorial-examples)
- [Public examples with implementation](#public-examples-with-implementation)

## Ranking and direct labels

| ID | Public example | Design application and checks |
|---|---|---|
| 001 | [F12 Dumbbell Queue](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Dumbbell%20Queue) | Use countable beads for paired change. Label exact endpoints and the bead unit. In a slide, keep both dates and the signed change. |
| 002 | [F5 Tick Rows](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Tick%20Rows) | Place category names beside countable ticks on a horizontal scale. Show what each tick represents and keep the leading categories at slide size. |
| 003 | [G3 Chunky Bars](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Chunky%20Bars) | Use bold bars and direct value labels for a quick ranking. Keep the zero baseline and order in the slide crop. |
| 004 | [Irish Olympic Ranking · Redesign](https://www.datawrapper.de/blog/irish-times-chart-redesigned-olympics) | Place rank 1 at the top and use host cities as time anchors. Show the comparison population if participation changes. |
| 005 | [Side-by-side Election Results](https://www.datawrapper.de/blog/comparison-columns) | Align current and previous results in adjacent columns. Label share differences in percentage points and keep both totals visible. |
| 006 | [The 100 Tallest Buildings in the World](https://www.visualcinnamon.com/portfolio/skyscrapers/) | Use recognizable building silhouettes to set the subject. For precise height comparison, retain a common baseline and scale. Keep perspective from altering apparent size. |
| 007 | [Top 10 Nintendo Switch Games](https://www.visualcinnamon.com/portfolio/best-selling-nintendo-switch-games/) | Borrow game-themed shapes for the opening image. Let common-scale lengths carry sales comparisons. Keep the top three and their units on a slide. |
| 008 | [Ethical NBA Championships, Ranked](https://pudding.cool/2026/06/ethical-champions/) | Put the ranking criteria next to the lead entries. Keep the rule summary and disclose the dependence on the author's definition. |
| 009 | [Annotations in Bar and Dot Charts](https://www.datawrapper.de/blog/annotations-in-bar-charts) | Use a short leader to connect a note to a bar or dot. Keep its value in a crop and check that the highlighted observation supports the wording. |
| 010 | [Internet Adoption](https://ourworldindata.org/grapher/share-of-individuals-using-the-internet) | Use a common percentage axis and date across regions. Label the eligible population and distinguish access from usage frequency. |

## Time, rhythm and turning points

| ID | Public example | Design application and checks |
|---|---|---|
| 011 | [Show Your Stripes](https://showyourstripes.info/) | Compress a long series into ordered stripes. Keep the baseline, years and color scale. Add a line or labels when exact values matter. |
| 012 | [Small-multiple Line Charts](https://www.datawrapper.de/blog/small-multiple-line-charts) | Repeat small frames for group trends. Share the scale when readers need to compare levels and keep only the key panels in a slide. |
| 013 | [Direct Labels in Line Charts](https://www.datawrapper.de/blog/improved-line-chart-editing) | Place text near the corresponding line endpoint. Label priority series and inspect crossings or gaps in the underlying observations. |
| 014 | [Top 10 Baby Names](https://www.visualcinnamon.com/portfolio/babynames/) | Keep entity identity stable across a long ranking history. Label a few names and explain what leaving the displayed top ranks means. |
| 015 | [A Year in Flights](https://www.visualcinnamon.com/portfolio/a-year-in-flights/) | Use a calendar grid to make seasonality visible from a distance. On a slide, keep one quarter and a total. Explain what the texture represents. |
| 016 | [GitHub Commit History Timeline](https://www.visualcinnamon.com/portfolio/orca-github-commits/) | Start with a full timeline, then zoom into the selected period. Keep date bounds and distinguish events from the amount of work. |
| 017 | [Satellite Surge](https://www.visualcinnamon.com/portfolio/sciam-satellite-surge/) | Facet growth by comparable groups to reveal where change concentrates. Keep the fastest-growing group and context with comparable units. |
| 018 | [GenCoop · Swiss Solar Power](https://www.visualcinnamon.com/portfolio/swissgrid-gencoop/) | Give long-run capacity and seasonal output separate views. Keep one time scale per view and distinguish stock from flow. |
| 019 | [Life Expectancy](https://ourworldindata.org/grapher/life-expectancy) | Begin with a few benchmark regions on a long timeline. Let readers add peers and distinguish period life expectancy from observed lifetimes. |
| 020 | [Urban Population Share through 2050](https://ourworldindata.org/grapher/urban-population-share-2050) | Separate observed and projected segments with line style and a boundary year. Keep the scenario assumptions with the forecast. |

## Composition, contributions and shares

| ID | Public example | Design application and checks |
|---|---|---|
| 021 | [Waterfall Subtotals and Direct Labels](https://www.datawrapper.de/blog/waterfall-charts) | Anchor a waterfall with opening, subtotal and closing values. Label changes with signs and reconcile them to the closing total. |
| 022 | [F7 Stacked Rungs](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Stacked%20Rungs) | Use stack segments for contribution and crossbars for local readout. Match legend and stack order. Reserve common-baseline comparison for aligned segments. |
| 023 | [L14 Hundred Field](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Hundred%20Field) | Divide a complete share into countable units. Label the unit and denominator. Verify the categories form the whole. |
| 024 | [F4 Tick Donut](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Tick%20Donut) | Use ring ticks to make units explicit when there are few categories. Label leading shares and use aligned positions for close comparisons. |
| 025 | [Treemap Hierarchy](https://www.data-to-viz.com/graph/treemap.html) | Use area for weight and containment for hierarchy. Label parent groups and largest boxes. Use an aligned view for exact rank. |
| 026 | [Stacked Area Chart](https://www.data-to-viz.com/graph/stackedarea.html) | Let the outline show the total and put the priority component at the bottom. Read the thickness of interior bands against the stack. |
| 027 | [Global Primary Energy Sources](https://ourworldindata.org/grapher/global-primary-energy-by-source) | Use consistent source colors and chronological order for energy composition. Label whether the chart shows absolute quantities or shares. |
| 028 | [Energy Mix Across Countries](https://ourworldindata.org/energy-mix) | Compare regions under one measurement definition. Show absolute amounts and shares in distinct slots, with each denominator visible. |
| 029 | [Renewable Share of Electricity Generation](https://ourworldindata.org/grapher/electricity-mix?frequency=annual&metric=share_of_generation&source=renewables) | Pair share and volume only when readers need both. Keep the power-generation denominator visible and distinguish generation from capacity. |
| 030 | [The Billion Dollar Gram](https://informationisbeautiful.net/visualizations/the-billion-dollar-gram/) | Use square area for broad orders of magnitude and direct labels for close values. Verify area ratios and keep the largest comparisons in a crop. |

## Distributions and outliers

| ID | Public example | Design application and checks |
|---|---|---|
| 031 | [The Radius Gap](https://www.visualcinnamon.com/portfolio/radius-gap/) | Use density contours to show clusters and the gap between them. Test bandwidth sensitivity and keep representative observations where useful. |
| 032 | [The Baby Spike](https://www.visualcinnamon.com/portfolio/baby-spike/) | Preserve the local time spike and its neighboring baseline. Label the date or time and avoid generalizing from a spike to yearly totals. |
| 033 | [Ridgeline Distributions](https://www.data-to-viz.com/graph/ridgeline.html) | Stack densities against one horizontal scale. Show the overlap boundary and clarify that density height does not directly count records. |
| 034 | [Violin Plot Distributions](https://www.data-to-viz.com/graph/violin.html) | Add observations and sample size when groups are small. Label key quantiles and check whether smoothing creates apparent extra modes. |
| 035 | [2D Density Plot](https://www.data-to-viz.com/graph/density2d.html) | Use contours when points overlap extensively. Show selected raw points or disclose bandwidth. Treat contour boundaries as density levels. |
| 036 | [Matrix Heatmap](https://www.data-to-viz.com/graph/heatmap.html) | Keep equal cell sizes and explicit row order, color domain and missing style. Use one scale across directly comparable panels. |
| 037 | [Sizing Chaos](https://pudding.cool/2026/02/womens-sizing/) | Start with a representative person or median, then show subgroup ranges. Keep both the anchor and the distribution in a slide. |
| 038 | [The Birthday Effect](https://pudding.cool/2025/04/birthday-effect/) | Place the exceptional date beside its neighbors. Show absolute and relative differences when the baseline is small. |
| 039 | [A Love Story](https://pudding.cool/2026/06/love-story/) | Track the same participants across survey waves. State eligibility for the paired sample and how attrition limits interpretation. |
| 040 | [Berkeley Earth · 2024 Global Temperature](https://berkeleyearth.org/global-temperature-report-for-2024/) | Show a record year against a long trend with reference period and dataset. Label temperature anomaly rather than absolute temperature. |

## Relationships and networks

| ID | Public example | Design application and checks |
|---|---|---|
| 041 | [Royal Constellations](https://www.visualcinnamon.com/portfolio/royal-constellations/) | Keep the network visible as context and highlight one selected node, neighbors and connecting path. Explain the meaning of position and edge length. |
| 042 | [Searching for Birds](https://www.visualcinnamon.com/portfolio/searching-for-birds/) | Combine searchable entities, illustrations and stable data marks. Keep the legend with the active view and interpret search counts according to their source. |
| 043 | [Small World of Words](https://www.visualcinnamon.com/portfolio/small-world-of-words/) | Start semantic-network exploration from a searchable term. Show its neighbors and explain how language and sample affect associations. |
| 044 | [UNESCO Intangible Cultural Heritage](https://www.visualcinnamon.com/portfolio/intangible-cultural-heritage/) | Use separate views for distinct relationships. Share a stable entity key and label the connection type in each view. |
| 045 | [RéciTAC](https://www.visualcinnamon.com/portfolio/recitac/) | State the collaboration rule and unit of analysis before highlighting a team. Differentiate shared project membership from direct ties. |
| 046 | [GitHub Top Contributor Network](https://www.visualcinnamon.com/portfolio/orca-top-contributors/) | Let readers follow a contributor and related projects within a dense network. Keep the link definition and avoid treating centrality as quality. |
| 047 | [Kantar MotiveMix](https://www.visualcinnamon.com/portfolio/kantar-motivemix/) | Explain what similarity and geographic distance each encode. Keep the two dimensions and a few locations in a compact comparison. |
| 048 | [CO₂ Emissions and GDP Per Capita](https://ourworldindata.org/grapher/co2-emissions-vs-gdp) | Label both per-capita units and explain a log axis where used. Annotate an exception and limit conclusions to association. |
| 049 | [Best in Show](https://informationisbeautiful.net/visualizations/best-in-show-whats-the-top-data-dog/) | Define both evaluation dimensions and the scoring method. Keep examples that expose the trade-off and explain how scores combine preferences. |
| 050 | [Parallel Coordinates](https://www.data-to-viz.com/graph/parallel.html) | Highlight one record across a few axes. Show axis order, units, direction and normalization, which all shape the apparent relationships. |

## Flows and paths

| ID | Public example | Design application and checks |
|---|---|---|
| 051 | [OECD Global Plastics Outlook](https://www.visualcinnamon.com/portfolio/oecd-global-plastics-outlook/) | Align Sankey nodes and width scales across periods. Keep a key flow and totals and reconcile source and destination quantities. |
| 052 | [Bussed Out](https://www.visualcinnamon.com/portfolio/bussed-out/) | Use one documented route to introduce a larger migration flow. Show its role alongside the total and distinguish an illustrative person from representative evidence. |
| 053 | [Visualizing Millions of People on the Move](https://www.visualcinnamon.com/portfolio/urbanization/) | Label origins, destinations, period and direction. Distinguish net movement from the volume of two-way movement. |
| 054 | [Switching Between Phone Brands](https://www.visualcinnamon.com/portfolio/phone-brand-switching/) | Use paired movements for switching and retention. Label the diagonal and specify the source or destination denominator for each percentage. |
| 055 | [Preferential Polling](https://www.visualcinnamon.com/portfolio/swayable-preferential-polling/) | Show transfer in discrete rounds with a rule and total at each step. Keep an example round and describe the simulated ranking assumptions. |
| 056 | [The Words in the Lord of the Rings](https://www.visualcinnamon.com/portfolio/words-lord-of-the-rings/) | Highlight links for one character or scene first. State whether weights are spoken words and interpret importance separately. |
| 057 | [Sankey Diagram](https://www.data-to-viz.com/graph/sankey.html) | Use link width for quantity. Keep the main flow, units and inlet and outlet totals, then reconcile additions or losses. |
| 058 | [Chord Diagram](https://www.data-to-viz.com/graph/chord.html) | Use a chord overview with a manageable number of groups. Label direction and weight and use a matrix for exact lookup. |
| 059 | [A Day in the Life of Americans](https://flowingdata.com/2015/12/15/a-day-in-the-life-of-americans/) | State the simulation and particle unit for moving activity dots. On a slide, use two snapshots of the same simulated time series. |
| 060 | [Landscape of Power Flows](https://www.visualcinnamon.com/portfolio/landscape-of-power-flows/) | Trace corridors with direction cues and a clear legend. Distinguish geographic distance from the network connections. |

## Maps and spatial comparisons

| ID | Public example | Design application and checks |
|---|---|---|
| 061 | [The True Size Of…](https://thetruesize.com/) | Use drag-and-compare to expose projection effects. Keep a before/after pair and explain which spatial property is preserved. |
| 062 | [Human Terrain](https://pudding.cool/2018/10/city_3d/) | Use height to introduce density. Give a cross-section or numeric scale for comparison and inspect occlusion from the chosen view. |
| 063 | [earth.nullschool.net](https://earth.nullschool.net/) | Label time, direction and units in a flow field. Keep the direction key in static output and distinguish streamlines from tracked trajectories. |
| 064 | [Norway Travel Map](https://www.visualcinnamon.com/portfolio/map-norway/) | Separate terrain, routes, stops and location observations. Keep the route and key landmarks at slide size and disclose sampling gaps. |
| 065 | [A Giant Map of the World](https://www.visualcinnamon.com/portfolio/worldmap/) | Plan one label hierarchy for overview and another for zoom. Pair a global view with one crop and explain scale-dependent mark density. |
| 066 | [NYC’s Urban Textscape](https://pudding.cool/2025/07/street-view/) | Connect searchable street text to coordinates and observation records. Show an example observation and state coverage limits. |
| 067 | [Imaging the Entire Earth, Every Day](https://www.visualcinnamon.com/portfolio/planet-globe/) | Use the globe as a spatial context for observation frequency. Retain coverage, window and observation definition, including the treatment of clouds. |
| 068 | [Happy Map](https://pudding.cool/2026/02/happy-map/) | Keep event record density distinct from population density. Include a sample note beside a visible cluster. |
| 069 | [Choosing a Choropleth Palette](https://www.datawrapper.de/blog/how-to-choose-a-color-palette-for-choropleth-maps) | Use ordered lightness for numeric intervals and give missing values a distinct style. Retain the range legend and avoid treating land area as statistical weight. |
| 070 | [Dollar Street](https://www.gapminder.org/dollar-street) | Organize comparable household objects by an income axis. Keep matched objects and explain how households were selected. |

## Editorial storytelling and evidence

| ID | Public example | Design application and checks |
|---|---|---|
| 071 | [In Pursuit of Democracy](https://pudding.cool/2025/11/democracy/) | Connect selected timeline marks to attributable records. Keep the overall trend and one sourced excerpt and state the selection scope. |
| 072 | [Women’s Pockets Are Inferior](https://pudding.cool/2018/08/pockets/) | Overlay shapes at a common scale and allow an object-fit test. Keep the tested dimensions and distinguish geometry from everyday use. |
| 073 | [A History of Menus is a Menu of History](https://pudding.cool/2026/06/menu-story/) | Lead with one archival menu and connect it to era-level evidence. Explain how preservation and collection affect the sample. |
| 074 | [5,000 Restaurant Menus](https://pudding.cool/2026/06/menu-collection/) | Expose archive records through a searchable view next to summary findings. Keep the sample filter and one record with clear scope. |
| 075 | [Bears Will Be Boys](https://pudding.cool/2025/07/kids-books/) | Use source-book imagery for recognition while preserving a clear quantitative encoding. Explain the category rules and sample. |
| 076 | [Film Dialogue by Gender](https://pudding.cool/2017/03/film-dialogue/) | Link summary shares to film-level records. Label the unit as dialogue lines and distinguish it from character counts or screen time. |
| 077 | [Asian Misrepresentation](https://pudding.cool/2025/05/aapi-casting/) | Show sample composition and demographic baseline together. Align region and time scope before describing the difference. |
| 078 | [How Musicals Use Motifs](https://pudding.cool/2025/12/motifs/) | Use synchronized audio and a visual motif marker. Provide a textual alternative and separate repetition from claims about intent. |
| 079 | [Walkachusetts](https://pudding.cool/2025/10/walk/) | Synchronize route, observations and narrative at specific stops. Keep a supported segment and qualify claims drawn from one route. |
| 080 | [30 Minutes with a Stranger](https://pudding.cool/2025/06/hello-stranger/) | Align source material and observations on a shared timeline. Explain time matching and how any emotional measures were obtained. |

## Interaction and simulation

| ID | Public example | Design application and checks |
|---|---|---|
| 081 | [Dicing an Onion](https://pudding.cool/2025/08/onions/) | Make one manipulable input update both the graphic and the metric. Compare fixed-input states in slides and state model assumptions. |
| 082 | [Gapminder World Health Chart](https://www.gapminder.org/fw/world-health-chart/) | Animate trajectories with time controls and pause. Preserve the bubble-area unit and use two dated states for static output. |
| 083 | [Why the Super Rich Are Inevitable](https://pudding.cool/2022/12/yard-sale/) | Expose model parameters, initial conditions and random variation. Compare fixed scenarios and state the effect of a single draw. |
| 084 | [Washington Post · Flatten the Curve Simulation](https://www.washingtonpost.com/graphics/2020/world/corona-simulator/) | Compare simulations at matching times with a shared scale. Distinguish individual random runs from the demonstrated mechanism. |
| 085 | [The Largest Vocabulary in Hip Hop](https://pudding.cool/2017/02/vocabulary/) | Make the ranked view searchable without changing the comparison window. Keep the shared vocabulary window and explain tokenization and sampling. |
| 086 | [How People Like You Spend Their Time](https://flowingdata.com/2016/12/06/how-people-like-you-spend-their-time/) | Let readers choose a group while keeping the activity and time scale aligned. Update the sample definition with the selection. |
| 087 | [CFR Global Inflation Tracker](https://www.cfr.org/articles/global-inflation-tracker) | Choose filters around a clear comparison question. Keep periods and frequency aligned and distinguish price levels from growth rates. |
| 088 | [Population & Demography Explorer](https://ourworldindata.org/explorers/population-and-demography) | Update title, denominator and unit with the selected metric. Keep a fixed state for export and state geographic and time scope. |
| 089 | [Reuters Japan Population](https://graphics.thomsonreuters.com/14/japan_pop/index.html) | Compare matching age bands across years. Make the choice between counts and shares explicit. |
| 090 | [World’s Biggest Data Breaches](https://informationisbeautiful.net/visualizations/worlds-biggest-data-breaches-hacks/) | Use bubble area to locate large cases then expose precise records in labels or details. State the reporting scope and area unit. |

## Data art and static composition

| ID | Public example | Design application and checks |
|---|---|---|
| 091 | [Film Flowers](https://sxywu.github.io/filmflowers/) | Assign each custom glyph feature a clear variable. Keep a legible legend and use aligned positions when precise ranking matters. |
| 092 | [Cycle of Many](https://flowingdata.com/2021/08/25/cycle-of-many/) | Use a circular layout for periodic time and map dot density to share. Keep the time direction and a small number of labeled rings. |
| 093 | [Gold Record with Data Art](https://www.visualcinnamon.com/portfolio/sony-music-data-art/) | Design one recognizable shape for distance and detail for close inspection. Identify the portions that carry data. |
| 094 | [Top 39 Actors](https://www.visualcinnamon.com/portfolio/graffu-actors/) | Use subject-specific movie symbols when they support recognition. Check each shape variable against its legend and keep representative records. |
| 095 | [Figures in the Sky](https://www.visualcinnamon.com/portfolio/figures-in-the-stars/) | Overlay interpretations on the same star coordinates. Include a two-culture comparison and state differences in historical coverage. |
| 096 | [An Ode to Cardcaptor Sakura](https://www.visualcinnamon.com/portfolio/cardcaptor-sakura/) | Separate narrative, data and decorative roles when extending a recognizable theme. Keep key records, scale and legend visible. |
| 097 | [The Top 2000 ❤ the 70s & 80s](https://www.visualcinnamon.com/portfolio/top2000/) | Use discrete time structure and a few artist highlights for orientation. Keep the chart population and distinguish chart records from listening behavior. |
| 098 | [Meet the Neighbors](https://www.visualcinnamon.com/portfolio/exoplanet-neighbors/) | Use separate frames for distinct scales and label each scale. Avoid mapping page spacing to physical distances. |
| 099 | [Space Wars](https://www.visualcinnamon.com/portfolio/space-wars/) | Maintain visible record-level points while grouping by meaningful orbit classes. Keep date and point units and clarify symbol size. |
| 100 | [Olympic Feathers](https://www.visualcinnamon.com/portfolio/olympic-feathers/) | Reuse the same mark-to-medal mapping across events. Label time and groups and account for different opportunities to win medals. |

## Probability, forecasts and decision paths

| ID | Public example | Design application and checks |
|---|---|---|
| 101 | [512 Paths to the White House · Creator's Notes](https://source.opennews.org/articles/nyts-512-paths-white-house/) | Keep conditional state filtering separate from outcome probability. Show an initial state and outcome branches, and distinguish path count from chance. |
| 102 | [Bank of England · CPI Forecast Fan Chart](https://www.bankofengland.co.uk/monetary-policy-report/2026/november-2026) | Use labeled probability bands around a central forecast. Keep one or two bands and state coverage and assumptions, including possible outcomes outside the bands. |
| 103 | [ggdist · Quantile Dotplots](https://mjskay.github.io/ggdist/articles/dotsinterval.html) | Show equal-weight probability dots against a threshold. Label probability and distinguish discretized model draws from observations. |
| 104 | [UW IDL · Hypothetical Outcome Plots](https://idl.uw.edu/papers/hops-trends) | Explain that animation frames are distinct possible trajectories. In static output, keep a small set of draws, benchmark and model description. |
| 105 | [UW IDL · Bus Arrival Uncertainty](https://idl.uw.edu/papers/uncertainty-bus) | Place a decision threshold beside the distribution. Label the probability of meeting it and distinguish that probability from mean arrival time. |
| 106 | [En-ROADS · Global Climate Simulator](https://www.climateinteractive.org/en-roads/) | Keep a fixed scenario baseline as controls change. Label changed assumptions and distinguish modeled outcomes from scenario likelihood. |

## Linked exploration

| ID | Public example | Design application and checks |
|---|---|---|
| 107 | [Observable · Penguin Scatterplot and Histogram](https://old.observablehq.com/blog/linked-brushing) | Brush one variable and show the linked distribution on a common axis. Keep full context and selection counts. |
| 108 | [Vega · Flight Crossfilter](https://vega.github.io/vega/examples/crossfilter-flights/) | Make multiple filters, their intersection and the reset action visible. State the filtered population for every readout. |
| 109 | [Vega-Lite · Crossfilter Highlight](https://vega.github.io/vega-lite/examples/interactive_layered_crossfilter.html) | Overlay a highlighted subset on a common distribution and bins. Show its sample size so raw counts remain interpretable. |
| 110 | [UK ONS · How the Population Changed Where You Live](https://www.ons.gov.uk/peoplepopulationandcommunity/populationandmigration/populationestimates/articles/howthepopulationchangedwhereyoulivecensus2021/2022-06-28) | Keep the same story sequence for each region with a national benchmark. Explain how boundaries and denominators affect comparisons. |

## Static and interactive delivery

| ID | Public example | Design application and checks |
|---|---|---|
| 111 | [BBC · News Chart Style](https://bbc.github.io/rcookbook/) | Stabilize typography, title slots, whitespace and source placement across chart families. Retest labels and units after applying the theme. |
| 112 | [Datawrapper · Accessible Interactive Charts](https://www.datawrapper.de/blog/better-accessibility-for-datawrapper-visualizations) | Give interaction states text or shape cues as well as color. Test keyboard access and make a readable static state. |
| 113 | [Datawrapper · Text in Charts](https://www.datawrapper.de/blog/text-in-data-visualizations) | Place a note near the relevant mark and test its attachment at narrow widths. Retain the finding, local evidence and unit in a crop. |

## Interpretation and correction

| ID | Public example | Design application and checks |
|---|---|---|
| 114 | [Distill · How to Use t-SNE Effectively](https://distill.pub/2016/misread-tsne/) | Compare multiple settings on the same data and explain the embedding assumptions. Interpret local clusters without treating displayed distances as original distances. |
| 115 | [Datawrapper · Missing Data in Line Charts](https://www.datawrapper.de/academy/missing-data-in-line-charts) | Keep the time slots for missing observations and show a gap unless imputation is clearly indicated. Preserve the missing-period explanation in static output. |
| 116 | [Spurious Correlations](https://www.tylervigen.com/spurious-correlations) | Keep unrelated series in their original units and qualify coincident movement. Avoid scales that imply unsupported causal relationships. |

## Chinese-language editorial examples

| ID | Public example | Design application and checks |
|---|---|---|
| 117 | [The Paper · Spring Festival High-speed Rail Ticket Index (Chinese)](https://www.thepaper.cn/newsDetail_forward_26181341) | Define the index before the route comparison. Keep long Chinese place names and the method legible at delivery size. |
| 118 | [The Paper · 74 Years of Chinese Population (Chinese)](https://www.thepaper.cn/newsDetail_forward_25793167) | Use one chronological spine for values, periods and turning points. Distinguish population totals, age structure and increments. |
| 119 | [The Paper · 15 Years of Train Timetables (Chinese)](https://www.thepaper.cn/newsDetail_forward_32482558) | Compare timetable periods on a stable time or route structure. Distinguish planned service from observed passengers. |
| 120 | [The Paper · Spring Festival Travel Report (Chinese)](https://www.thepaper.cn/newsDetail_forward_26181344) | Keep a short scale, annotated peak and time-window definition. State what transport trips count and whether the measurement window changed. |

## Public examples with implementation

| ID | Public example | Design application and checks |
|---|---|---|
| 121 | [Vega-Lite · Horizontal Bars with Negative Values and Labels](https://vega.github.io/vega-lite/examples/bar_negative_horizontal_label.html) | Emphasize the shared zero line and put values at signed bar ends. Verify positive, negative and zero cases read correctly. |
| 122 | [Vega-Lite · Slope Graph](https://vega.github.io/vega-lite/examples/line_slope.html) | Label both periods on one vertical scale and connect matching entities. Move to aligned rows when lines crowd. Describe change between endpoints only. |
| 123 | [Vega-Lite · Line Chart with Invalid Values](https://vega.github.io/vega-lite/examples/line_skip_invalid_mid_overlay.html) | Keep expected periods visible and break the line where values are missing. Leave valid zeros plotted and check missing markers and segments. |
| 124 | [Vega-Lite · Top-K and Others](https://vega.github.io/vega-lite/examples/window_top_k_others.html) | Aggregate the categories outside the leading set into Others. Keep it clearly labeled and reconcile totals and ties at the cutoff. |
| 125 | [Vega-Lite · Ranged Dot Plot](https://vega.github.io/vega-lite/examples/layer_ranged_dot.html) | Use one row per category with two distinct endpoint symbols. Check endpoint identity and line length when direction reverses. |
| 126 | [Vega-Lite · Histogram with Global Mean Overlay](https://vega.github.io/vega-lite/examples/layer_histogram_global_mean.html) | Use a light reference line for the overall mean. Verify bar heights and mean independently. Match bin boundaries across comparable groups. |
| 127 | [Vega-Lite · Trellis Scatterplot](https://vega.github.io/vega-lite/examples/trellis_scatter.html) | Share axis domains across wrapped facets and align panel titles. Label sparse panels and check that equal values map to equal relative positions. |
| 128 | [Vega-Lite · Scatterplot with Marginal Histograms](https://vega.github.io/vega-lite/examples/concat_marginal_histograms.html) | Align the marginal histograms with their corresponding scatter axes. Check sample and filtering consistency and clearly label counts. |
| 129 | [Vega-Lite · Hover and Click Selection](https://vega.github.io/vega-lite/examples/interactive_bar_select_highlight.html) | Use hover for previews and selection for persistent focus. Provide equivalent keyboard actions and check that geometry stays fixed. |
| 130 | [Vega-Lite · Scatter Brush and Table](https://vega.github.io/vega-lite/examples/brush_table.html) | Connect a scatter brush to record details through stable keys. Show both total matches and displayed rows when capped. Test empty and cleared states. |
| 131 | [Vega-Lite · Overview and Detail](https://vega.github.io/vega-lite/examples/interactive_overview_detail.html) | Keep the full time period in the overview and the selected range in the detail. Verify range alignment, units and reset. |
| 132 | [Vega-Lite · Line Chart with Confidence Band](https://vega.github.io/vega-lite/examples/layer_line_errorband_ci.html) | Draw the estimate above a subdued confidence band. Label the interval definition and coverage and check bounds for clipping or forecast mislabeling. |
