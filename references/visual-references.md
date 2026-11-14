# Data to Viz｜120 个视觉参考案例

这份索引适用于已经有数据与读者问题，需要为图表选择表达方式、视觉语言或交互的工作。纳入标准是案例有可指认的设计手法，并能说清它适用于什么情境。原有 100 个编号保留，新增 20 个案例，涵盖概率与决策路径、联动探索、静态与交互交付、误读修正和中文编辑设计。每条附半页 PPT 的取舍与易错读法。

## 按问题查找

- 001–010 排名、简报与直接标注
- 011–020 时间、节奏与转折
- 021–030 组成、加减与份额
- 031–040 分布、例外与不确定性
- 041–050 关系、关联与网络
- 051–060 流向、迁移与路径
- 061–070 地理位置与空间感
- 071–080 编辑叙事与可核查证据
- 081–090 交互、模拟与视图切换
- 091–100 数据艺术与静态构图

- 101–106 概率、预测与决策路径
- 107–110 联动探索与逐层展开
- 111–113 静态与交互交付
- 114–116 误读与修正
- 117–120 中文编辑设计

## 首批 10 个入门案例

原有十类各选一例。案例通过链接打开，作者作品页有时会同时提供图像、过程和交互入口。

- **001** [F12 Dumbbell Queue](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Dumbbell%20Queue)。前后配对。百分数先确定单位粒度，保留精确端点。

- **011** [Show Your Stripes](https://showyourstripes.info/)。长序列气氛图，精确值另配折线或注释。

- **021** [瀑布图的小计与直标](https://www.datawrapper.de/blog/waterfall-charts)。桥接期初、变动项与期末，保证逐项可对账。

- **031** [The Radius Gap](https://www.visualcinnamon.com/portfolio/radius-gap/)。均值不足以说明分布时，先找聚集与缺口。

- **041** [Royal Constellations](https://www.visualcinnamon.com/portfolio/royal-constellations/)。依赖图高亮选定节点、邻居与路径，保留其他节点作背景。

- **051** [OECD Global Plastics Outlook](https://www.visualcinnamon.com/portfolio/oecd-global-plastics-outlook/)。前后桑基图沿用节点顺序与比例口径。

- **061** [The True Size Of…](https://thetruesize.com/)。地图切换前后明确正在比较的空间属性。

- **071** [In Pursuit of Democracy](https://pudding.cool/2025/11/democracy/)。标记连接来源或样本，注明精选范围。

- **081** [Dicing an Onion](https://pudding.cool/2025/08/onions/)。交互每次改变可说明的输入，并联动图形和读数。

- **091** [Film Flowers](https://sxywu.github.io/filmflowers/)。自定义图形每个通道写明定义，精确排名另用位置。

## 让 Data to Viz 使用这份索引

1. 写明读者要回答的问题、数据单位、分母和交付媒介，再选一个主图类型。

2. 从最接近的两类里最多找 3 个案例。打开原作，记录值得迁移的具体手法，例如对齐、可数刻度、证据标注或交互展开。

3. 用自己的数据重新设计。确认视觉单位与数据一致，网页的交互状态可用，PPT 或图片的静态版能保留关键发现。

4. 对照原始数据验算，并在实际输出尺寸复查标签、对比度、重点和样本口径。用「容易误读什么」检查标题和图形是否会引出过度解读。缩成 PPT 半页时，参考保留项，在实际尺寸核查。引用案例编号便于复盘。

**可直接使用的提示词**

> 用 data-to-viz 为这组数据选图。读《120 个视觉参考案例》，按读者的问题挑最多三个参考。打开原作，指出每个案例的一条可迁移手法，然后制作原创图表。交付时标注参考编号、采用的设计决策，以及数值和最终渲染的检查结果。

案例链接指向公开作品或发布方样例页。索引中的观察和迁移建议是本项目整理的读图笔记。直接复用原作的图像、代码或模板时，以各作者的授权条款为准。

## 排名、简报与直接标注

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 001 | [F12 Dumbbell Queue](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Dumbbell%20Queue) | 用可数串珠给哑铃线段一个真实单位。 | 前后配对。百分数先确定单位粒度，保留精确端点。 | 两期端点、单位、变化值 | 珠子数是变化幅度，方向看两期位置 |
| 002 | [F5 Tick Rows](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Tick%20Rows) | 把横向排名拆成可数刻线，类别名贴近标记。 | 类别少、数值有自然单位时可做简报。 | 前五项、直标、单位 | 一格的单位需要显式说明 |
| 003 | [G3 Chunky Bars](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Chunky%20Bars) | 用粗形状和直标缩短读图时间。 | 周报用长度比较，优先把数值标在柱旁。 | 零基线、关键柱、排序 | 柱长从非零值开始会夸大差距 |
| 004 | [爱尔兰奥运排名 · 修正版](https://www.datawrapper.de/blog/irish-times-chart-redesigned-olympics) | 让第 1 名出现在顶部，保留主办城市作时间锚点。 | 名次、优先级、等级的顺序要符合读者直觉。 | 主办城市、名次方向、关键年份 | 参赛范围不同，名次的含义会变 |
| 005 | [选举结果对比列](https://www.datawrapper.de/blog/comparison-columns) | 把本次结果与上次结果并排，让数字与差值对得上。 | 读者既要看当前水平又要看同比时使用。 | 当前和上期、差值单位 | 份额变化用百分点，别混成相对增幅 |
| 006 | [The 100 Tallest Buildings in the World](https://www.visualcinnamon.com/portfolio/skyscrapers/) | 建筑轮廓强化题材识别，特别适合整页视觉。 | 从对象借剪影，正式精确排名另用共基线。 | 关键建筑及共同高度标尺 | 透视远近影响目测大小 |
| 007 | [Top 10 Nintendo Switch Games](https://www.visualcinnamon.com/portfolio/best-selling-nintendo-switch-games/) | 用与游戏主题相连的实体图形做排行榜。 | 封面或故事页借形体，柱长仍应承担精确比较。 | 前三项销量和统一尺度 | 实体符号的体积容易抢过长度编码 |
| 008 | [Ethical NBA Championships, Ranked](https://pudding.cool/2026/06/ethical-champions/) | 把带前提的冠军排名写成可解释的编辑叙事。 | 综合榜单保留定义和判定依据。 | 前三名、评判规则短句 | 榜单顺序依赖作者定义 |
| 009 | [点图与条形图旁注样例](https://www.datawrapper.de/blog/annotations-in-bar-charts) | 在窄柱或小点旁用短引线解释该数据点的意义。 | 直接在异常点旁放注释，避免读者往返图例。 | 一个焦点、引线、数值 | 旁注选中的事例不能代表所有点 |
| 010 | [互联网使用率](https://ourworldindata.org/grapher/share-of-individuals-using-the-internet) | 用百分比坐标比较不同地区的普及水平。 | 跨市场 adoption 图优先展示共同口径和单位。 | 地区对比、共同年份、分母 | 上网人口占比无法反映使用频率 |

## 时间、节奏与转折

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 011 | [Show Your Stripes](https://showyourstripes.info/) | 把每年压缩成时间顺序中的一条色带。 | 长序列气氛图，精确值另配折线或注释。 | 起止年份、基准温度、色阶 | 红蓝通常是距基准的偏差 |
| 012 | [小多图折线样例](https://www.datawrapper.de/blog/small-multiple-line-charts) | 用重复的小画幅让多条趋势变得可扫读。 | 按职能比较趋势时优先共享尺度。 | 少数面板、共享轴、直接标题 | 各面板独立纵轴会放大微小变化 |
| 013 | [折线直标和符号样例](https://www.datawrapper.de/blog/improved-line-chart-editing) | 线条与端点文字尽量在同一阅读位置。 | 通常只直标关键线，其余留作参考。 | 关键线、端点、时间单位 | 连接线可能跨过缺失月份 |
| 014 | [Top 10 Baby Names](https://www.visualcinnamon.com/portfolio/babynames/) | 沿长期时间轴读单个名字进出榜单的变化。 | 看排名轨迹时让读者可追踪同一对象。 | 两三个名字、名次纵轴 | 离开前十仍可能很常见 |
| 015 | [A Year in Flights](https://www.visualcinnamon.com/portfolio/a-year-in-flights/) | 全年的数据可作远看有节奏、近看能读细节的大画幅。 | 日历型记录适合海报和办公室展示。 | 一个季度的时间网格和总量 | 繁密纹理容易被当作数量 |
| 016 | [GitHub Commit History Timeline](https://www.visualcinnamon.com/portfolio/orca-github-commits/) | 给全部提交一条可探索的历史轴。 | 日志型时间线用总览定位，再显示选中期间记录。 | 全期时间轴、一个局部放大 | 提交数不能直接代表工作量 |
| 017 | [Satellite Surge](https://www.visualcinnamon.com/portfolio/sciam-satellite-surge/) | 把大主题拆成可对照的轨道与重量分组，突出一组突增。 | 总体上升时用分组显示变化集中在哪。 | 增长最快分组和背景组 | 不同重量或轨道分组的口径须一致 |
| 018 | [GenCoop · 瑞士太阳能](https://www.visualcinnamon.com/portfolio/swissgrid-gencoop/) | 分别讲长期装机扩张与一年中的发电节律。 | 分开设计长期变化和季节周期，避免共用一条时间轴。 | 一个季节对比或一个长期趋势 | 装机是存量，发电是流量 |
| 019 | [Life Expectancy](https://ourworldindata.org/grapher/life-expectancy) | 给长时间跨度的多地区趋势保留直接比较入口。 | 让读者从少数参考线开始，再添加关注对象。 | 少数地区、起末读数 | 时期生命表指标不是实际出生队列寿命 |
| 020 | [城市人口占比至 2050 年](https://ourworldindata.org/grapher/urban-population-share-2050) | 在同一时间语境中放入历史与预测。 | 明确区分观测段、预测段与分界年。 | 历史实线、预测虚线、分界年 | 情景投影受假设驱动 |

## 组成、加减与份额

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 021 | [瀑布图的小计与直标](https://www.datawrapper.de/blog/waterfall-charts) | 用阶段小计给累计方向提供停顿点。 | 桥接期初、变动项与期末，保证逐项可对账。 | 起点、主要增减、终点 | 中间柱是变动量，终点柱是总量 |
| 022 | [F7 Stacked Rungs](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Stacked%20Rungs) | 堆叠讲加总，横档提供局部读数。 | 分组构成须共享单位，图例顺序贴合堆叠顺序。 | 少数分组、档位单位、总量 | 堆叠中段没有共同基线 |
| 023 | [L14 Hundred Field](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Hundred%20Field) | 把 100% 的整体摊成可数单元。 | 份额有共同分母且合计完整时可用。 | 核心份额、总分母、点单位 | 多选题加总可能超过 100% |
| 024 | [F4 Tick Donut](https://github.com/larashero3-dotcom/lieflat-charts/blob/main/catalog.md#:~:text=Tick%20Donut) | 环上的刻度让份额对应可解释单位。 | 少数类别做概览，接近的份额改用共基线读数。 | 主份额和其余合计 | 接近的圆弧难做精确比较 |
| 025 | [Treemap 层级示例](https://www.data-to-viz.com/graph/treemap.html) | 面积给权重，包围关系给层级。 | 组合总览先标父组，精确排序另给条形。 | 父类、最大块、权重单位 | 格子位置不表示相似性 |
| 026 | [堆叠面积图示例](https://www.data-to-viz.com/graph/stackedarea.html) | 让外轮廓读总量，内部层读组成。 | 基线会影响中间层的比较，重点系列放底部。 | 总轮廓、底层重点、图例 | 中间层应读厚度而非上边界 |
| 027 | [全球一次能源来源](https://ourworldindata.org/grapher/global-primary-energy-by-source) | 同一长序列呈现不同来源对总量的叠加。 | 年度结构变化结合来源颜色与图例排序。 | 主要来源、总量轴、年份 | 能源绝对量和各来源份额含义不同 |
| 028 | [Energy Mix · 跨国能源结构](https://ourworldindata.org/energy-mix) | 把能源结构放进统一口径下比较。 | 地区驱动分析先区分绝对量与相对份额。 | 两三个地区和相同口径 | 初级能源与发电结构的分母不同 |
| 029 | [可再生电力占发电量的比重](https://ourworldindata.org/grapher/electricity-mix?frequency=annual&metric=share_of_generation&source=renewables) | 用明确的分母定义避免把发电结构读成能源总量。 | 同一套 KPI 给份额和绝对量各自标签。 | 一个国家对照、比例与分母 | 发电量占比不是装机占比 |
| 030 | [The Billion Dollar Gram](https://informationisbeautiful.net/visualizations/the-billion-dollar-gram/) | 用统一尺度的面积让大数量产生视觉冲击。 | 适合量级浏览，细小差距用直接标值。 | 几块最有意义的面积与直标 | 方块面积成比例，边长不成比例 |

## 分布、例外与不确定性

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 031 | [The Radius Gap](https://www.visualcinnamon.com/portfolio/radius-gap/) | 用密度等高线让两个群体和中间空隙都显形。 | 均值不足以说明分布时，先找聚集与缺口。 | 两个密度区与中间缺口 | 平滑参数会改变缺口观感 |
| 032 | [The Baby Spike](https://www.visualcinnamon.com/portfolio/baby-spike/) | 把出生时间的局部峰值变成文章中的主要发现。 | 细粒度时点数据保留尖峰，谨慎平滑。 | 关键峰值、前后基线与具体时间 | 峰尖并不说明全年总量很高 |
| 033 | [Ridgeline 分布样例](https://www.data-to-viz.com/graph/ridgeline.html) | 将多组密度沿同一横轴错落排列。 | 扫形状时统一尺度，标明密度不是样本量。 | 三组分布、共享轴、重叠边界 | 峰高反映密度，未必代表样本多 |
| 034 | [Violin Plot 分布样例](https://www.data-to-viz.com/graph/violin.html) | 通过厚薄呈现密度，宽处提示常见值。 | 小样本补原始散点与组样本量。 | 关键分位数、组样本量 | 小样本经平滑可能呈现虚假双峰 |
| 035 | [二维密度示例](https://www.data-to-viz.com/graph/density2d.html) | 用等高线暴露散点重叠后的聚集。 | 保留原始点或标清带宽与平滑方法。 | 主等高线和少量原始点 | 等高线边界不是硬性分类线 |
| 036 | [Heatmap 矩阵示例](https://www.data-to-viz.com/graph/heatmap.html) | 同尺寸格子给颜色编码留下稳定结构。 | 排序、颜色刻度和缺失值样式同等重要。 | 行列短名、色标和缺失样式 | 颜色深浅不能跨不同色标对比 |
| 037 | [Sizing Chaos](https://pudding.cool/2026/02/womens-sizing/) | 由典型人物推进到年龄与人群差异。 | 用一个中位数或个案开场，再显示分布范围。 | 一个典型人物与人群分布 | 中位体型不能代表每种体型 |
| 038 | [生日效应](https://pudding.cool/2025/04/birthday-effect/) | 让一个特殊日期与周边日期一起进入比较。 | 异常值要有邻近基线，避免只报相对变化。 | 焦点日期与相邻基准 | 相对变化很大时绝对差可能很小 |
| 039 | [A Love Story](https://pudding.cool/2026/06/love-story/) | 保留参与者纵向轨迹以及调查波次的匹配条件。 | 从个人经历过渡到队列，用配对口径限定样本。 | 一人轨迹、三轮调查和样本限定 | 筛出三轮都参与的人会影响代表性 |
| 040 | [Berkeley Earth 2024 · 全球温度图](https://berkeleyearth.org/global-temperature-report-for-2024/) | 在长趋势中说明本年位置与测量口径。 | 纪录型标题同时交代基准、数据集及估计差异。 | 年份、基准期和关键温差 | 温度异常不能直接读成绝对温度 |

## 关系、关联与网络

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 041 | [Royal Constellations](https://www.visualcinnamon.com/portfolio/royal-constellations/) | 大网络平时给结构，悬停后才突出一条联系。 | 依赖图高亮选定节点、邻居与路径，保留其他节点作背景。 | 一条路径、起讫点和关系图例 | 节点位置和边长不代表亲疏距离 |
| 042 | [Searching for Birds](https://www.visualcinnamon.com/portfolio/searching-for-birds/) | 把数据分析、物种插图和探索界面编成一体。 | 分类检索提供可识别对象，并保留一致的数据编码。 | 主物种、图例及一幅视图 | 搜索出现频次不等于鸟类实际数量 |
| 043 | [Small World of Words](https://www.visualcinnamon.com/portfolio/small-world-of-words/) | 把词与词之间的联想关系当成浏览对象。 | 语义网络支持实体查找，聚类用途和含义要讲清。 | 一个中心词和邻接关系 | 词联想受语言与样本群体影响 |
| 044 | [UNESCO Intangible Cultural Heritage](https://www.visualcinnamon.com/portfolio/intangible-cultural-heritage/) | 同批文化遗产用不同视图回答不同关系问题。 | 多视图围绕同一实体联动，每个视图只承担一种关系。 | 一个关系视图和一个遗产实例 | 不同视图可能使用不同关系定义 |
| 045 | [RéciTAC](https://www.visualcinnamon.com/portfolio/recitac/) | 用项目合作网络表达研究者间的联系。 | 先明确连边依据和分析粒度，再做视觉聚焦。 | 一个团队的局部子网 | 同属一个项目与直接合作需区分 |
| 046 | [GitHub Top Contributor Network](https://www.visualcinnamon.com/portfolio/orca-top-contributors/) | 把贡献者与项目联系组织成可读的关系空间。 | 复杂图优先让人追踪某个节点的局部关系。 | 一个贡献者及相关项目 | 网络中心性不等于贡献质量 |
| 047 | [Kantar MotiveMix](https://www.visualcinnamon.com/portfolio/kantar-motivemix/) | 在空间与态度维度之间切换观察相似性。 | 把相似度和地理距离的编码解释清楚。 | 两个维度与几个代表地区 | 地理接近不等于态度相似 |
| 048 | [CO₂ 与人均 GDP](https://ourworldindata.org/grapher/co2-emissions-vs-gdp) | 在同一散点空间审视两项人均指标。 | 保留轴单位、对数读法与关键例外，避免因果暗示。 | 两轴单位、对数注明、典型例外 | 相关关系本身无法说明因果 |
| 049 | [Best in Show](https://informationisbeautiful.net/visualizations/best-in-show-whats-the-top-data-dog/) | 把两个评价维度放进一个可扫读的定位空间。 | 二维选型先定义评分；主观指标给方法说明。 | 两轴名称、一两个取舍实例 | 综合分数会折叠偏好差异 |
| 050 | [平行坐标示例](https://www.data-to-viz.com/graph/parallel.html) | 借高亮追踪一条多指标记录穿过各轴。 | 轴排序影响观感，清楚说明归一化和正负方向。 | 少数轴、量纲和选中轨迹 | 改轴顺序会改变看见的相邻关系 |

## 流向、迁移与路径

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 051 | [OECD Global Plastics Outlook](https://www.visualcinnamon.com/portfolio/oecd-global-plastics-outlook/) | 为两期的塑料流向保持可对照的结构。 | 前后桑基图沿用节点顺序与比例口径。 | 两期节点对齐、主路径、合计 | 为比较流宽，两期必须同尺度 |
| 052 | [Bussed Out](https://www.visualcinnamon.com/portfolio/bussed-out/) | 把跨地迁移和具体人物经历放在一个调查叙事里。 | 宏观流量可用个案引导，但个案与总体证据要区分。 | 一条代表路线和总体体量 | 一个个案无法代表项目全部结果 |
| 053 | [Visualizing Millions of People on the Move](https://www.visualcinnamon.com/portfolio/urbanization/) | 用视觉路径组织跨地域的大规模人口移动。 | 同时交代起讫、方向和统计期间。 | 起讫区域、时间与迁移量 | 净迁移与双向总迁移需区分 |
| 054 | [Switching Between Phone Brands](https://www.visualcinnamon.com/portfolio/phone-brand-switching/) | 围绕品牌之间的实际切换来表达移动。 | 留存、流失和去向用成对转移数据。 | 两个品牌与对角留存 | 换入比例与换出比例的分母不同 |
| 055 | [Preferential Polling](https://www.visualcinnamon.com/portfolio/swayable-preferential-polling/) | 把排名投票中的多轮转移变成可追踪步骤。 | 需要解释重分配时保留每一阶段、规则和合计。 | 一轮转移、规则及最终结果 | 次序映射是模拟规则下的结果 |
| 056 | [The Words in the Lord of the Rings](https://www.visualcinnamon.com/portfolio/words-lord-of-the-rings/) | 用弦线让人物与发言场景的连接可追踪。 | 先高亮选中实体的关系，再允许浏览其他路径。 | 一个人物、一个场景和线义 | 发言字数并不等于角色重要性 |
| 057 | [Sankey Diagram 示例](https://www.data-to-viz.com/graph/sankey.html) | 连线宽度呈现各路径数量。 | 验证入口、出口和损失项能对账。 | 主路径、单位及进出合计 | 流量守恒不表示跟踪了相同个体 |
| 058 | [Chord Diagram 示例](https://www.data-to-viz.com/graph/chord.html) | 在共享的环形结构中表现多方关系。 | 类别较少时用作概览，精确查数可以配矩阵。 | 少量节点、方向和最大联系 | 带宽代表权重，弧长是否编码须说明 |
| 059 | [A Day in the Life of Americans](https://flowingdata.com/2015/12/15/a-day-in-the-life-of-americans/) | 让代表模拟个体的点随时间迁移到不同活动。 | 明确粒子单位、仿真假设与静态输出。 | 两个时点对照、模拟说明 | 仿真人物轨迹不是观察到的个人连续记录 |
| 060 | [Landscape of Power Flows](https://www.visualcinnamon.com/portfolio/landscape-of-power-flows/) | 把电网中的流向视为需要辨识的网络。 | 网络路径表达连接与方向，布局不代表距离时要说明。 | 选中电网走廊和方向图例 | 地理距离与电网拓扑关系要区分 |

## 地理位置与空间感

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 061 | [The True Size Of…](https://thetruesize.com/) | 用拖动对照让投影对面积的影响变得可体验。 | 地图切换前后明确正在比较的空间属性。 | 拖拽前后并排和比例尺 | 二维投影无法同时保真全部空间属性 |
| 062 | [Human Terrain](https://pudding.cool/2018/10/city_3d/) | 让人口密度成为地表上的高度。 | 用空间立体做第一印象，精确比较配标尺和数值。 | 一个地区截面、标尺和视角 | 遮挡与透视会改变对高度的判断 |
| 063 | [earth.nullschool.net](https://earth.nullschool.net/) | 通过流线让方向和空间场共同可见。 | 风、流量或速度场说明动效与数据单位。 | 一张流场截图、时刻和图例 | 流线展示的方向、速度不等于个体轨迹 |
| 064 | [挪威旅行地图](https://www.visualcinnamon.com/portfolio/map-norway/) | 把地形背景与步行、停留和位置记录用不同符号分层。 | 地图主层只保留与问题直接相关的对象。 | 核心路径和几个定位点 | 个人定位记录有遗漏和采样偏差 |
| 065 | [A Giant Map of the World](https://www.visualcinnamon.com/portfolio/worldmap/) | 用大画幅地图支持整体浏览和局部查找。 | 规划远看与近看的不同标签层级。 | 一个总览与一个局部放大 | 地图比例变化会改变标记密度 |
| 066 | [NYC’s Urban Textscape](https://pudding.cool/2025/07/street-view/) | 把街景可见文字转为空间检索入口。 | 探索式地图用搜索结果联系点位和观察记录。 | 一个词、几个位置和原图例证 | 街景覆盖率会影响搜到的文字数量 |
| 067 | [Imaging the Entire Earth, Every Day](https://www.visualcinnamon.com/portfolio/planet-globe/) | 用地球作为卫星覆盖这个主题的天然视图。 | 覆盖率视图保留空间范围与观测频率说明。 | 覆盖区、时间窗口和观测定义 | 覆盖频率不等于地面实际无云影像数量 |
| 068 | [Happy Map](https://pudding.cool/2026/02/happy-map/) | 把幸福事件变成可浏览的地理样本。 | 样本地图应保留代表性说明，避免把记录密度当成总体密度。 | 一个地理聚集与样本注 | 上报密度受采样分布影响 |
| 069 | [分级设色地图配色样例](https://www.datawrapper.de/blog/how-to-choose-a-color-palette-for-choropleth-maps) | 让视觉深浅与数值顺序一致。 | 给空值独立样式，避免把它画成最低值。 | 代表地区、区间色标和缺失样式 | 地理面积大不意味着数据权重大 |
| 070 | [Dollar Street](https://www.gapminder.org/dollar-street) | 用家庭照片让同一生活维度在不同收入水平上可比较。 | 地图并非唯一入口，按收入或其他有效变量重排内容。 | 两个收入位置、同类物件照片 | 示例家庭不是该收入段的统计平均 |

## 编辑叙事与可核查证据

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 071 | [In Pursuit of Democracy](https://pudding.cool/2025/11/democracy/) | 点选时间图中的记录，阅读对应年度精选发言。 | 标记连接来源或样本，注明精选范围。 | 总趋势和带出处的一段引文 | 精选发言不是全体观点分布 |
| 072 | [Women’s Pockets Are Inferior](https://pudding.cool/2018/08/pockets/) | 直接叠放口袋轮廓，并让读者测试物品能否放入。 | 实体形状承担解释，保留尺寸与测试口径。 | 同尺度轮廓、同一物件及命中规则 | 平铺几何可容纳不等同穿着体验 |
| 073 | [A History of Menus is a Menu of History](https://pudding.cool/2026/06/menu-story/) | 从菜单原件进入更长的饮食史。 | 证据先具象化，再连接总体趋势。 | 一张菜单与对应时代指标 | 存世档案受采集和保存偏差影响 |
| 074 | [5,000 Restaurant Menus](https://pudding.cool/2026/06/menu-collection/) | 用档案浏览界面让读者查看单份菜单。 | 高层统计旁提供可检索原始记录。 | 一个筛选条件与一张原菜单 | 档案检索结果不能代表全部当年餐厅 |
| 075 | [Bears Will Be Boys](https://pudding.cool/2025/07/kids-books/) | 儿童书中的原始视觉语汇参与叙事。 | 素材增强主题识别，编码结论仍来自数据。 | 关键比例与原书角色对照 | 角色分类规则和抽取样本影响结论 |
| 076 | [Film Dialogue by Gender](https://pudding.cool/2017/03/film-dialogue/) | 在汇总发现和影片级明细之间建立连接。 | 比例结论绑定可检查的分析单位与分组。 | 主要差异、影片范围与一句证据 | 对白行数并不是角色数量或银幕时长 |
| 077 | [Asian Misrepresentation](https://pudding.cool/2025/05/aapi-casting/) | 围绕实际人群与银幕再现的落差提出可视对照。 | 基准人口与样本构成同屏交代。 | 人口基准、银幕样本及对照比例 | 基准年份和地域需与影视样本匹配 |
| 078 | [How Musicals Use Motifs](https://pudding.cool/2025/12/motifs/) | 用音乐片段和屏幕提示帮助读者识别主题复现。 | 声音属于证据时保留文字或视觉替代。 | 一段复现时间轴及简短听觉说明 | 作品里的重复不自动证明作者意图 |
| 079 | [Walkachusetts](https://pudding.cool/2025/10/walk/) | 路线、观察和故事同步向前推进。 | 只在叙事节点要求读者切换注意力。 | 一段路径和有数据支持的节点 | 个人路线的观察不代表所有路段 |
| 080 | [30 Minutes with a Stranger](https://pudding.cool/2025/06/hello-stranger/) | 把真实对话与随时间变化的观察放在一起。 | 时间轴联动原始材料时明确时间对齐方式。 | 一段时间轴、一个同步证据和样本口径 | 情绪读数的测量方法影响解释 |

## 交互、模拟与视图切换

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 081 | [Dicing an Onion](https://pudding.cool/2025/08/onions/) | 拖动切数并切到拆解视图，形状和离散度同时变化。 | 交互每次改变可说明的输入，并联动图形和读数。 | 两种切法并列、相同切数、离散指标 | 理想几何下的最优结果取决于模型 |
| 082 | [Gapminder World Health Chart](https://www.gapminder.org/fw/world-health-chart/) | 播放时间，让散点中的国家轨迹逐步可见。 | 动画适合迁移，保留可暂停的时间控制。 | 两期、少数国家和泡泡面积单位 | 时间轨迹的关联不等于因果 |
| 083 | [Why the Super Rich Are Inevitable](https://pudding.cool/2022/12/yard-sale/) | 用可操控模拟引导读者观察结果如何形成。 | 明确参数、随机性、初值与结果代表的范围。 | 固定假设的一对模拟画面 | 单次模拟结果受随机抽样影响 |
| 084 | [Washington Post 扁平曲线模拟](https://www.washingtonpost.com/graphics/2020/world/corona-simulator/) | 相邻模拟让读者比较不同设定的结果模式。 | 对照场景沿用视觉口径，并区分单次随机轨迹与总体结论。 | 同一时点的两种设定与结果 | 简化模拟只是演示机制 |
| 085 | [The Largest Vocabulary in Hip Hop](https://pudding.cool/2017/02/vocabulary/) | 在统一比较尺度上按兴趣定位特定艺人。 | 排行榜给搜索或点选入口，并交代样本窗口。 | 主要艺人与统一词数窗口 | 曲库、歌词抽样和词形规则影响排名 |
| 086 | [How People Like You Spend Their Time](https://flowingdata.com/2016/12/06/how-people-like-you-spend-their-time/) | 让读者选择与自己相关的分组看时间使用。 | 分群控件改变明确口径，并同步更新读数和样本说明。 | 两组的同一活动和共同时间尺度 | 人群均值不是一位典型个体的日程 |
| 087 | [CFR Global Inflation Tracker](https://www.cfr.org/articles/global-inflation-tracker) | 让读者按经济体与时期探索价格变化。 | 筛选首先服务可复用的比较问题。 | 两经济体、同一频率、基期说明 | 指数、同比和环比容易混读 |
| 088 | [Population & Demography Explorer](https://ourworldindata.org/explorers/population-and-demography) | 把指标、国家、时间组织为可组合的探索入口。 | 避免控件改变口径后，标题和单位仍留在原状态。 | 固定指标、地区、年度与单位 | 切换指标后须同步检查分母与单位 |
| 089 | [Reuters Japan Population](https://graphics.thomsonreuters.com/14/japan_pop/index.html) | 让读者在不同年份的年龄结构之间比较。 | 人口或用户队列的年龄结构切换要保持年龄带一致。 | 两个年份同龄带、人数或份额单位 | 不同年代的结构与绝对人口应区分 |
| 090 | [World’s Biggest Data Breaches](https://informationisbeautiful.net/visualizations/worlds-biggest-data-breaches-hacks/) | 通过气泡集合提供规模浏览，再配合筛选看细节。 | 面积编码适合找大项，精确记录量放在直接标签或详情。 | 最大几例、日期、气泡面积单位 | 报道数量受披露规则与覆盖范围影响 |

## 数据艺术与静态构图

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 091 | [Film Flowers](https://sxywu.github.io/filmflowers/) | 用花瓣形状、数量与整花大小映射电影属性。 | 自定义图形每个通道写明定义，精确排名另用位置。 | 少量花形与一套可读图例 | 花瓣数、颜色和花大小分别编码独立变量 |
| 092 | [Cycle of Many](https://flowingdata.com/2021/08/25/cycle-of-many/) | 24 小时成圆，环表示活动，点密度表示对应份额。 | 当时间本身有周期时，环形构图才有解释价值。 | 少数活动环、时钟方向和图例 | 点的密度对应份额，不能直接读人数 |
| 093 | [Gold Record with Data Art](https://www.visualcinnamon.com/portfolio/sony-music-data-art/) | 为展陈距离设计完整画面与近看的数据细节。 | 海报先定远看主形，再排可供近读的内容。 | 一个主体和一块细节放大 | 海报图形先确认哪些装饰不编码数据 |
| 094 | [Top 39 Actors](https://www.visualcinnamon.com/portfolio/graffu-actors/) | 用爆米花等电影语汇表达电影记录。 | 图形隐喻贴合题材时才有辨识度，逐条验证标记映射。 | 几部电影和标记含义 | 主题符号会让读者误认为所有特征都编码 |
| 095 | [Figures in the Sky](https://www.visualcinnamon.com/portfolio/figures-in-the-stars/) | 让不同文化在同一片星空上有可比的轮廓。 | 共同坐标承载多种解释，避免把叙事差异混同数据差异。 | 同一星图下选择两种文化 | 历史资料覆盖不均会影响比较 |
| 096 | [An Ode to Cardcaptor Sakura](https://www.visualcinnamon.com/portfolio/cardcaptor-sakura/) | 让角色、情节和作品视觉语言互相呼应。 | 编辑长图先定叙事层和数据层，再定装饰层。 | 几个角色或事件和映射图例 | 主题造型可能遮住精确读数 |
| 097 | [The Top 2000 ❤ the 70s & 80s](https://www.visualcinnamon.com/portfolio/top2000/) | 用年代排布观察歌曲集中期，少数艺人突出为识别线索。 | 为密集时间点加主题符号，同时保留可读尺度。 | 主要年代和一两位高亮艺人 | 上榜歌曲反映榜单来源的偏好 |
| 098 | [Meet the Neighbors](https://www.visualcinnamon.com/portfolio/exoplanet-neighbors/) | 把天体与行星系统组织成有层级的静态图版。 | 报告跨尺度时明确每块画面对应的空间尺度。 | 两个尺度面板与各自标尺 | 画面间距不能直接当作真实星际距离 |
| 099 | [Space Wars](https://www.visualcinnamon.com/portfolio/space-wars/) | 把卫星保留为独立可见的点，整体仍显示结构。 | 当单条记录本身重要时，分组与注释优先于完全聚合。 | 关键轨道分组、点单位和年份 | 每个点的大小不一定映射卫星实体尺寸 |
| 100 | [Olympic Feathers](https://www.visualcinnamon.com/portfolio/olympic-feathers/) | 用可辨识的重复形展示不同赛项的奖牌分布。 | 形成系列时保持标记语义稳定，并标赛事时间及分组。 | 少数赛项、年代和奖牌图例 | 赛项数量或参赛机会不同会影响总奖牌 |
## 新增案例怎么选

- 有分支方案时先看 101。有可校准的预测分布时再看 102–105。106 用于设计可调假设的情景对照。
- 做交互探索时看 107–110。需要缩成半页 PPT 时，参考 111–113 和每个案例的精简提示。
- 复查图表时按 114–116 的方式保留一组对照。做中文稿时用 117–120 检查长标题、数字单位、标签、注释和手机宽度。

## 概率、预测与决策路径

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 101 | [512 Paths to the White House · 作者解析](https://source.opennews.org/articles/nyts-512-paths-white-house/) | 选定部分州的结果，剩余胜选路径随之收窄。 | 把路径筛选和结局概率分别编码。 | 一个起点、两条分支和最终结局 | 可行路径的数量不等于胜率 |
| 102 | [英格兰银行 · CPI 预测扇形图](https://www.bankofengland.co.uk/monetary-policy-report/2026/november-2026) | 用不同深浅的概率带表达随时间变化的预测分布。 | 对比实际值与预测，同时标注区间覆盖率和假设。 | 历史线、中央预测和一到两层区间 | 扇形不是承诺范围，区间外仍可能发生 |
| 103 | [ggdist · 分位点阵](https://mjskay.github.io/ggdist/articles/dotsinterval.html) | 用等概率权重的点表示分布。 | 保留点数和阈值标线，让超阈值概率可数。 | 一条阈值、等权点和概率直标 | 这些点表示分布的离散化，不属于原始样本 |
| 104 | [UW IDL · 假想结果图](https://idl.uw.edu/papers/hops-trends) | 对照静态多条轨迹、误差线和随帧切换的模型抽样。 | 看可能结果是怎么变化的，静态版保留抽样集合。 | 少量示意轨迹、基准和模型说明 | 动画帧是不同的可能结果，不是时间推进 |
| 105 | [UW IDL · 公交到站不确定性](https://idl.uw.edu/papers/uncertainty-bus) | 从手机上判断到站时间超过自己到站时间的概率。 | 把问题写成与行动直接相关的阈值。 | 一个行动阈值、一张点阵及概率标注 | 需区分平均到站时间和赶上车的概率 |
| 106 | [En-ROADS · 全球气候模拟器](https://www.climateinteractive.org/en-roads/) | 调整政策假设时，图与结果同时更新。 | 用固定基线对照情景，交代用户改动了哪些输入。 | 基准与一个政策情景、改动项 | 模型情景不自带发生概率 |

## 联动探索与逐层展开

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 107 | [Observable · 企鹅散点与直方图](https://old.observablehq.com/blog/linked-brushing) | 框选喙的尺寸，一起看对应体重分布。 | 保留全体分布作为参照并显示选中样本数。 | 全体和被框选人群的同轴对照 | 高亮数量变化也受框选的样本量影响 |
| 108 | [Vega · 航班多维筛选](https://vega.github.io/vega/examples/crossfilter-flights/) | 时间、延误和距离各有一个可拖动的筛选视图。 | 让筛选范围、重置入口和各面板状态都可见。 | 一组筛选条件及最相关的分布 | 多个筛选条件取交集，读数是筛选后的样本 |
| 109 | [Vega-Lite · 高亮式交叉筛选](https://vega.github.io/vega-lite/examples/interactive_layered_crossfilter.html) | 在总分布上保留选中子集，未选数据变成背景。 | 比较选中样本和全体时优先考虑保留背景。 | 两层直方图、共同分箱及样本数 | 绝对计数较少不意味着比例更低 |
| 110 | [英国统计局 · 你所在地区的人口变化](https://www.ons.gov.uk/peoplepopulationandcommunity/populationandmigration/populationestimates/articles/howthepopulationchangedwhereyoulivecensus2021/2022-06-28) | 先选择地区，再阅读按该地区组织的人口故事。 | 沿用同一叙事结构，用地名与基准定位读者。 | 一个地区、全国基准和普查年份 | 辖区边界与人口基准会改变比较结果 |

## 静态与交互交付

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 111 | [BBC · 新闻图表样式](https://bbc.github.io/rcookbook/) | 标题、字号、留白和来源随不同图形保持一致。 | 先定可重复的版式，再换标记与图形。 | 标题、主图、直标及来源 | 应用样式之后仍须重新检查读数与口径 |
| 112 | [Datawrapper · 可访问的交互图](https://www.datawrapper.de/blog/better-accessibility-for-datawrapper-visualizations) | 把图表描述与色觉检查纳入设计。 | 让关键状态有文字或形状线索，验证键盘操作。 | 直标、非颜色线索和短图注 | 仅凭颜色区分会丢失可读信息 |
| 113 | [Datawrapper · 图中文字设计](https://www.datawrapper.de/blog/text-in-data-visualizations) | 对照图例、直标和就地旁注在画面里的距离。 | 给 PPT 与手机分别实测文字长度，保留最关键读数。 | 一句结论、一个就地注释及单位 | 注释离证据太远容易被归到相邻系列 |

## 误读与修正

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 114 | [Distill · 如何读 t-SNE](https://distill.pub/2016/misread-tsne/) | 让同一批数据在不同参数下并排呈现。 | 展示参数敏感性，再判断哪些结构可解释。 | 两个参数结果及固定的数据说明 | 簇的面积和距离不能直接当作原空间关系 |
| 115 | [Datawrapper · 折线图中的缺失值](https://www.datawrapper.de/academy/missing-data-in-line-charts) | 对照断线、延伸和显式标注缺失的设计。 | 说明断档位置及数据是否经过插补。 | 带断口的线、缺失日期和一句说明 | 空档不代表 0，也不证明平滑延续 |
| 116 | [Spurious Correlations](https://www.tylervigen.com/spurious-correlations) | 让看似贴合、实则缺少机制证据的序列并排。 | 结论中区分视觉同向、统计相关与因果证据。 | 两个原始量纲、时间范围和反例 | 双轴缩放可以让无关走势看起来高度吻合 |

## 中文编辑设计

| 编号 | 原作或样图 | 观察什么 | 怎么用 | 半页 PPT 保留什么 | 容易误读什么 |
|---|---|---|---|---|---|
| 117 | [澎湃美数课 · 春运高铁好买指数](https://www.thepaper.cn/newsDetail_forward_26181341) | 先定义指数，再按出发城市讲跨城市对比。 | 中文长地名和方法分层，给复合指标一个简短释义。 | 一个出发城市、代表路线和指数口径 | 估算的好买指数不等于实际购票成功率 |
| 118 | [澎湃美数课 · 中国人口 74 年图谱](https://www.thepaper.cn/newsDetail_forward_25793167) | 把人口长周期放进面向移动端的中文图文叙事。 | 把读数、阶段和注释排出清晰层次。 | 一条时间主轴、一组转折及人数单位 | 人口总量、年龄构成与增量含义不同 |
| 119 | [澎湃美数课 · 15 年列车运行图](https://www.thepaper.cn/newsDetail_forward_32482558) | 把不同时期的运行图放进同一个春运变化故事。 | 保留可比的时间定位与列车类别。 | 两个年份、相同范围及班次数口径 | 计划班次并不等于实际客运量 |
| 120 | [澎湃美数课 · 春节旅游成绩单](https://www.thepaper.cn/newsDetail_forward_26181344) | 用人数、支出与节期的指标层次组织中文长图。 | 大字讲总量，小字明确人次、元和统计窗口。 | 一个金额、出游人次与可比口径 | 假期天数不同会改变总量，同比需核对口径 |
