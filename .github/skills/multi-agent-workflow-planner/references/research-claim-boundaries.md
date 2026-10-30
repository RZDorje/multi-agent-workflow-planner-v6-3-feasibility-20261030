# Research Claim Boundaries / 研究主张边界

Read this reference only when a task asks about agent count, topology, collaboration effectiveness, or research evidence. These selected sources do not establish a universal number of agents. Report each result with its task, model/version, topology, budget, metric, and whether coordinators, tools, repeated samples, or other units are counted. “Agent” can refer to different units; do not treat those counts as interchangeable.

仅当任务涉及 Agent 数量、拓扑、协作效能或研究证据时读取本参考资料。以下精选来源不能证明存在通用 Agent 数量。报告结果时应同时写明任务、模型/版本、拓扑、预算、指标，以及是否计入协调者、工具、重复样本或其他单位。“Agent”可能指不同计数单位，不应混为一谈。

For every entry, the date field reflects the cited page or version record—not an internal note. **Access date for every entry: 2026-10-30.**

每个条目的日期字段均来自所引页面或版本记录，而非内部备注。**所有条目的查阅日期：2026-10-30。**

## Contents / 目录

- [Vendor engineering guidance / 厂商工程指南](#vendor-engineering-guidance--厂商工程指南)
- [Vendor-reported systems and experiments / 厂商报告的系统与实验](#vendor-reported-systems-and-experiments--厂商报告的系统与实验)
- [Google Research, Nature, and arXiv: keep versions separate / Google Research、Nature 与 arXiv：分开版本](#google-research-nature-and-arxiv-keep-versions-separate--google-researchnature-与-arxiv分开版本)
- [Topology-specific papers and repeated sampling / 特定拓扑论文与重复采样](#topology-specific-papers-and-repeated-sampling--特定拓扑论文与重复采样)
- [Safe planning conclusions / 稳妥的规划结论](#safe-planning-conclusions--稳妥的规划结论)

## Vendor engineering guidance / 厂商工程指南

### OpenAI — building-agent guide / OpenAI——Agent 构建指南

- **Page title / 页面原文标题:** EN: “A practical guide to building agents” — [OpenAI guide](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/). 中文：页面原文标题为 “A practical guide to building agents”——[OpenAI 指南](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/)。
- **Source type / 来源类型:** EN: OpenAI first-party business/engineering guide; vendor guidance, not an independent benchmark. 中文：OpenAI 第一方业务/工程指南；属于厂商指导，不是独立基准。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Published 2026-01-15; no version shown. 中文：发布于 2026-01-15；未标版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The guide recommends first strengthening a capable single-agent workflow, then considering multiple agents when complex instructions, branching, or overlapping tools make the single-agent approach difficult. It describes manager/tool-call and decentralized handoff patterns. 中文：指南建议先完善有竞争力的单 Agent 流程；当复杂指令、分支或工具重叠令单 Agent 难以胜任时，再考虑使用多个 Agent。指南介绍 manager/tool-call 和 decentralized handoff 模式。
- **Does not establish / 来源不能证明:** EN: The guide's discussion of more than 15 well-differentiated tools versus fewer than 10 overlapping tools is implementation guidance/anecdote, not a universal threshold, controlled benchmark, or proof that any agent count is optimal. 中文：指南中“超过 15 个清晰区分的工具”与“少于 10 个彼此重叠的工具”的讨论属于实现经验/示例，不是通用阈值、受控基准，也不能证明某个 Agent 数量最优。

## Vendor-reported systems and experiments / 厂商报告的系统与实验

### Anthropic — “How we built our multi-agent research system” / Anthropic——“How we built our multi-agent research system”

- **Page title / 页面原文标题:** EN: “How we built our multi-agent research system” — [Anthropic Engineering](https://www.anthropic.com/research/multi-agent-research-system). 中文：页面原文标题为 “How we built our multi-agent research system”——[Anthropic Engineering](https://www.anthropic.com/research/multi-agent-research-system)。
- **Source type / 来源类型:** EN: Official Anthropic Engineering web article and vendor system/evaluation report. 中文：Anthropic 官方 Engineering 网页文章及厂商系统/评测报告。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Published 2025-06-13; no separate update or version shown. 中文：发布于 2025-06-13；未标独立更新日期或版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: Anthropic describes an orchestrator-worker research system and reports that, in its internal research evaluation, a Claude Opus 4 lead with Claude Sonnet 4 workers scored 90.2% higher than a single Claude Opus 4 baseline. The article also reports multi-agent research using about 15 times as many tokens as ordinary chat in its described data. 中文：Anthropic 描述了 orchestrator-worker 研究系统，并报告在其内部研究评测中，Claude Opus 4 lead 搭配 Claude Sonnet 4 workers 的得分比单独 Claude Opus 4 基线高 90.2%。文章还报告，在其所述数据中，多 Agent 研究约使用普通聊天 15 倍的 token。
- **Does not establish / 来源不能证明:** EN: These are vendor-reported results for the named system and evaluation, not independent replication or a general 90.2% improvement. The article does not establish that multi-agent systems outperform on tasks needing shared context or substantial inter-agent dependencies; preserve its cost and task-fit caveats. 中文：这些是厂商针对特定系统和评测报告的结果，不是独立复现，也不是普遍提升 90.2% 的证据。文章不能证明多 Agent 系统在需要共享上下文或大量 Agent 间依赖的任务上更好；应保留其成本和任务适配限制。

### Anthropic — “Patterns and problems in emerging multiagent systems” / Anthropic——“Patterns and problems in emerging multiagent systems”

- **Page title / 页面原文标题:** EN: “Patterns and problems in emerging multiagent systems” — [Anthropic Research](https://www.anthropic.com/research/multiagent-systems). 中文：页面原文标题为 “Patterns and problems in emerging multiagent systems”——[Anthropic Research](https://www.anthropic.com/research/multiagent-systems)。
- **Source type / 来源类型:** EN: Official Anthropic Research / Frontier Red Team web article and vendor-reported experiment report. 中文：Anthropic 官方 Research / Frontier Red Team 网页文章及厂商报告的实验结果。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Published 2026-08-13; no separate update or version shown. 中文：发布于 2026-08-13；未标独立更新日期或版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The article reports scenario-specific vulnerability-search and game-building experiments. In the described vulnerability setup, Anthropic reports 266 findings from a coordinating swarm over 27 million tokens versus 21 findings from independent parallel agents over 6.5 million tokens; it notes roughly half of the swarm findings were outside the directories targeted by the independent agents. The article says the core-directory comparison was roughly comparable in tokens per vulnerability and reports poor game outputs in a separate simulation. 中文：文章报告了特定场景下的漏洞搜索与游戏开发实验。在所述漏洞实验中，Anthropic 报告协调 swarm 使用 2,700 万 tokens 得到 266 项结果，独立并行 agents 使用 650 万 tokens 得到 21 项结果；文章指出 swarm 结果中约一半位于独立 agents 搜索目标目录之外。文章称仅比较核心目录时，每项漏洞的 token 成本大致相当，并报告另一项模拟中的游戏产物质量较差。
- **Does not establish / 来源不能证明:** EN: These vendor-described scenarios do not establish real-world failure rates or general superiority. The comparison differs in token spend and search scope; the page itself qualifies the comparison. It is not independent replication or an external audit. 中文：这些厂商所述场景不能证明现实世界失败率或普遍优势。对照组在 token 花费和搜索范围上不同；页面本身也对比较作了限定。该报告不是独立复现或外部审计。

## Google Research, Nature, and arXiv: keep versions separate / Google Research、Nature 与 arXiv：分开版本

### Google Research blog — early report / Google Research 博客——早期报告

- **Page title / 页面原文标题:** EN: “Towards a science of scaling agent systems: When and why agent systems work” — [Google Research](https://research.google/blog/towards-a-science-of-scaling-agent-systems-when-and-why-agent-systems-work/). 中文：页面原文标题为 “Towards a science of scaling agent systems: When and why agent systems work”——[Google Research](https://research.google/blog/towards-a-science-of-scaling-agent-systems-when-and-why-agent-systems-work/)。
- **Source type / 来源类型:** EN: Official Google Research blog post. 中文：Google Research 官方博客文章。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Published 2026-01-28; no page version shown. 中文：发布于 2026-01-28；未标页面版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The early blog report describes 180 agent configurations across four benchmarks. It reports task-dependent outcomes, including +80.9% on Finance-Agent and -39% to -70% on sequential PlanCraft in its described settings; the blog reports R²=0.513. 中文：这篇早期博客报告描述了 180 种 Agent 配置和四个基准。文章报告效果因任务而异，在其所述设置中，Finance-Agent 为 +80.9%，顺序 PlanCraft 为 -39% 至 -70%；博客报告 R²=0.513。
- **Does not establish / 来源不能证明:** EN: These early blog values are not universal task effects. Do not replace them with or merge them into the later Nature version or arXiv v3 counts and values. The page does not establish the later version's 260 configurations or six benchmarks. 中文：这些早期博客数据不是普遍任务效果。不得以之后 Nature 版本或 arXiv v3 的计数和数值替换它们，也不得将其合并。该页不能证明后续版本的 260 种配置或六个基准。

### Nature Machine Intelligence — version of record / Nature Machine Intelligence——正式出版版本

- **Page title / 页面原文标题:** EN: “Capable language models can outgrow the benefits of collaboration” — [Nature Machine Intelligence](https://www.nature.com/articles/s42256-026-01268-y). 中文：页面原文标题为 “Capable language models can outgrow the benefits of collaboration”——[Nature Machine Intelligence](https://www.nature.com/articles/s42256-026-01268-y)。
- **Source type / 来源类型:** EN: Peer-reviewed journal article, version of record. 中文：同行评审期刊论文，正式出版版本。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Published and version of record 2026-07-24; no separate revision number shown. 中文：于 2026-07-24 发布并成为正式版本；未列独立修订号。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The article reports experiments across 260 configurations, six benchmarks, five architectures, and three model families. The abstract reports task-specific results including +80.8% for financial reasoning and -70.0% for sequential planning relative to single-agent baselines in the tested settings. In its SWE-bench Verified setup, “seven” refers to tools, not agents. 中文：论文报告了 260 种配置、六个基准、五种架构和三个模型家族的实验。摘要报告相对于单 Agent 基线的任务特定结果，包括所测金融推理 +80.8%、顺序规划 -70.0%。在 SWE-bench Verified 设置中，“七”指工具数量，不是 Agent 数量。
- **Does not establish / 来源不能证明:** EN: Findings are bounded by the tested tasks, models, architectures, and budgets; an empirical selection heuristic is not a universal scaling law. Do not mix this version's counts/results with the early Google blog or a separately versioned preprint. 中文：结论受测试任务、模型、架构和预算限制；经验性选择启发式不是普遍缩放定律。不得将该版本的计数/结果与 Google 早期博客或单独编号的预印本混合。

### arXiv — version 3 preprint / arXiv——v3 预印本

- **Page title / 页面原文标题:** EN: “Towards a Science of Scaling Agent Systems” — [arXiv v3 record](https://arxiv.org/abs/2512.08296v3). 中文：页面原文标题为 “Towards a Science of Scaling Agent Systems”——[arXiv v3 记录](https://arxiv.org/abs/2512.08296v3)。
- **Source type / 来源类型:** EN: arXiv preprint/version record; this record is not itself a peer-reviewed publication. 中文：arXiv 预印本/版本记录；该记录本身不等同于同行评审出版物。
- **Publication/update/version date / 发布、更新或版本日期:** EN: v1 submitted 2025-12-09; v2 submitted 2025-12-17; v3 last revised 2026-04-08. 中文：v1 于 2025-12-09 提交；v2 于 2025-12-17 提交；v3 最后修订于 2026-04-08。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The v3 abstract reports 260 configurations across six benchmarks, five architectures, and three model families; cross-validated R²=0.373 (0.413 with its task-grounded capability metric); and task-specific results including +80.8% and -70.0%. 中文：v3 摘要报告 260 种配置、六个基准、五种架构和三个模型家族；交叉验证 R²=0.373（使用其 task-grounded capability metric 时为 0.413）；以及包括 +80.8% 和 -70.0% 在内的任务特定结果。
- **Does not establish / 来源不能证明:** EN: These are v3 abstract claims, not the early Google blog's 180-configuration/four-benchmark results. The record does not explain every difference between versions; cite the intended version and do not merge their counts. 中文：这些是 v3 摘要中的主张，不是 Google 早期博客的 180 种配置/四个基准结果。该记录没有解释所有版本差异；引用时应注明所用版本，不得合并计数。

## Topology-specific papers and repeated sampling / 特定拓扑论文与重复采样

### MacNet — ICLR 2025 poster entry / MacNet——ICLR 2025 海报条目

- **Page title / 页面原文标题:** EN: “Scaling Large Language Model-based Multi-Agent Collaboration” — [ICLR 2025 virtual-program poster](https://iclr.cc/virtual/2025/poster/30077). 中文：页面原文标题为 “Scaling Large Language Model-based Multi-Agent Collaboration”——[ICLR 2025 虚拟会议海报条目](https://iclr.cc/virtual/2025/poster/30077)。
- **Source type / 来源类型:** EN: ICLR 2025 conference virtual-program poster entry for a peer-reviewed conference paper. 中文：同行评审会议论文对应的 ICLR 2025 会议虚拟节目海报条目。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Conference year and poster type shown as 2025; exact posting date not shown. 中文：页面标注会议年份和海报类型为 2025；未显示确切发布日期。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The abstract describes MacNet as organizing agents in directed acyclic graphs (DAGs), with interactive reasoning topologically orchestrated; it reports experiments involving large-scale configurations, including over a thousand agents. 中文：摘要将 MacNet 描述为以有向无环图（DAG）组织 agents，并按拓扑顺序编排交互推理；摘要报告了大规模配置实验，包括超过一千个 agents 的设置。
- **Does not establish / 来源不能证明:** EN: DAG nodes and edges are specific to this method; the poster does not establish a universal team-size recommendation or real-world optimal agent count. It does not establish the repeated-sampling method of the separate Agent Forest paper. 中文：DAG 节点和边属于该方法特定设计；海报不能证明通用团队规模建议或现实场景中的最优 Agent 数量，也不能证明另一篇 Agent Forest 论文所述的重复采样方法。

### MacNet — arXiv v3 / MacNet——arXiv v3

- **Page title / 页面原文标题:** EN: “Scaling Large Language Model-based Multi-Agent Collaboration” — [arXiv v3 record](https://arxiv.org/abs/2406.07155v3). 中文：页面原文标题为 “Scaling Large Language Model-based Multi-Agent Collaboration”——[arXiv v3 记录](https://arxiv.org/abs/2406.07155v3)。
- **Source type / 来源类型:** EN: arXiv preprint abstract/record, version 3. 中文：arXiv 预印本摘要/记录，第 3 版。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Submitted 2024-06-11; v3 last revised 2025-03-17; the record comments say “Accepted to ICLR-2025.” 中文：提交于 2024-06-11；v3 最后修订于 2025-03-17；记录备注称 “Accepted to ICLR-2025”。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The abstract describes MacNet as DAG-organized agent collaboration with topologically orchestrated interactive reasoning; the arXiv record supplies the v3 date and ICLR-2025 acceptance comment. 中文：摘要将 MacNet 描述为以 DAG 组织的 Agent 协作，并通过拓扑顺序编排交互推理；arXiv 记录提供 v3 日期及 ICLR-2025 接收备注。
- **Does not establish / 来源不能证明:** EN: This version record does not establish the ICLR poster page's exact posting date or a universal optimal agent count. Its DAG method is not the repeated-sampling/voting method in the separate Agent Forest paper. 中文：该版本记录不能证明 ICLR 海报页面的确切发布日期，也不能证明通用最优 Agent 数量。其 DAG 方法不同于另一篇 Agent Forest 论文中的重复采样/投票方法。

### “More Agents Is All You Need” — repeated sampling / “More Agents Is All You Need”——重复采样

- **Page title / 页面原文标题:** EN: “More Agents Is All You Need” — [arXiv HTML v2](https://arxiv.org/html/2402.05120v2). 中文：页面原文标题为 “More Agents Is All You Need”——[arXiv HTML v2](https://arxiv.org/html/2402.05120v2)。
- **Source type / 来源类型:** EN: arXiv full-text preprint, version 2. 中文：arXiv 预印本全文，第 2 版。
- **Publication/update/version date / 发布、更新或版本日期:** EN: v2 revised 2024-10-11; no separate journal publication date is shown on this page. 中文：v2 修订于 2024-10-11；该页未显示单独的期刊发布日期。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The paper describes Agent Forest as repeated LLM sampling followed by aggregation/voting to select an answer. 中文：论文将 Agent Forest 描述为重复进行 LLM 采样，再通过汇总/投票选择答案。
- **Does not establish / 来源不能证明:** EN: Repeated samples/votes are not equivalent to a work-sharing team with separate responsibilities, handoffs, and shared state. The listed page does not display TMLR publication metadata; do not assert that venue from this URL alone. 中文：重复采样/投票不等同于具有独立分工、交接和共享状态的协作团队。所列页面未显示 TMLR 出版信息；仅凭该 URL 不应断言其期刊出处。

## Safe planning conclusions / 稳妥的规划结论

These are bounded planning recommendations, not universal empirical laws:

以下是有边界的规划建议，不是普遍经验定律：

- Compare a candidate multi-agent design with a capable single-agent baseline on the same task and budget; the OpenAI guide describes starting with a capable single-agent workflow, while the Google, Nature/arXiv, and Anthropic reports show results tied to specific tasks, models, and experimental setups ([OpenAI](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/), [Google Research](https://research.google/blog/towards-a-science-of-scaling-agent-systems-when-and-why-agent-systems-work/), [Nature](https://www.nature.com/articles/s42256-026-01268-y), [Anthropic](https://www.anthropic.com/research/multiagent-systems)). / 将候选多 Agent 方案与同一任务、同一预算下有竞争力的单 Agent 基线比较；OpenAI 指南建议先建立有竞争力的单 Agent 流程，而 Google、Nature/arXiv 和 Anthropic 报告均显示结果受具体任务、模型和实验设置限制（[OpenAI](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/)、[Google Research](https://research.google/blog/towards-a-science-of-scaling-agent-systems-when-and-why-agent-systems-work/)、[Nature](https://www.nature.com/articles/s42256-026-01268-y)、[Anthropic](https://www.anthropic.com/research/multiagent-systems)）。
- Choose topology based on separable work, sequential dependencies, evidence/capability differences, shared-state needs, cost, and error consequences; distinguish DAG collaboration from repeated sampling/voting ([MacNet](https://arxiv.org/abs/2406.07155v3), [Agent Forest](https://arxiv.org/html/2402.05120v2)). / 根据工作可分离性、顺序依赖、证据/能力差异、共享状态需求、成本及错误后果选择拓扑；区分 DAG 协作与重复采样/投票（[MacNet](https://arxiv.org/abs/2406.07155v3)、[Agent Forest](https://arxiv.org/html/2402.05120v2)）。
- Measure quality, coverage, time, monetary/token cost, coordination, conflict, and rework. Without a same-task, same-tool, same-budget comparison, recommend only a provisional configuration for the current task; do not claim universal optimal headcount, causal efficiency gains, or a general success rate. / 衡量质量、覆盖面、耗时、金钱/token 成本、协调、冲突和返工。没有同任务、同工具、同预算对照时，只提出适用于当前任务的暂定配置；不得声称存在通用最优人数、因果效率收益或普遍成功率。
