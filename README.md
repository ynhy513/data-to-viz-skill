# Data to Viz Skill

用于**选图、制作和审查数据可视化**的可复用 Agent Skill。以 [From Data to Viz](https://www.data-to-viz.com/) 的数据结构决策树和常见图表陷阱为基础，补充任务目的、工具路由、数值核对与实际渲染验收。

An Agent Skill for choosing, creating, and reviewing truthful charts. It combines an adapted Data to Viz decision tree with conditional caveat checks and clear ownership between chart, calculator, web, and artifact workflows.

## 工作方式

1. **明确问题与数据口径**：受众要看什么关系，一行数据代表什么，单位、分母、缺失值和聚合是否正确。
2. **按数据结构筛选，再按目的选图**：分布、比较、关联、时间、组成、层级、网络或地理；必要时比较一个合理替代方案。
3. **调用合适的制作工具**：保留用户指定的工具、格式、可编辑性和交付位置。
4. **检查可能误导的地方**：刻度、面积、分箱、样本量、不确定性、遮挡、缺失值、加权口径与因果措辞。
5. **验证实际结果**：区分产物生成、数值核对、渲染与交互检查，以及真实受众效果。

Skill 提供方法与检查规则，实际图表由环境中可用的渲染器或插件完成。基础选图不需要额外插件；制作时使用已有工具。

## 安装

在支持 Agent Skills 的 Codex 环境中，可安装到用户级技能目录：

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/ynhy513/data-to-viz-skill.git ~/.agents/skills/data-to-viz
```

如果你的环境使用 `~/.codex/skills`，将上述安装根目录替换为该路径。选择一个被当前客户端识别的目录，避免同时安装两份同名 Skill。客户端未显示新 Skill 时，可刷新或重新启动。参见 [Codex 技能说明](https://learn.chatgpt.com/docs/build-skills)。

仓库根目录就是技能目录，包含 `SKILL.md`、`agents/` 和 `references/`。安装不需要复制本仓库以外的个人配置。

## 使用

显式调用：

```text
用 $data-to-viz 帮我选择并制作这组数据的图表，说明选图理由并检查相关问题。
```

也可直接提出数据可视化任务。`agents/openai.yaml` 已允许隐式调用；客户端仍需先发现技能，模型再根据描述选择。不能把一次调用成功视为所有未来任务都必然调用。

如果希望为自己的环境增加明确路由，可在适用的 `AGENTS.md` 中加入类似规则，并按实际安装路径调整：

```markdown
涉及定量图表的选图、制作、修改或审查时，先读取
`~/.agents/skills/data-to-viz/SKILL.md`，应用其决策树与相关 caveats，
再按交付目标使用合适的渲染器或插件。纯概念图和仅提及图表的翻译等任务不触发此规则。
```

可尝试的任务：

- “比较 12 个国家的销售额，主要想看排名，应该用什么图？”
- “做一个带渠道选择器的月收入图，缺失值和零要分开。”
- “做一个可调价格和销量的收入、利润情景计算器。”
- “审查这张图有没有截断坐标轴、隐藏分布或夸大结论的问题。”

## 与制作工具配合

| 任务 | 制作职责 |
| --- | --- |
| 标准图表、日期/分类筛选、系列选择 | 可用时使用 Data 的标准图表组件 |
| 聊天中的情景计算器、模拟器、交互解释器 | 可用时由 Visualize 负责整个工具及其中的图表 |
| 已有应用中的 React 图表或地图组件 | 保留项目技术栈，使用相关 Web 专项能力 |
| 科学图片、PNG/PDF/SVG、可编辑工作簿或演示稿 | 使用适合所需格式的绘图或原生文档工具 |
| 纯概念结构图 | 使用对应图示方法，如 Mermaid；不强套定量图表规则 |

这些插件不是强制依赖。未安装时，使用可用且适合目标的替代工具，并说明实际限制。详细规则见 [桌面工具路由](references/desktop-routing.md)。

## 内容

- [SKILL.md](SKILL.md)：触发范围与主要工作流程。
- [选图决策树](references/decision-tree.md)：按数据结构和表达目的选择图表。
- [常见陷阱](references/caveats.md)：有条件的图表检查与修正方法。
- [制作与验收](references/create-and-verify.md)：数据准备、制作和验证。
- [桌面工具路由](references/desktop-routing.md)：处理多个可视化能力的职责重叠。

## 已做的验证

2026-11-04 的开发环境验证包括技能结构检查、自然语言自动调用测试、相邻任务的排除检查，以及 Data 与 Visualize 的实际预览测试。渠道筛选、缺失与零、情景计算、零销量及重置路径均已检查；两个原生聊天内联实例的显示与控件也经人工确认。

这些是特定环境和示例的验证，不能证明所有客户端、插件版本、输入组合或未来调用都正常，也不代表受众理解或商业效果已验证。本仓库不打包第三方插件运行时或本机调试记录。

## 来源与许可

方法来源为 Yan Holtz 与 Conor Healy 的 [From Data to Viz](https://www.data-to-viz.com/)，尤其是其 [项目理念](https://www.data-to-viz.com/about.html)、[数据示例](https://www.data-to-viz.com/#story) 与 [常见陷阱](https://www.data-to-viz.com/caveats.html)。

这里是经过改写并扩展的操作指南，不是原网站二十种数据格式海报的逐节点复刻。数据质量、交付验证和插件路由等扩展已在文档中区分。该项目独立维护，未获上游项目或 OpenAI 背书。

本仓库原创内容采用 [MIT License](LICENSE)。上游来源署名与许可见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。
