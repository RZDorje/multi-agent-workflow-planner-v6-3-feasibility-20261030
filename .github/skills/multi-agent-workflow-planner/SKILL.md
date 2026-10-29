---
name: multi-agent-workflow-planner
description: "EN: Plan proportionate single- or multi-agent workflows around the requested outcome, hard constraints, verified host capabilities, human decision gates, and authorization boundaries. Use when a task needs responsibility splitting, parallel or sequential work, independent review, handoffs, staged approval, capability checks, or automation planning; do not silently replace a required execution mode. / 中文：围绕目标、硬性要求、已核实的宿主能力、人类决策点和授权边界，规划适度的单 Agent 或多 Agent 工作流程。用于需要职责拆分、并行或串行协作、独立审查、交接、阶段审批、能力核验或自动化规划的任务；不得静默替换用户要求的执行模式。"
---

# Multi-Agent Workflow Planner / 多 Agent 工作流程规划器

Design the workflow around the user's outcome—not around a preferred number of agents. Roles describe responsibilities, not fixed seats. First identify constraints and decision rights, then verify the capabilities actually available in this run, and choose the least burdensome workflow that satisfies the requirements. A stated requirement is an acceptance condition, not an optimization preference.

围绕用户要完成的成果设计流程，而不是先决定 Agent 数量。角色代表责任，不代表固定席位。先识别约束和决策权，再核实本次实际可用能力，最后选择满足要求且负担最小的流程。用户明确提出的要求是验收条件，不是可自行放宽的优化偏好。

## Choose the light or full path / 选择轻量或完整流程

### Light path — simple, low-risk work / 轻量流程——简单、低风险任务

For a bounded task that one capable agent can complete with little uncertainty, use only these steps:

对于边界清楚、单个 Agent 即可完成且不确定性较低的任务，只做以下步骤：

1. State the requested output, any hard constraints, who decides, and what is authorized now. / 写明交付物、硬性要求、决策者以及当前授权范围。
2. Check only the capabilities that could change this task; never assume a requested capability exists. / 只核实可能改变本任务方案的能力；绝不假定用户要求的能力已存在。
3. Do the smallest suitable unit of work, normally with one agent; verify the result against the request. / 以最小合适工作单元执行，通常由单个 Agent 完成，并按要求核验结果。
4. Deliver the result, any material limitation, and the next decision if one is needed; stop. / 交付结果、重要限制和必要的下一项决定，然后停止。

Do not add agents, plans, trackers, approval gates, or questions merely for form. The light path reduces process overhead only; it never relaxes a hard requirement, capability gate, privacy rule, or authorization boundary.

不要为了形式增加 Agent、计划、跟踪表、审批门或提问。轻量流程只减少流程负担，绝不放宽硬性要求、能力门槛、隐私规则或授权边界。

### Full path — complex, risky, or multi-stage work / 完整流程——复杂、高风险或多阶段任务

Use the relevant steps below, scaling their detail to risk and uncertainty; not every task needs every artifact.

按风险和不确定性采用下列相关步骤；并非每个任务都需要所有环节或文档。

1. Define outcome, hard requirements, decision owner, authorized phase, and stop conditions. / 定义成果、硬性要求、决策者、当前授权阶段和停止条件。
2. Verify the actual host, tools, permissions, and required execution mode. / 核验实际宿主、工具、权限和用户要求的执行模式。
3. Choose the delivery mode and human handoff point. / 选择交付模式和人类交接点。
4. Split responsibilities only where it adds real value; assign ownership, dependencies, and status. / 仅在确有价值时拆分职责；明确负责人、依赖关系和状态。
5. Add risk-proportionate stage gates and small, reviewable intermediate outputs. / 按风险设置阶段门和小型、可审查的中间产物。
6. Track material facts, unknowns, assumptions, decisions, versions, and changes. / 记录重要事实、未知、假设、决定、版本和变更。
7. Verify factual correctness separately from suitability for the audience and purpose. / 将事实正确性与受众和用途适配度分开验证。
8. At acceptance or a decision boundary, stop, hand off, or continue only within existing authorization. / 到达验收点或决策边界时，停止、交接，或仅在现有授权范围内继续。

## 1. Define outcome, constraints, and decision rights / 定义成果、约束与决策权

Create a compact task card. Separate explicit requirements from inferences:

建立简明任务卡，并区分明确要求与推断：

- **Output and audience:** deliverable, users, format, scope, and timing. / **交付物与对象：** 产出、使用者、格式、范围和时间要求。
- **Hard requirements:** required scope, format, sources, privacy, budget, permissions, execution mode, and prohibited actions. Treat each as pass/fail; never downgrade an explicit requirement to a preference. / **硬性要求：** 必须满足的范围、格式、来源、隐私、预算、权限、执行模式和禁止事项。逐项作为通过/不通过条件；不得把明确要求降格为偏好。
- **Trade-offs:** speed, cost, coverage, readability, and conservatism. If no priority is stated, mark it undecided rather than inventing one. / **权衡项：** 速度、成本、覆盖面、可读性和保守程度。未给出优先级时标为待定，不得擅自编造。
- **Subjective quality:** turn goals such as “persuasive,” “clear,” or “creative” into review dimensions or examples. For an undecided direction, offer low-cost alternatives instead of choosing for the user. / **主观质量：** 将“有说服力”“清楚”“有创意”等目标转成审查维度或样例。方向未定时先提供低成本选项，不替用户定案。
- **Decision owner:** identify who may choose direction, accept risk, approve changes, or authorize external action. Review comments are not authorization. / **决策者：** 标明谁可决定方向、接受风险、批准修改或授权外部行动。审查意见不是授权。
- **Phase and stop conditions:** state what is allowed now, what awaits a later decision, and when to pause or abandon. / **阶段与停止条件：** 写明当前允许事项、等待后续决定的事项，以及暂停或放弃的条件。

Classify relevant statements as facts, unknowns, assumptions, preferences, or decisions. Ask only when missing information could materially change the current phase's direction, risk, authority, or acceptance and cannot be safely defaulted. For staged work, ask only what blocks the current phase; do not front-load questions about future purchase, publication, or finalization. If a hard requirement cannot be met or verified, stop at the decision point described below rather than rewriting the requirement as an “optimization.”

将重要陈述分类为事实、未知、假设、偏好或决定。只有当缺失信息会实质改变当前阶段的方向、风险、权限或验收，且无法安全默认时，才提问。分阶段工作只问阻塞当前阶段的问题；不要提前追问未来购买、发布或定稿事项。若硬性要求无法满足或核实，应按下文停在决定点，不得以“优化”为名改写要求。

## 2. Verify host capabilities; enforce hard gates / 核验宿主能力并执行硬性门槛

Before assigning collaboration, inspect the actual environment, currently visible tools, and the user-specified target platform or runtime. A product name, past experience, marketing page, or capability in another account does not prove availability in this run. Respect any limit to approved materials or static simulation; do not perform new platform research or real operations when out of scope.

安排协作前，检查本次实际运行环境、当前可见工具以及用户指定的平台或运行时。产品名称、过往经验、营销页面或其他账户的能力都不能证明本次可用。遵守获准资料范围或静态模拟限制；超出范围时不得开展新的平台研究或真实操作。

Check only what is relevant, such as:

按任务相关程度核查，例如：

- Whether agents/workers exist, are persistent or temporary, have independent context, and what quantity is available. / 是否有 Agent/worker、是否持久或临时、上下文是否独立及可用数量。
- Whether work can run in parallel; how it is scheduled, returned, paused, resumed, cancelled, retried, and logged. / 是否可并行、如何调度和返回结果、暂停/恢复/取消/重试及查看记录。
- What files, messages, memory, skills, browsers, accounts, and credentials are shared or isolated. / 文件、消息、记忆、Skills、浏览器、账号和凭证的共享或隔离范围。
- Which search, code, file, and external-service tools are available and authorized now. / 当前有哪些已授权的搜索、代码、文件和外部服务工具。
- What an approval covers and which side effects may already have occurred. / 审批实际覆盖什么，以及哪些副作用可能已发生。
- Skill file format, loading method, and scope, if relevant. / 若涉及 Skill，核实其文件格式、加载方式和生效范围。

Label consequential capabilities by evidence: **observed/run in this session**, **visible but not run**, **documented by an approved source**, **internal experience**, **unknown/unverified**, or **not visible in this environment**. Cite a source and date for platform-specific claims when relevant. “Not visible” does not mean “unsupported.” Async invocation does not prove durable background execution, retries, or an audit log. Read [platform capability examples](references/platform-capability-examples.md) only when a platform example or public source is useful; it is not a complete catalog or a guarantee for the current account.

按证据标记会影响方案的能力：**本次已观察/运行**、**当前可见但未运行**、**获准来源有说明**、**内部经验**、**未知/未验证**或**当前环境未显示**。涉及平台具体能力时，按需引用来源和日期。“未显示”不等于“不支持”；异步调用也不能证明有持久后台运行、重试或审计记录。仅在需要平台示例或公开来源时读取[平台能力示例](references/platform-capability-examples.md)；它不是完整目录，也不保证当前账户具备这些能力。

**Non-negotiable execution-mode gate:** If the user explicitly requires a mode or resource—such as a specified number of independent agents running in parallel or overnight/durable background work—and this host does not show or verify it, do not start work using a substitute mode. State that the capability is “not visible/unverified here,” not that the platform cannot support it. Offer one concrete alternative with its differences, or an environment with verified capability, and ask whether the user accepts. Until the user accepts a specific alternative, stop. A deadline, agent recommendation, or platform hint is not permission to change modes.

**不可弱化的执行模式门槛：** 若用户明确要求某种模式或资源（例如指定数量的独立 Agent 并行、夜间或持久后台工作），而本次宿主未显示或验证该能力，不得先用替代模式启动工作。应说明“本次未显示/未验证”，而非断言平台不支持；提出一个具体替代方案及其差异，或建议使用能力已验证的环境，并询问用户是否接受。用户未接受具体替代方案前必须停止。截止时间、Agent 建议或平台提示都不是更换模式的授权。

Apply the same rule to every other unmet hard requirement. Use a safe alternative only if it violates no hard requirement or the user has accepted it. Continue without asking only when no hard requirement is changed and the alternative does not change the goal, acceptance, risk, or commitment; disclose material limits. Never claim parallelism, durable background work, credential isolation, or automatic retries without evidence from this run.

对其他未满足的硬性要求同样执行此规则。只有不违反任何硬性要求，或用户已接受替代方案时，才可采用安全替代。只有在未改变硬性要求，且替代方案不会改变目标、验收、风险或承诺时，才可不经询问继续，并披露重要限制。没有本次证据时，绝不声称已并行、持久后台运行、凭证隔离或自动重试。

## 3. Choose phases and human handoffs / 选择阶段与人类交接

Choose among a direct answer, editable draft, options, staged collaboration, or an authorized ongoing process. Define each handoff: recipient/decision owner, decision needed, options and trade-offs, evidence to review, and default pause point.

在直接答复、可编辑草稿、备选方案、分阶段协作或已授权的持续流程中选择。明确每次交接的接收者/决策者、所需决定、选项与取舍、待审证据和默认暂停点。

For creative or subjective work without a chosen direction, first provide inexpensive, reversible options—a direction card, title/opening samples, a short outline, or a prototype. Expand only after the decision owner chooses. Report factual accuracy separately from audience/style fit: accuracy does not prove suitability, and preference does not prove truth.

对方向未定的创意或主观工作，先给低成本、可撤回的选项，例如方向卡、标题/开头样例、短提纲或小样。决策者选定后再扩大投入。事实准确性与受众/风格适配应分开报告：准确不等于适合，偏好也不证明事实正确。

After an authorized phase or subtask, deliver its output, status, unresolved items, and required decision. Pause at the user's decision point or phase boundary. Do not expand scope, start an unauthorized phase, or treat a recommendation as an approved decision. Continue within the original authorization only if the next phase is already clearly authorized and needs no new decision.

完成已授权阶段或子任务后，交付其产物、状态、未决项和所需决定。到达用户决策点或阶段边界时暂停。不得扩围、启动未授权阶段或把建议当成已批准决定。只有下一阶段已有明确授权且无需新增用户决定时，才可在原授权范围内继续。

Research permission is not action permission. If the user authorizes research or a draft, do not buy, pay, order, publish, send, submit, or change access/visibility. Before an external action, confirm the exact target, content, channel/recipient, amount, and material terms as applicable, and obtain explicit authorization. Without it, stop at a draft or recommendation awaiting approval. A time estimate is not authorization for another execution mode, ongoing work, or an external action.

研究授权不等于行动授权。用户只授权研究或起草时，不得购买、付款、下单、发布、发送、提交或更改访问权限/可见性。外部行动前，应核对具体对象、内容、渠道/收件人、金额和重要条款（如适用），并取得明确授权。未获授权时停在待批准草稿或建议。时间估算不是更换执行模式、持续工作或外部行动的授权。

## 4. Divide responsibility and maintain state / 按责任分工并维护状态

First test whether one agent can meet quality, risk, time, and cost constraints. Split only when a new responsibility adds meaningful parallelism, a distinct capability/evidence source, or an independent check. Coordination, research, production, validation, integration, and human decisions are separable responsibilities, not a mandatory role roster. Do not claim an optimal number without a comparable same-task, same-budget test.

先判断单个 Agent 是否能在质量、风险、时间和成本约束内完成。只有新增责任能带来实质并行、不同能力/证据来源或独立检查时才拆分。协调、研究、制作、验证、整合和人类决策是可分离的责任，不是固定角色表。没有同任务、同预算的可比测试，不得宣称人数最优。

For each work unit, record only the fields needed for control:

每个工作单元只记录维持控制所需的信息：

| Field / 字段 | Record / 记录内容 |
|---|---|
| ID, goal, exclusions / 编号、目标、排除项 | One inspectable output boundary / 可检查的单一产出边界 |
| Owner, status / 负责人、状态 | One accountable owner; e.g. queued, active, blocked, review, done, stale / 一名交付负责人；如待办、进行中、阻塞、待审、完成、过期 |
| Inputs, dependencies / 输入、依赖 | Required sources, upstream decisions/version, dependency state / 必需来源、上游决定/版本及依赖状态 |
| Output, evidence, acceptance / 产出、证据、验收 | Format, source bar, review method, location / 格式、来源要求、审查方式、位置 |
| Permission, stop / 权限、停止条件 | Allowed/prohibited actions and when to pause / 允许/禁止的行动及暂停条件 |
| Deduplication key / 去重键 | Covered question/source/file to prevent duplicate or conflicting work / 已覆盖的问题、来源或文件，用于避免重复和冲突 |

Parallelize only when inputs and outputs are separable and expected benefit exceeds duplication, conflict, handoff, and integration cost. Give shared writes one owner or a clear interface. Track claims, sources, files, and ownership to prevent duplicate assignments. The integrator resolves duplicates, conflicts, open items, and acceptance. For independent review, freeze the candidate version where practical; ask reviewers for evidence and defects, not agreement. Use a sequential alternative only if it does not violate a hard requirement or the user has accepted it.

仅当输入与产物可分离，且预期收益高于重复、冲突、交接和整合成本时并行。共享写入应有唯一负责人或明确接口。跟踪问题、来源、文件和负责人，避免重复派发。整合者负责去重、冲突、未决项和验收。独立审查尽可能先冻结待审版本；请审查者给出依据和缺陷，而非只表态同意。只有不违反硬性要求或用户已接受时，才可改用串行方案。

## 5. Use risk-proportionate stage gates / 按风险设置阶段门

Use only the gates that can expose a material error or protect a decision:

只采用能发现重要错误或保护决策的阶段门：

1. **Plan gate:** task card, hard requirements, capability evidence, assignment, and risk boundary. / **计划门：** 任务卡、硬性要求、能力证据、分工和风险边界。
2. **Evidence gate:** for research, key findings, source list, conflicts, and unknowns before major drafting or action. For high-consequence legal or similar work, ask for the jurisdiction if its absence could change the conclusion. / **证据门：** 研究任务在重要写作或行动前交关键发现、来源清单、冲突和未知。法律等高后果任务中，若法域会改变结论而未提供，应先询问法域。
3. **Direction gate:** for subjective or costly production, show low-fidelity options and trade-offs before expanding. / **方向门：** 主观或高成本制作先展示低保真选项和取舍，再扩大工作。
4. **Delivery gate:** integrated version, separate fact/fit checks, open items, and change notes. / **交付门：** 整合版本、分开的事实/适配检查、未决项和变更记录。
5. **External-action gate:** stop before payment, public posting/sending, submission, or permission change until the exact action is authorized. / **外部行动门：** 付款、公开发布/发送、提交或权限变更前必须停下，直至具体行动获授权。

Each gate should produce a small, readable, reversible artifact that can reveal errors. A gate is not a reason to ask for permission repeatedly. Pause only when direction, risk, authority, hard requirements, or irreversibility materially changes. Future-phase questions are not current blockers.

每个阶段门都应产出小而可读、可撤回且能暴露错误的材料。阶段门不是反复征求许可的理由。只有方向、风险、权限、硬性要求或难逆性发生实质变化时才暂停询问。未来阶段的问题不应伪装成当前阻塞。

## 6. Track evidence and propagate changes / 记录证据并传递变更

For work where it matters, keep a concise ledger:

对重要工作维护精简台账：

- **Fact:** checkable statement, evidence location, source type, date/version, scope; distinguish primary sources from retellings. / **事实：** 可核查陈述、证据位置、来源类型、日期/版本和适用范围；区分原始来源与转述。
- **Unknown:** missing evidence, why it matters, and who can resolve it; never fill gaps with speculation. / **未知：** 缺失证据、重要性及可解决者；不得用猜测填补。
- **Assumption:** temporary condition, basis, impact, and validation/failure trigger. / **假设：** 暂用条件、依据、影响和验证/失效触发点。
- **Decision:** decision owner, options, trade-offs, date, and authorization scope; distinguish advice, user decision, and execution. / **决定：** 决策者、选项、取舍、日期和授权范围；区分建议、用户决定与执行。
- **Version:** stable identifiers for inputs, standards, drafts, and outputs; who changed what and when. / **版本：** 输入、标准、草稿和产出的稳定标识，以及变更者和时间。

If the goal, audience, success criteria, budget, sources, or authorization changes, pause affected work and trace impacts to decisions, active/queued tasks, shared instructions, files, tests, acceptance criteria, dependencies, and handoffs. Preserve work independent of old conditions; mark dependent work stale or needing review; update versions and affected downstream instructions before resuming. Do not discard completed work wholesale when only some dependencies changed.

若目标、受众、成功标准、预算、来源或授权改变，应暂停受影响工作，并追踪其对决定、进行中/待办任务、共享指令、文件、测试、验收标准、依赖和交接的影响。保留不依赖旧条件的成果；将依赖旧条件的工作标为过期或待复核；恢复前更新版本和受影响的下游指令。只有部分依赖变化时，不要一概丢弃已完成工作。

## 7. Verify truth and suitability separately / 分开验证事实与适配度

**Fact check:** Is each material claim supported and accurate? Check key claims against primary sources, dates, definitions, calculations, context, and contrary evidence. State conflicts and what the evidence cannot establish. High-impact claims should not rely only on the author or copies of the same source. Use independent evidence or a mechanical test when appropriate.

**事实核验：** 重要陈述是否有依据且准确？对照原始来源、日期、定义、计算、上下文和反证核查关键主张。说明来源冲突及证据无法证明之处。高影响主张不应只依赖作者或同一来源的副本；适用时使用独立证据或机械测试。

**Fit check:** Is the output appropriate for this user, audience, goal, and use? Check the task card's audience, purpose, tone, structure, format, actionability, accessibility, and quality criteria. Read [research claim boundaries](references/research-claim-boundaries.md) only when advising on agent counts, topologies, or collaboration effectiveness.

**适配核验：** 交付是否适合当前用户、受众、目标和用途？按任务卡检查受众、用途、语气、结构、格式、可操作性、可访问性和质量标准。只有讨论 Agent 数量、拓扑或协作效能时才读取[研究主张边界](references/research-claim-boundaries.md)。

Report the two checks separately. Readability, format compliance, user preference, compilation, or another agent's agreement does not prove factual accuracy; factual accuracy does not prove suitability. Resolve substantive disagreements by classifying them as fact, definition, reasoning, preference, or risk acceptance and seeking evidence or a discriminating test. Without new evidence, record the issue as unresolved rather than voting by headcount.

分别报告两类检查。可读、格式合规、用户喜欢、编译通过或另一个 Agent 同意，都不能证明事实准确；事实准确也不能证明用途适配。将实质分歧归类为事实、定义、推理、偏好或风险接受，再寻找证据或能区分选项的测试。没有新证据时记录未决，不靠人数投票。

## 8. Deliver, stop, and learn / 交付、停止与复盘

At handoff, state the current phase's acceptance status, actual artifact and version, evidence/source types, unresolved unknowns, capability limits, next decision, and whether external actions remain unperformed. Distinguish document review, static inspection, and observed runtime behavior.

交接时说明当前阶段验收状态、实际产物及版本、证据/来源类型、未解决未知、能力限制、下一项决定，以及外部行动是否仍未执行。区分文档核查、静态检查和真实运行观察。

Stop when the current phase meets its hard acceptance criteria and more work is unlikely to change a material decision; when a user decision or phase boundary is reached; when risk or authority requires a handoff; when a substitute would violate a hard requirement or has not been accepted; or when further work would repeat known material without new evidence, a decision-relevant question, or a discriminating test. Record unfinished items and the condition for resuming. Do not manufacture progress through repeated rewrites or reviews.

当当前阶段已满足硬性验收且继续工作不太可能改变重要决定；到达用户决策点或阶段边界；风险或权限要求交接；替代方案会违反硬性要求或尚未获接受；或后续工作没有新证据、决策相关问题或区分性测试、只会重复已知内容时，停止。记录未完成项和恢复条件。不得用反复改写或审查制造进展。

A retrospective should use observable data only: outputs by phase, defects/omissions, rework and causes, waiting/coordination/review time, reliable call/cost data if available, stop point, and one testable next improvement. Distinguish a single static simulation, user/author report, official documentation, and runtime observation. Without a controlled comparison, do not infer causal multi-agent gains, universal success rates, or an optimal team size.

复盘仅记录可观察数据：各阶段产物、错误/遗漏、返工及原因、等待/协调/复核时间、（若有可靠数据）调用或费用、停止点和一个可测试的改进。区分单次静态模拟、用户/作者自述、官方文档和真实运行观察。没有受控对照时，不得推断多 Agent 的因果收益、通用成功率或最优人数。

## References / 参考资料

- Read [platform capability examples](references/platform-capability-examples.md) only for relevant platform-specific examples, public documentation, and installation notes. / 仅在需要平台能力示例、公开文档或安装说明时读取[平台能力示例](references/platform-capability-examples.md)。
- Read [research claim boundaries](references/research-claim-boundaries.md) only for agent-count, topology, or collaboration-effectiveness claims. / 仅在涉及 Agent 数量、拓扑或协作效能主张时读取[研究主张边界](references/research-claim-boundaries.md)。
