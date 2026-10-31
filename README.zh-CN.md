[English](README.md)

# 多 Agent 工作流程规划器 v6.5

这是一款双语 Agent Skill，帮助助手规划适度的单 Agent 或多 Agent 工作流程。v6.5 新增用于多阶段/共享工作的可选简短可回查状态卡；要求阶段切换或重新接手时依据原始指示和适用规则刷新状态；明确可问责协调者也可兼任低冲突工作单元；并记录关于上下文、验证、协调模式和角色提示的有边界证据。它提供指令和参考资料，并非平台集成；不会自行创建 Agent、工具、权限、后台任务或运行时行为。

## 用途

本 Skill 关注交付物、硬性要求、已核实的宿主能力、人类决策、隐私、外部行动授权、核验和停止条件。对边界清楚、低风险的任务保留轻量流程；对复杂、高风险或多阶段任务采用完整流程。每项交付物和共享写入都有明确负责人，但不要求固定团队岗位表。具体团队章程中的主要职责应予遵守，同时允许相容职责兼任；通用工作流程应按交付物映射职责，而非强加固定席位。

**设计来源边界：**角色/关注重点启发规则根据用户对一个共享 ChatGPT 对话的描述提炼。该分享页混合用户构想、模型生成的综合建议、外部产品/研究陈述及可能的抓取噪声；这里只将其作为设计启发，不当作独立研究、平台能力依据或普遍效果保证。平台和研究事实主张以链接来源及其范围为限；v6.5 研究参考区分检索位置研究、指令遵循评测、特定上下文压缩实验、厂商系统示例和框架特定结果。协调规则属于设计建议，不是某种角色安排总会更有效的因果证明。

## 仓库结构

- `.github/skills/multi-agent-workflow-planner/SKILL.md` — 简明的双语核心规则与安全门槛。
- `.github/skills/multi-agent-workflow-planner/references/platform-capability-examples.md` — 有日期且受来源范围限定的平台文档；不是运行时测试结果。
- `.github/skills/multi-agent-workflow-planner/references/research-claim-boundaries.md` — 关于 Agent 数量、拓扑、上下文、角色或协作效能主张的证据限制。
- `.github/skills/multi-agent-workflow-planner/references/workflow-templates.md` — 可选的任务、工作单元、变更、交接和当前状态卡表单。
- `.github/skills/multi-agent-workflow-planner/references/behavior-checks.md` — 可选的行为测试提示；提示不代表测试已运行。
- `LICENSE-CHOICE-REQUIRED.txt` — 等待所有者决定的提示，不是许可证。

## 后续安装或导入（仅为说明）

1. Skill 文件位于 `.github/skills/multi-agent-workflow-planner/`。若所有者之后决定导入，请将其中的 `SKILL.md` 与相邻的 `references/` 目录放在一起，因为 Skill 使用相对链接。v6.5 双语候选曾被分配到一个探索性 Cue 筛查群；可见群记录未显示实际选择的软件包哈希或逐轮 Skill 激活情况。因此不能确认该包已加载，也不能据此判断运行时表现。README 和许可证提示保留在软件包根目录。
2. 在 GitHub 文档说明的 Copilot 项目场景中，`.github/skills/multi-agent-workflow-planner/` 是一种文档所述的发现路径。导入步骤和支持的位置应以当前宿主的文档为准。[Agent Skills 格式规范](https://agentskills.io/specification)说明文件格式；[GitHub 添加 Copilot Agent Skills 指南](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills)仅说明 GitHub 专属路径和 CLI 行为。GitHub 路径并非通用 Agent Skills 要求。
3. 若之后导入，应确认当前宿主已加载该 Skill，且其相对参考链接均可访问。导入 Skill 不会赋予宿主新的功能或权限。

## 核验状态

- **Skill 结构：** 本地 v6.5 副本中的 Skill 目录通过 `quick_validate.py`。
- **本地静态检查：** 通过——7 个 Markdown 文件；12 条相对 Markdown 链接均可解析；15 个行为检查均有成对的中英文提示与预期；双语/版本标记、软件包结构及隐私/绝对路径扫描通过。v6.3/v6.4 哈希保持不变，v6.5 未复制 Git 元数据。
- **来源链接：** 新增的 8 个来源链接均可访问。对软件包中 30 条唯一外部 Markdown 链接进行了检查；其中沿用的一个 OpenAI 指南对直接链接检查器返回 HTTP 403，但通过公开页面读取器成功读取了页面标题与内容，未发现失效链接。所引摘要不能证明协调者角色、上下文长度或多 Agent 的普遍因果效应。
- **行为检查：**`references/behavior-checks.md` 包含回归提示。v4 快速 Cue 筛查按方案将一个新群分配给 v6.5 双语候选；可见群记录未显示实际选择的软件包哈希或逐轮 Skill 激活情况。因此，这轮不能确认已加载本包，也不能证明运行时表现、稳定性或因果效果。测试群中未见实际搜索、委派或研究行动。
- **运行时/平台测试：** v6.5 未在 Cue、GitHub Copilot、Claude Code 或其他宿主内实测；不声称已验证实际运行时行为。
- **跨平台测试：** 未在 Windows 或 macOS 上测试。Markdown/YAML 格式和相对链接不保证宿主兼容。

## 宿主能力边界

Skill 仅提供指令和随附参考资料。每项任务都应核实当前宿主、账户、版本和权限。不得仅凭参考示例推断能力可用、资源共享或隔离、自动重试、后台运行或授权状态。

## 许可证与发布门槛

本仓库为公开仓库。v6.5 双语版位于 `main` 的 `.github/skills/multi-agent-workflow-planner/`，作为当前活动 Skill。本仓库尚未选择许可证；见 [`LICENSE-CHOICE-REQUIRED.txt`](LICENSE-CHOICE-REQUIRED.txt)，该文件不是许可证。本次不创建 Git 标签或 GitHub Release。仓库公开可见不等于授予使用、修改或再分发权利。
