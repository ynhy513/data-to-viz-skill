# Data to Viz Skill

**English** | [简体中文](README.zh-CN.md)

A reusable Agent Skill for **choosing, creating, and reviewing data visualizations**. It builds on [From Data to Viz](https://www.data-to-viz.com/)'s data-format decision tree and chart caveats, adding purpose-driven selection, tool routing, numerical checks, and verification of rendered output.

## How it works

1. **Define the question and data contract:** what the audience needs to compare, what one row represents, and whether units, denominators, missing values, and aggregation are correct.
2. **Narrow by data structure, then choose by purpose:** distribution, comparison, association, time, composition, hierarchy, networks, or geography. Compare a credible alternative when it helps resolve the choice.
3. **Use the appropriate creation tool:** preserve the requested tool, format, editability, and delivery destination.
4. **Check what could mislead:** scales, area encoding, binning, sample size, uncertainty, overplotting, missingness, weighting, and causal language.
5. **Verify the result:** distinguish artifact generation, numerical checks, rendering and interaction checks, and evidence of actual audience outcomes.

The skill supplies reasoning and review rules; available renderers or plugins create the chart. Basic chart selection needs no additional plugin. Creation uses tools available in the current environment.

## Installation

In a Codex environment that supports Agent Skills, install it in the user-level skills directory:

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/ynhy513/data-to-viz-skill.git ~/.agents/skills/data-to-viz
```

If your environment uses `~/.codex/skills`, substitute that installation root. Choose a location recognized by your client and avoid installing two copies with the same skill name. Refresh or restart the client if the new skill does not appear. See the [Codex skills documentation](https://learn.chatgpt.com/docs/build-skills).

The repository root is the skill directory and contains `SKILL.md`, `agents/`, and `references/`. Installation does not require copying personal configuration from outside this repository.

## Usage

Invoke the skill explicitly:

```text
Use $data-to-viz to choose and create a chart for this dataset. Explain the choice and check the relevant caveats.
```

You can also describe a visualization task without naming the skill. `agents/openai.yaml` allows implicit invocation, but the client must first discover the skill and the model then selects it from its description. A successful invocation does not guarantee selection for every future task.

For an explicit routing rule in your own environment, add something like this to the applicable `AGENTS.md`, adjusting the path to match your installation:

```markdown
For quantitative chart selection, creation, revision, or review, first read
`~/.agents/skills/data-to-viz/SKILL.md` and apply its decision tree and relevant caveats.
Then use the appropriate renderer or plugin for the requested destination.
Exclude pure conceptual diagrams and tasks such as translation that only mention charts.
```

Example requests:

- “I need to compare sales across 12 countries, mainly to see the ranking. Which chart fits?”
- “Create a monthly revenue chart with a channel selector. Keep missing values distinct from zero.”
- “Create a revenue and profit scenario calculator with adjustable price and demand.”
- “Review this chart for truncated axes, hidden distributions, or exaggerated claims.”

## Working with creation tools

| Task | Presentation responsibility |
| --- | --- |
| Standard charts, date/category filters, and series selection | Use Data's standard chart component when available |
| In-conversation scenario calculators, simulations, and interactive explainers | Let Visualize own the whole tool, including its charts, when available |
| React chart or map components in an existing application | Preserve the project stack and use relevant web visualization specialists |
| Scientific figures, PNG/PDF/SVG exports, editable workbooks, or presentations | Use plotting or native artifact tools suited to the requested format |
| Pure conceptual structure diagrams | Use an appropriate diagram method, such as Mermaid, without forcing quantitative-chart rules onto it |

These plugins are optional, not mandatory dependencies. When unavailable, use an appropriate available alternative and state the actual limitation. See [desktop routing](references/desktop-routing.md) for the detailed ownership rules.

## Contents

- [SKILL.md](SKILL.md): scope, triggers, and the main workflow.
- [Chart-selection decision tree](references/decision-tree.md): select charts by data structure and analytical purpose.
- [Caveats](references/caveats.md): conditional chart checks and remedies.
- [Creation and verification](references/create-and-verify.md): prepare data, create the artifact, and verify the result.
- [Desktop routing](references/desktop-routing.md): resolve overlapping responsibilities between visualization capabilities.

## Validation performed

Development-environment checks on **2026-11-04** covered skill structure, implicit invocation from ordinary requests, exclusion of adjacent tasks, and actual Data and Visualize preview runs. Channel selection, missing versus zero, modeled calculations, zero demand, and reset were checked. Display and controls for both native in-chat examples were also manually confirmed.

These checks apply to specific fixtures and one environment. They do not establish compatibility with every client, plugin version, input combination, or future invocation, nor do they demonstrate audience comprehension or business effectiveness. Third-party plugin runtimes and local debugging records are not bundled in this repository.

## Sources and license

The method draws on [From Data to Viz](https://www.data-to-viz.com/), by **Yan Holtz and Conor Healy**, particularly its [project philosophy](https://www.data-to-viz.com/about.html), [data stories](https://www.data-to-viz.com/#story), and [chart caveats](https://www.data-to-viz.com/caveats.html).

This is an adapted and extended operational guide, not a node-for-node reproduction of the original twenty-format poster. The documents distinguish additions such as data-quality checks, delivery verification, and plugin routing. This project is independently maintained and is not endorsed by the upstream project or OpenAI.

Original contributions in this repository use the [MIT License](LICENSE). Upstream attribution and licensing information are in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
