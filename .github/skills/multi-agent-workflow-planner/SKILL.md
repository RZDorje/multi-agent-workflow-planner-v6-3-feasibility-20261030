---
name: multi-agent-workflow-planner
description: "EN: Plan proportionate single- or multi-agent workflows around the requested outcome, hard constraints, verified host capabilities, human decision gates, and authorization boundaries. Use when a task needs responsibility splitting, parallel or sequential work, independent review, handoffs, staged approval, capability checks, or automation planning; do not silently replace a required execution mode. / 中文：围绕目标、硬性要求、已核实的宿主能力、人类决策点和授权边界，规划适度的单 Agent 或多 Agent 工作流程。用于需要职责拆分、并行或串行协作、独立审查、交接、阶段审批、能力核验或自动化规划的任务；不得静默替换用户要求的执行模式。"
---

# Multi-Agent Workflow Planner / 多 Agent 工作流程规划器

Design the workflow around the user's requested outcome, not a preferred number of agents. Roles describe responsibilities, not fixed seats. Choose the least burdensome workflow that meets every explicit requirement; treat hard requirements as pass/fail, not preferences.

围绕用户要求的成果设计流程，而不是先决定 Agent 数量。角色代表责任，而非固定席位。选择满足所有明确要求且负担最小的流程；硬性要求是通过/不通过条件，不是偏好。

## Choose a workflow / 选择流程

### Light path — bounded, low-risk work / 轻量流程——边界清楚、低风险任务

For work one capable agent can complete with little uncertainty, use only the necessary steps:

对单个有能力的 Agent 即可低不确定性完成的任务，只做必要步骤：

1. State the output, hard constraints, decision owner, and what is authorized now. / 写明交付物、硬性约束、决策者和当前授权事项。
2. Check only capabilities that could change this task; never assume a requested capability exists. / 只核查可能改变本任务方案的能力；绝不假定用户要求的能力存在。
3. Do the smallest suitable unit of work and verify it against the request. / 执行最小合适工作单元，并按要求核验。
4. Deliver the result, material limits, and any next decision; stop. / 交付结果、重要限制和必要的下一项决定，然后停止。

Do not add agents, paperwork, approval gates, or questions merely for form. The light path never relaxes a hard requirement, privacy rule, capability gate, or authorization boundary.

不得为了形式增加 Agent、文书、审批门或提问。轻量流程绝不放宽硬性要求、隐私规则、能力门槛或授权边界。

### Full path — complex, risky, or multi-stage work / 完整流程——复杂、高风险或多阶段任务

Use only the steps and detail that help control the current task; scale them to uncertainty and consequences, not a fixed threshold.

仅采用有助于控制当前任务的步骤和细节；按不确定性和后果调整，不设固定门槛。

1. Define the outcome, acceptance conditions, hard requirements, decision owner, authorized phase, and stop conditions. / 定义成果、验收条件、硬性要求、决策者、已授权阶段和停止条件。
2. Verify the actual host, relevant tools and permissions, and any required execution mode. Label consequential capability evidence as observed in this run, visible but not run, documented, or unknown/not visible. / 核实实际宿主、相关工具与权限以及用户要求的执行模式。将重要能力证据标为本次已观察运行、当前可见但未运行、文档有说明或未知/未显示。
3. Choose the delivery mode, phases, and human handoffs. Ask only when missing information blocks the current phase and cannot be safely defaulted; do not front-load future-phase questions or treat advice/review as authorization. For an unsettled creative or costly direction, show low-cost, reversible options and trade-offs before expanding. / 选择交付方式、阶段和人类交接点。只有缺失信息阻塞当前阶段且无法安全默认时才询问；不要提前追问未来阶段，也不得把建议或审查意见当授权。创意或高成本工作的方向未定时，先展示低成本、可撤回的选项和取舍，再扩大投入。
4. Map deliverables and dependencies into the smallest useful work units and assign provisional accountable owners before deciding whether one agent can cover them or multiple agents add material value. Give every deliverable and shared write a clear owner; for shared writes, prefer one accountable owner with an explicit interface. Work units may be claimed, reassigned, split, merged, reprioritized, or canceled as evidence and dependencies change. Use multiple agents only when separable responsibilities add material value beyond duplication, conflict, handoff, and integration costs. Assign coordination, execution, integration, and independent review only as useful; do not require each role to produce its own parallel artifact. Weigh an independent review's expected risk reduction or decision value against its time and coordination cost; omit it when it would add little. Do not claim an optimal team size or causal multi-agent gains without a comparable same-task, same-budget test, or generalize task-specific results into universal success claims. / 先将交付物和依赖拆成必要且有用的工作单元，并为各单元指定暂定的可问责负责人，再判断一个 Agent 能否覆盖，或多个 Agent 是否能带来实质价值。每个交付物及共享写入都要有明确负责人；共享写入优先指定一名最终负责人与清晰接口。随着证据和依赖变化，可认领、重分配、拆分、合并、调整优先级或取消工作单元。只有当可分离职责带来的实质价值高于重复、冲突、交接和整合成本时才使用多个 Agent。仅在有用时分配协调、执行、整合和独立审查职责；不要求每个角色各自产出一份并行成果。权衡独立审查预期降低的风险或决策价值与其时间和协调成本；若审查增益很小则省略。没有同任务、同预算的可比测试时，不得宣称团队人数最优或多 Agent 带来因果收益，也不得把特定任务结果泛化为普遍成功率。
5. Use risk-proportionate gates and track only material facts, unknowns, assumptions, decisions, and versions. / 按风险设置阶段门，只记录重要事实、未知、假设、决定和版本。
6. Check key factual claims against primary and contrary evidence where relevant; report source limits and conflicts. Check factual accuracy separately from audience and purpose fit. Resolve substantive disagreements with evidence or a discriminating test, not a vote or agent consensus. / 适用时用原始证据和反证核查重要事实主张；说明来源限制和冲突。将事实准确性与受众及用途适配度分开检查。通过证据或区分性测试解决实质分歧，不靠投票或 Agent 共识。
7. Deliver the artifact and version, acceptance status, limits, open items, next decision, and which external actions remain unperformed; then stop or hand off. / 交付产物及版本、验收状态、限制、未决项、下一项决定，以及尚未执行的外部行动；然后停止或交接。

### Responsibility and reporting / 责任与汇报

Treat role names as complementary attention lenses or default review tendencies, not exclusive task boundaries, fixed seats, or a required four-role roster. Keep each work unit's accountable owner and primary responsibility emphasis reasonably stable where continuity helps, while allowing task boundaries, priorities, and working modes to change. Any member may flag a material gap or dependency outside their main focus and offer evidence or options, but should not silently change the allocation. The coordinator maintains the plan and decides whether to adopt proposals within current authorization. Set one user-facing coordinator/reporting owner; in multi-agent work, other members route routine progress, findings, and drafts to them for deduplication before one consolidated user/group update. Do not send duplicate standalone updates. Exceptions: the user directly names a member to report; the user directly asks a member a question or replies to that member, in which case the member may give the necessary direct response or next step and then report the outcome to the coordinator; the task explicitly requires separate reports or direct delivery of that member's artifact; or a material, time-sensitive risk or blocker needs immediate attention from the user/group. If a change transfers a work unit or deliverable, do not switch ownership until responsibilities are explicitly reassigned, a new accountable owner is named, affected tasks/dependencies are identified, and status, evidence, inputs, and acceptance criteria are handed over. Resolve substantive disagreements with evidence or a discriminating test, not role authority or a vote. Pause stale dependent work; stop for the user's decision if a change affects the objective, acceptance, or authorized scope. Preserve evidence requirements and stop conditions. / 将角色名称视为互补的关注视角或默认审查倾向，而非排他的任务边界、固定席位或必须配齐的四角色岗位表。在有助于保持连续性的情况下，让每个工作单元的可问责负责人和主要责任重心相对稳定，同时允许任务边界、优先级和工作模式变化。任何成员都可指出主责范围之外的重要缺口或依赖并提供证据/选项，但不得暗中改变任务分配。协调者负责维护计划，并判断是否在现有授权内采纳建议。指定一名单一的对外协调/汇报人；多 Agent 协作时，其他成员先将常规进度、发现和草稿交给其去重，再由其向用户/群发送一份汇总更新。避免成员各自重复对外汇报。例外：用户直接点名某成员汇报；用户直接向某成员提问或回复该成员时，该成员可先作必要的直接答复或给出下一步，再将结果回报协调者；任务明确要求分别汇报或由该成员直接交付其产物；或重大且紧急的风险/阻断需要立即告知用户/群。若变化会转移某个工作单元或交付物，在明确重分配职责、指定新的可问责负责人、列出受影响的任务/依赖，并交接当前状态、证据、输入和验收条件之前，不得切换负责人。通过证据或区分性测试而非角色权威或投票解决实质分歧。暂停已过期的依赖工作；若变化影响目标、验收或已授权范围，应停下等待用户决定。保留证据要求和停止条件。

## Non-negotiable gates / 不可弱化的门槛

**Unmet hard requirement or required mode.** If an explicitly required mode or resource is not visible or verified in this run, do not start with a substitute. Say “not visible/unverified here,” not “unsupported”; offer one concrete alternative and its differences (or a verified environment), ask whether the user accepts it, and stop until that specific alternative is accepted. Apply the same rule to every unmet hard requirement.

**未满足的硬性要求或执行模式。** 若本次未显示或验证用户明确要求的模式或资源，不得先用替代方案启动。应说“本次未显示/未验证”，而非“不支持”；提出一个具体替代方案及其差异（或能力已验证的环境），询问用户是否接受，并在用户接受该具体方案前停止。其他未满足的硬性要求同样处理。

**Authorization.** Research, recommendations, drafts, deadlines, or workflow plans do not authorize external action. Before buying, paying, ordering, publishing, sending, submitting, or changing access/visibility, obtain explicit authorization for the exact target and action, plus applicable content, recipient/channel, amount, and material terms. Without it, stop at a draft or recommendation; do not expand scope or begin an unauthorized phase.

**授权。** 研究、建议、草稿、截止日期或工作计划均不构成外部行动授权。购买、付款、下单、发布、发送、提交或更改访问权限/可见性前，必须取得针对具体对象和行动的明确授权，并确认适用的内容、收件人/渠道、金额和重要条款。未获授权时停在草稿或建议；不得扩围或启动未授权阶段。

**Change propagation.** If the goal, audience, acceptance criteria, budget, sources, or authorization changes, pause affected work and trace impacts through decisions, active/queued tasks, shared instructions, files, tests, acceptance, dependencies, and handoffs. Preserve unaffected and still-valid completed work; mark dependent work stale or needing review; update versions and downstream instructions before resuming.

**变更传递。** 若目标、受众、验收标准、预算、来源或授权改变，应暂停受影响的工作，并追踪对决定、进行中/待办任务、共享指令、文件、测试、验收、依赖和交接的影响。保留不受影响且仍有效的已完成工作；将依赖项标为过期或待复核；恢复前更新版本和下游指令。

**Stop and hand off.** Pause at a user decision, when risk or authority requires it, or when a substitute would violate an unaccepted hard requirement. At a phase boundary, continue only if the next phase is already clearly authorized and needs no new decision; do not ask permission repeatedly. Stop when acceptance is met and more work is unlikely to change a material decision, or when further review would only repeat known material without new evidence, a decision-relevant question, or a discriminating test. Record unresolved items and the condition for resuming.

**停止与交接。** 到达用户决策点、风险或权限要求暂停，或替代方案会违反尚未获接受的硬性要求时，必须暂停。阶段结束后，只有下一阶段已明确授权且无需新决定时才可继续；不得反复征求许可。达到验收且继续工作不太可能改变重要决定时停止；若后续审查没有新证据、决策相关问题或区分性测试、只会重复已知内容，也应停止。记录未决事项和恢复条件。

## Read references only when useful / 仅在有用时读取参考资料

- For copyable task, work-unit, change, or handoff forms, read [workflow templates](references/workflow-templates.md). They are optional; do not impose them on light-path tasks. / 需要可复制的任务、工作单元、变更或交接表单时，读取[工作流模板](references/workflow-templates.md)。模板为可选内容，不得强加给轻量任务。
- For behavior review, use [behavior checks](references/behavior-checks.md) as prompts, not as evidence that tests were run. / 进行行为审查时，可将[行为检查](references/behavior-checks.md)用作提示；提示本身不是测试已运行的证据。
- Read [platform capability examples](references/platform-capability-examples.md) only when a relevant host-specific source or installation example helps. Documentation is not proof of current runtime availability; check the live environment. / 仅在相关宿主来源或安装示例有帮助时，读取[平台能力示例](references/platform-capability-examples.md)。文档不证明当前运行时具备该能力；应检查实际环境。
- Read [research claim boundaries](references/research-claim-boundaries.md) only for claims about agent counts, topologies, or collaboration effectiveness. / 仅在涉及 Agent 数量、拓扑或协作效能主张时，读取[研究主张边界](references/research-claim-boundaries.md)。
