[English](README.md)

# 多 Agent 工作流程规划器 v6.3

这是一款双语 Agent Skill，帮助助手规划适度的单 Agent 或多 Agent 工作流程。它提供指令和参考资料，并非平台集成；不会自行创建 Agent、工具、权限、后台任务或运行时行为。

## 用途

本 Skill 关注交付物、硬性要求、已核实的宿主能力、人类决策、隐私、外部行动授权、核验和停止条件。对边界清楚、低风险的任务保留轻量流程；对复杂、高风险或多阶段任务采用完整流程。

## 安装或导入

1. 可安装的 Skill 位于 `.github/skills/multi-agent-workflow-planner/`。请将其中的 `SKILL.md` 与相邻的 `references/` 目录放在一起，因为 Skill 使用相对链接。README 和许可证提示保留在软件包根目录。
2. 在 GitHub 文档说明的 Copilot 项目场景中，`.github/skills/multi-agent-workflow-planner/` 是一种文档所述的发现路径。导入步骤和支持的位置应以当前宿主的文档为准。[Agent Skills 格式规范](https://agentskills.io/specification)说明文件格式；[GitHub 添加 Copilot Agent Skills 指南](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills)仅说明 GitHub 专属路径和 CLI 行为。GitHub 路径并非通用的 Agent Skills 要求。
3. 确认当前宿主已加载该 Skill，且其相对参考链接均可访问。导入 Skill 不会赋予宿主新的功能或权限。

## 核验状态

- **Skill 结构：** 软件包修订版 v6.3 中的 `.github/skills/multi-agent-workflow-planner/` 已通过 `quick_validate.py`。
- **来源：** 已直接打开 25 个公开来源 URL，未报告 URL 抓取失败。部分较长页面仅返回部分提取内容，但已核对相关段落。参考文件记录了仍存在的页面限制，包括 Manus 博文 “Monday, September 28” 旁未注明年份、帮助中心仅显示相对更新时间、Grok Bot 对审批可见性的说法冲突、ICLR 海报未标确切发布日期，以及所列 arXiv HTML 页面未显示 TMLR 元数据。
- **本地链接与隐私：** 所有相对 Markdown 链接均可访问。扫描未发现禁止的来源历史文字、工作区绝对路径或类似凭证的字符串。
- **运行时/平台测试：** 未在 Cue、GitHub Copilot、Claude Code 或其他宿主内实测；不声称已验证实际运行时行为。
- **跨平台测试：** 未在 Windows 或 macOS 上测试。Markdown/YAML 格式和相对链接不保证宿主兼容。

## 宿主能力边界

Skill 仅提供指令和随附参考资料。每项任务都应核实当前宿主、账户、版本和权限。不得仅凭参考示例推断能力可用、资源共享或隔离、自动重试、后台运行或授权状态。

## 许可证与发布门槛

本软件包尚未选择许可证；详见 [`LICENSE-CHOICE-REQUIRED.txt`](LICENSE-CHOICE-REQUIRED.txt)。目前本包保存在私有可行性测试仓库中，尚未公开发布。分发前，所有者必须选择适用条款并另行批准发布。本次 README 本地化不选择许可证，也不授权公开发布。
