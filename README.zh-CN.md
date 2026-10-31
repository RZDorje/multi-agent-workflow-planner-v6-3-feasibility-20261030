[English](README.md)

# 多 Agent 工作流程规划器 v6.4

这是一款双语 Agent Skill，帮助助手规划适度的单 Agent 或多 Agent 工作流程。v6.4 增加了先拆交付物/工作单元并明确负责人、按需分配角色且随证据调整重点并明确交接、按风险/价值权衡独立审查，以及由单一协调人去重汇总用户/群汇报的规则。它提供指令和参考资料，并非平台集成；不会自行创建 Agent、工具、权限、后台任务或运行时行为。

## 用途

本 Skill 关注交付物、硬性要求、已核实的宿主能力、人类决策、隐私、外部行动授权、核验和停止条件。对边界清楚、低风险的任务保留轻量流程；对复杂、高风险或多阶段任务采用完整流程。每项交付物和共享写入都有明确负责人，但不要求固定团队岗位表。

**设计来源边界：**角色/关注重点启发规则根据用户对一个共享 ChatGPT 对话的描述提炼。该分享页混合用户构想、模型生成的综合建议、外部产品/研究陈述及可能的抓取噪声；这里只将其作为设计启发，不当作独立研究、平台能力依据或普遍效果保证。任何平台或研究事实性主张，都必须回到对应一手来源核验。

## 仓库结构

- `.github/skills/multi-agent-workflow-planner/SKILL.md` — 简明的双语核心规则与安全门槛。
- `.github/skills/multi-agent-workflow-planner/references/platform-capability-examples.md` — 有日期且受来源范围限定的平台文档；不是运行时测试结果。
- `.github/skills/multi-agent-workflow-planner/references/research-claim-boundaries.md` — 关于 Agent 数量、拓扑或协作效能主张的证据限制。
- `.github/skills/multi-agent-workflow-planner/references/workflow-templates.md` — 可选的任务、工作单元、变更和交接表单。
- `.github/skills/multi-agent-workflow-planner/references/behavior-checks.md` — 可选的行为测试提示；提示不代表测试已运行。
- `LICENSE-CHOICE-REQUIRED.txt` — 等待所有者决定的提示，不是许可证。

## 后续安装或导入（仅为说明）

1. Skill 文件位于 `.github/skills/multi-agent-workflow-planner/`。若所有者之后决定导入，请将其中的 `SKILL.md` 与相邻的 `references/` 目录放在一起，因为 Skill 使用相对链接。此 v6.4 本地草稿尚未安装或加载到任何宿主。README 和许可证提示保留在软件包根目录。
2. 在 GitHub 文档说明的 Copilot 项目场景中，`.github/skills/multi-agent-workflow-planner/` 是一种文档所述的发现路径。导入步骤和支持的位置应以当前宿主的文档为准。[Agent Skills 格式规范](https://agentskills.io/specification)说明文件格式；[GitHub 添加 Copilot Agent Skills 指南](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills)仅说明 GitHub 专属路径和 CLI 行为。GitHub 路径并非通用的 Agent Skills 要求。
3. 若之后导入，应确认当前宿主已加载该 Skill，且其相对参考链接均可访问。导入 Skill 不会赋予宿主新的功能或权限。

## 核验状态

- **Skill 结构：** 本地 v6.4 副本中的 `.github/skills/multi-agent-workflow-planner/` 已通过 `quick_validate.py`。
- **本地静态检查：** 通过——7 个 Markdown 文件中的 12 条相对 Markdown 链接均可解析；软件包命名/目录结构和双语版本/内容标记均通过。隐私扫描未发现本机绝对路径或类似凭证字符串。
- **来源：** 平台和研究参考资料沿用 v6.3；本次修订未刷新或独立重核其外部来源主张。
- **行为检查：**`references/behavior-checks.md` 包含回归提示。一次探索性 Cue 群组与 v6.4 相关联。可见群记录未显示所选软件包哈希、逐轮 Skill 激活情况或模型/版本；因此不能确认已加载本包，也不能证明运行时表现、稳定性或因果效果。测试群中未见实际搜索、委派或研究行动。
- **运行时/平台测试：** v6.4 未在 Cue、GitHub Copilot、Claude Code 或其他宿主内实测；不声称已验证实际运行时行为。
- **跨平台测试：** 未在 Windows 或 macOS 上测试。Markdown/YAML 格式和相对链接不保证宿主兼容。

## 宿主能力边界

Skill 仅提供指令和随附参考资料。每项任务都应核实当前宿主、账户、版本和权限。不得仅凭参考示例推断能力可用、资源共享或隔离、自动重试、后台运行或授权状态。

## 许可证与发布门槛

本仓库为公开仓库。在本次 `main` 提交中，v6.4 位于 `.github/skills/multi-agent-workflow-planner/`，作为当前活动 Skill。本仓库尚未选择许可证；见 [`LICENSE-CHOICE-REQUIRED.txt`](LICENSE-CHOICE-REQUIRED.txt)，该文件不是许可证。本次不创建 Git 标签或 GitHub Release。仓库公开可见不等于授予使用、修改或再分发权利。
