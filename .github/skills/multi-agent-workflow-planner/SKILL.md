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
4. Divide work only when separable responsibilities add material value beyond duplication, conflict, handoff, and integration costs. Give shared writes one owner or a clear interface; assign dependencies. Do not claim an optimal team size or causal multi-agent gains without a comparable same-task, same-budget test, or generalize task-specific results into universal success claims. / 仅当可分离的职责带来的实质价值高于重复、冲突、交接和整合成本时才拆分工作。共享写入应有唯一负责人或明确接口；注明依赖关系。没有同任务、同预算的可比测试时，不得宣称团队人数最优或多 Agent 带来因果收益，也不得把特定任务结果泛化为普遍成功率。
5. Use risk-proportionate gates and track only material facts, unknowns, assumptions, decisions, and versions. / 按风险设置阶段门，只记录重要事实、未知、假设、决定和版本。
6. Check key factual claims against primary and contrary evidence where relevant; report source limits and conflicts. Check factual accuracy separately from audience and purpose fit. Resolve substantive disagreements with evidence or a discriminating test, not a vote or agent consensus. / 适用时用原始证据和反证核查重要事实主张；说明来源限制和冲突。将事实准确性与受众及用途适配度分开检查。通过证据或区分性测试解决实质分歧，不靠投票或 Agent 共识。
7. Deliver the artifact and version, acceptance status, limits, open items, next decision, and which external actions remain unperformed; then stop or hand off. / 交付产物及版本、验收状态、限制、未决项、下一项决定，以及尚未执行的外部行动；然后停止或交接。

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
