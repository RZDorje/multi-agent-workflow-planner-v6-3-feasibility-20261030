# Multi-Agent Workflow Planner v6.3 / 多 Agent 工作流程规划器 v6.3

This bilingual Agent Skill helps an assistant plan proportionate single- or multi-agent workflows. It is instruction and reference material, not a platform integration; it does not itself create agents, tools, permissions, background jobs, or runtime behavior.

本双语 Agent Skill 帮助助手规划适度的单 Agent 或多 Agent 工作流程。它只提供指令和参考资料，并非平台集成；不会自行创建 Agent、工具、权限、后台任务或运行时行为。

## What it does / 用途

The Skill focuses on deliverables, hard requirements, verified host capabilities, human decisions, privacy, external-action authorization, validation, and stopping conditions. It preserves a light path for bounded, low-risk work and a full path for complex, risky, or multi-stage work.

本 Skill 关注交付物、硬性要求、已核实的宿主能力、人类决策、隐私、外部行动授权、核验和停止条件。对边界清楚、低风险的任务保留轻量流程；对复杂、高风险或多阶段任务采用完整流程。

## Install or import / 安装或导入

1. The installable Skill is in `.github/skills/multi-agent-workflow-planner/`; keep its `SKILL.md` and adjacent `references/` directory together because it uses relative links. The README and license notice stay at the package root. / 可安装的 Skill 位于 `.github/skills/multi-agent-workflow-planner/`；其 `SKILL.md` 与相邻的 `references/` 目录必须放在一起，因为本 Skill 使用相对链接。README 和许可证提示保留在软件包根目录。
2. In the documented GitHub Copilot project context, `.github/skills/multi-agent-workflow-planner/` is the documented discovery path; follow the active host's documented import flow and supported locations. The [Agent Skills format page](https://agentskills.io/specification) describes the file format, while [GitHub's guide to adding agent skills for Copilot](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills) describes only GitHub's product-specific locations and CLI behavior. These GitHub paths are not universal Agent Skills requirements. / 在 GitHub Copilot 文档所述的项目场景中，`.github/skills/multi-agent-workflow-planner/` 是文档规定的发现路径；仍须遵循当前宿主文档所述的导入流程和支持路径。[Agent Skills 格式页面](https://agentskills.io/specification)说明文件格式；[GitHub 添加 Copilot Agent Skills 指南](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills)只说明 GitHub 产品专属路径和 CLI 行为。GitHub 路径并非通用 Agent Skills 要求。
3. Confirm that the active host loaded the Skill and that its local reference links resolve. Importing a Skill does not grant host features or permissions. / 确认当前宿主已加载 Skill，且本地参考链接可访问。导入 Skill 不会赋予宿主新的功能或权限。

## Verification status / 核验状态

- **Skill structure:** `quick_validate.py` passed for `.github/skills/multi-agent-workflow-planner/` in package revision v6.3. / **Skill 结构：** 软件包修订版 v6.3 中的 `.github/skills/multi-agent-workflow-planner/` 通过 `quick_validate.py`。
- **Sources:** 25 public source URLs were opened directly. No URL fetch failure was reported. Some long pages returned partial extraction; relevant passages were checked. The remaining page-specific limits are recorded in the references, including the Manus blog's missing year beside “Monday, September 28,” the Help Center's relative-only update label, conflicting Grok Bot approval-visibility descriptions, the ICLR poster's missing exact posting date, and absent TMLR metadata on the listed arXiv HTML page. / **来源：** 已直接打开 25 个公开来源 URL；未报告 URL 抓取失败。部分较长页面仅返回部分提取内容，但已核对相关段落。参考文件记录了仍存在的页面限制，包括 Manus 博文 “Monday, September 28” 旁未注明年份、帮助中心仅显示相对更新时间、Grok Bot 对审批可见性的说法冲突、ICLR 海报未标确切发布日期，以及所列 arXiv HTML 页面未显示 TMLR 元数据。
- **Local links and privacy:** all relative Markdown links resolve; the scan found no prohibited source-history text, absolute workspace paths, or token-like credential strings. / **本地链接与隐私：** 所有相对 Markdown 链接均可访问；扫描未发现禁止的来源历史文字、工作区绝对路径或类似凭证的字符串。
- **Runtime/platform testing:** not performed inside Cue, GitHub Copilot, Claude Code, or another host; no live runtime behavior is claimed. / **运行时/平台测试：** 未在 Cue、GitHub Copilot、Claude Code 或其他宿主内实测；不声称已验证实际运行时行为。
- **Cross-platform testing:** not performed on Windows or macOS. Markdown/YAML format and relative links do not guarantee host compatibility. / **跨平台测试：** 未在 Windows 或 macOS 上测试。Markdown/YAML 格式和相对链接不保证宿主兼容。

## Host capability boundary / 宿主能力边界

A Skill provides instructions and bundled references only. Check the active host, account, version, and permissions for each task. Do not infer availability, sharing, isolation, retries, background execution, or authorization merely from an example in a reference.

Skill 仅提供指令和随附参考资料。每项任务都应核实当前宿主、账户、版本和权限。不得仅凭参考示例推断能力可用、资源共享或隔离、自动重试、后台运行或授权状态。

## License and release gate / 许可证与发布门槛

This package has no selected license; see [`LICENSE-CHOICE-REQUIRED.txt`](LICENSE-CHOICE-REQUIRED.txt). Before any distribution, the owner must choose the applicable terms and separately approve release. This revision does not create a repository or publish the package.

本包尚未选择许可证；详见 [`LICENSE-CHOICE-REQUIRED.txt`](LICENSE-CHOICE-REQUIRED.txt)。分发前，所有者必须选择适用条款并另行批准发布。本次修订未创建仓库，也未发布本包。
