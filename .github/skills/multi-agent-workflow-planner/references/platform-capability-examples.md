# Platform Capability Examples / 平台能力示例

Use these examples to show why workflows must be checked against the active host, product surface, account, and version. A vendor page supports only what that page states for the named product; it is not independent proof of quality, security, universal availability, or current entitlement. Recheck the live host before relying on a capability.

这些示例用于说明为什么必须按当前宿主、产品形态、账户和版本核实工作流程。厂商页面只能支持该页面对指定产品明确写出的内容；它不是质量、安全性、普遍可用性或当前账户权限的独立证明。依赖某项能力前，应重新检查实时宿主。

Every entry gives the page's actual title, source type, page-stated publication/update/version date (or says that the page is undated), access date, a narrowly supported claim, and what the source does not establish. **Access date for every entry: 2026-10-30.**

每个条目均列出页面原文标题、来源类型、页面注明的发布日期/更新时间/版本（或明确注明页面未注明日期）、查阅日期、来源明确支持的主张及来源不能证明的事项。**所有条目的查阅日期：2026-10-30。**

## Contents / 目录

- [Skill format and host-specific installation / Skill 格式与宿主专属安装](#skill-format-and-host-specific-installation--skill-格式与宿主专属安装)
- [Cue and Manus: keep public claims narrow / Cue 与 Manus：限定公开主张范围](#cue-and-manus-keep-public-claims-narrow--cue-与-manus限定公开主张范围)
- [Grok Bot / Grok Bot 产品](#grok-bot--grok-bot-产品)
- [Grok Build and xAI API / Grok Build 与 xAI API](#grok-build-and-xai-api--grok-build-与-xai-api)
- [Claude Code Agent Teams / Claude Code Agent Teams](#claude-code-agent-teams--claude-code-agent-teams)
- [OpenAI Agents SDK / OpenAI Agents SDK](#openai-agents-sdk--openai-agents-sdk)
- [Evidence boundary / 证据边界](#evidence-boundary--证据边界)

## Skill format and host-specific installation / Skill 格式与宿主专属安装

### Agent Skills format / Agent Skills 格式

- **Page title / 页面原文标题:** EN: “Specification” — [Agent Skills specification page](https://agentskills.io/specification). 中文：页面原文标题为 “Specification”——[Agent Skills 规范页面](https://agentskills.io/specification)。
- **Source type / 来源类型:** EN: Public open-format specification/documentation. 中文：公开开放格式规范/文档。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Page undated; no date or specification version is shown. 中文：页面未注明日期，也未显示规范版本号。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page defines a Skill as a directory containing at least `SKILL.md`, with YAML frontmatter and Markdown instructions; it describes required `name` and `description` fields and optional metadata and reference-file conventions. 中文：该页将 Skill 定义为至少包含 `SKILL.md` 的目录，其中有 YAML frontmatter 和 Markdown 指令；页面说明必需的 `name`、`description` 字段，以及可选元数据和参考文件约定。
- **Does not establish / 来源不能证明:** EN: It does not establish universal host discovery, loading, permissions, tools, or runtime behavior. 中文：该页不能证明所有宿主都能发现或加载 Skill，也不能证明宿主具备特定权限、工具或运行时行为。

### GitHub Copilot skill locations / GitHub Copilot Skill 路径

- **Page title / 页面原文标题:** EN: “Adding agent skills for GitHub Copilot” — [GitHub Docs](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills). 中文：页面原文标题为 “Adding agent skills for GitHub Copilot”——[GitHub 文档](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills)。
- **Source type / 来源类型:** EN: Official GitHub Copilot product documentation/how-to. 中文：GitHub Copilot 官方产品文档/操作指南。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Page undated; no page version is shown. 中文：页面未注明日期，也未显示页面版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: In the documented GitHub Copilot context, the page lists `.github/skills/`, `.claude/skills/`, and `.agents/skills/` as project skill locations. It describes `gh skill` as public preview, requires GitHub CLI 2.90.0 or later, and documents `gh skill preview` for inspecting a skill. 中文：在该页所述 GitHub Copilot 场景中，页面列出 `.github/skills/`、`.claude/skills/` 和 `.agents/skills/` 作为项目 Skill 路径。页面称 `gh skill` 为公开预览功能，要求 GitHub CLI 2.90.0 或更高版本，并说明可用 `gh skill preview` 检查 Skill。
- **Does not establish / 来源不能证明:** EN: These paths or CLI behavior are not universal Agent Skills requirements and do not establish compatibility, permissions, or runtime behavior for other hosts. 中文：这些路径或 CLI 行为不是 Agent Skills 的通用要求，也不能证明其他宿主的兼容性、权限或运行时行为。

### GitHub CLI announcement / GitHub CLI 公告

- **Page title / 页面原文标题:** EN: “Manage agent skills with GitHub CLI” — [GitHub Changelog](https://github.blog/changelog/2026-04-16-manage-agent-skills-with-github-cli/). 中文：页面原文标题为 “Manage agent skills with GitHub CLI”——[GitHub 更新日志](https://github.blog/changelog/2026-04-16-manage-agent-skills-with-github-cli/)。
- **Source type / 来源类型:** EN: Official GitHub Changelog release announcement. 中文：GitHub 官方更新日志发布公告。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Published 2026-04-16; an editor’s note on the page is dated 2026-04-17. 中文：发布于 2026-04-16；页面编辑注记日期为 2026-04-17。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The announcement describes GitHub CLI skill discovery and management, says to use GitHub CLI 2.90.0 or later, and labels `gh skill` public preview. It describes GitHub's product-specific implementation of the open Agent Skills format. 中文：公告介绍 GitHub CLI 的 Skill 发现与管理功能，要求使用 GitHub CLI 2.90.0 或更高版本，并将 `gh skill` 标为公开预览。公告说明的是 GitHub 对开放 Agent Skills 格式的产品专属实现。
- **Does not establish / 来源不能证明:** EN: It does not establish universal host behavior or a publication/version date for the separate Agent Skills specification. 中文：该公告不能证明所有宿主的行为，也不能证明另一份 Agent Skills 规范的发布日期或版本。

## Cue and Manus: keep public claims narrow / Cue 与 Manus：限定公开主张范围

The public Cue page supports group chat and user-controlled agent identity/access examples. The Manus post separately describes Cue as a standalone app and has distinct Manus-only Cloud Computer and Computer Use sections. Do not merge those products or infer unmentioned sharing or isolation properties.

Cue 公开页面支持群聊及用户控制 Agent 身份/访问的说明。Manus 博文另将 Cue 描述为独立应用，并分别介绍仅属于 Manus 的 Cloud Computer 和 Computer Use。不得混淆产品，也不得推断来源未说明的共享或隔离属性。

### Cue product page / Cue 产品页

- **Page title / 页面原文标题:** EN: “Your personal agents, on Cue.” — [Cue official product page](https://cue.im/). 中文：页面原文标题为 “Your personal agents, on Cue.”——[Cue 官方产品页](https://cue.im/)。
- **Source type / 来源类型:** EN: Official Cue product page. 中文：Cue 官方产品页。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Page undated; no date or version is shown. 中文：页面未注明日期或版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page describes group chat in which users bring agents together to collaborate, and says distinct agents can have different responsibilities and keep their work in one workspace. It says each agent has its own identity, including its own phone number, email address, wallet, and computer workspace; users “set the tools and permissions” and control what an agent can access and which actions need approval. 中文：页面介绍用户可将多个 Agent 放入群聊协作，并称可为不同 Agent 分配不同职责、让其在一个工作区中开展工作。页面称每个 Agent 有自己的身份，包括电话号码、电子邮件地址、钱包和电脑工作区；用户可“设置其所需的工具和权限”，并控制 Agent 可访问的内容及哪些操作需要审批。
- **Does not establish / 来源不能证明:** EN: It does not document agent-to-agent handoff mechanics on this page; group collaboration is not itself proof of handoff. It does not establish account-level Skills sharing/import, shared files or browser state, credential sharing or isolation, a shared single computer, or extra Manus Cloud Computer allocation for Cue. It is not an independent security or runtime evaluation. 中文：该页面没有说明 Agent 之间的交接机制；群体协作本身不等于已证明交接。页面不能证明账户级 Skills 共享/导入、文件或浏览器状态共享、凭证共享或隔离、多个 Agent 共用一台电脑，或 Cue 获得额外 Manus Cloud Computer。该页也不是独立的安全性或运行时评估。

### Manus 2.0 announcement: Cue section / Manus 2.0 公告：Cue 部分

- **Page title / 页面原文标题:** EN: “Introducing Manus 2.0” — [Manus official blog](https://manus.im/blog/introducing-manus-2-0). 中文：页面原文标题为 “Introducing Manus 2.0”——[Manus 官方博客](https://manus.im/blog/introducing-manus-2-0)。
- **Source type / 来源类型:** EN: Official Manus product blog post. 中文：Manus 官方产品博客文章。
- **Publication/update/version date / 发布、更新或版本日期:** EN: The page displays “Monday, September 28” but does not print the year beside the date; the exact year is not verifiable from that visible date. 中文：页面显示 “Monday, September 28”，但日期旁未注明年份；仅凭页面可见日期无法核实确切年份。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: In its Cue section, the post calls Cue a standalone app from Manus, says each Cue agent has its own identity, email, phone, wallet, and computer, and describes several agents working in a group chat with a shared goal and handing work to one another. It says the user sets direction and makes the final call. 中文：在 Cue 部分，博文称 Cue 是 Manus 推出的独立应用，每个 Cue Agent 有自己的身份、电子邮件、电话、钱包和电脑；并描述多个 Agent 在具有共同目标的群聊中相互交接工作。博文称用户设定方向并作最终决定。
- **Does not establish / 来源不能证明:** EN: The separate Manus Cloud Computer and Computer Use sections are not evidence that Cue agents share Manus computer resources, files, browser state, or credentials, or that Cue receives an additional Cloud Computer. This page does not describe account-level Cue Skills sharing/import, or claim an isolation/security guarantee. 中文：同一博文中独立的 Manus Cloud Computer 和 Computer Use 部分，不能证明 Cue Agent 共享 Manus 电脑资源、文件、浏览器状态或凭证，也不能证明 Cue 获得额外 Cloud Computer。该页没有说明账户级 Cue Skills 共享/导入，也没有声称提供隔离/安全保证。

### Manus Help Center: Skills configuration boundary / Manus 帮助中心：Skills 配置边界

- **Page title / 页面原文标题:** EN: “How to Share and Use Skills in Manus?” — [Manus Help Center](https://help.manus.im/en/articles/14753565-how-to-share-and-use-skills-in-manus). 中文：页面原文标题为 “How to Share and Use Skills in Manus?”——[Manus 帮助中心](https://help.manus.im/en/articles/14753565-how-to-share-and-use-skills-in-manus)。
- **Source type / 来源类型:** EN: Official Manus Help Center article. 中文：Manus 官方帮助中心文章。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Exact date not shown; the page says “Updated over 3 weeks ago.” 中文：未显示确切日期；页面标注 “Updated over 3 weeks ago”。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The article describes Skill sharing/import methods for Manus and explicitly says Cue and Manus have separate Skills configurations; Skills created or imported in Manus are not automatically available in Cue, and Cue must be configured separately. 中文：文章介绍 Manus 的 Skill 共享/导入方式，并明确称 Cue 与 Manus 的 Skills 配置彼此分开；在 Manus 中创建或导入的 Skills 不会自动在 Cue 中提供，Cue 需要单独配置。
- **Does not establish / 来源不能证明:** EN: It does not explain Cue-internal Skills sharing, Cue account-level import workflows, or any broader computer/file/browser/credential-sharing or isolation relationship. 中文：该文章没有说明 Cue 内部的 Skills 共享方式、Cue 账户级导入流程，也没有说明更广泛的电脑/文件/浏览器/凭证共享或隔离关系。

## Grok Bot / Grok Bot 产品

These are separate Grok Bot documentation pages. One page's approval-visibility statement conflicts with another's; retain the conflict rather than inventing a unified rule.

以下是彼此独立的 Grok Bot 文档页面。其中一页关于审批可见性的说法与另一页冲突；应保留该冲突，不得编造统一规则。

### Grok Bot: group chat and collaboration / Grok Bot：群聊与协作

- **Page title / 页面原文标题:** EN: “Message and collaborate” — [Grok Bot documentation](https://docs.x.ai/grok-bot/chat-and-collaboration). 中文：页面原文标题为 “Message and collaborate”——[Grok Bot 文档](https://docs.x.ai/grok-bot/chat-and-collaboration)。
- **Source type / 来源类型:** EN: Official Grok Bot product documentation/user guide. 中文：Grok Bot 官方产品文档/用户指南。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Page undated. 中文：页面未注明日期。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page describes group chats with two to six Bots, asynchronous Bot-to-Bot handoffs, and suggests assigning one owner per stage. It says group-chat approval requests do not appear in the group. 中文：页面介绍由 2 至 6 个 Bot 组成的群聊、Bot 之间的异步交接，并建议每个阶段指定一名负责人。页面称群聊中的审批请求不会显示在群组中。
- **Does not establish / 来源不能证明:** EN: It does not establish general handoff reliability or security. Its approval-visibility statement conflicts with the separate “Approvals, security, and privacy” page; the public sources do not resolve that conflict. 中文：该页不能证明交接普遍可靠或安全。其审批可见性说法与另一份 “Approvals, security, and privacy” 页面冲突；公开来源没有解决该冲突。

### Grok Bot: Skills and routines / Grok Bot：Skills 与 routines

- **Page title / 页面原文标题:** EN: “Skills and routines” — [Grok Bot documentation](https://docs.x.ai/grok-bot/skills-routines-and-automations). 中文：页面原文标题为 “Skills and routines”——[Grok Bot 文档](https://docs.x.ai/grok-bot/skills-routines-and-automations)。
- **Source type / 来源类型:** EN: Official Grok Bot product documentation/user guide. 中文：Grok Bot 官方产品文档/用户指南。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Last updated 2026-10-28; no version shown. 中文：最后更新于 2026-10-28；未标版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page distinguishes reusable Skill instructions from one Bot's scheduled or event-triggered routines and says routines run in the cloud. 中文：页面区分可复用的 Skill 指令与单个 Bot 按计划或事件触发的 routine，并称 routines 在云端运行。
- **Does not establish / 来源不能证明:** EN: It does not establish equivalence to Grok Build Skills/subagents or the xAI API's multi-agent feature, or guarantee routine reliability or outcomes. 中文：该页不能证明其功能等同于 Grok Build 的 Skills/subagents 或 xAI API 多 Agent 功能，也不能保证 routine 的可靠性或结果。

### Grok Bot: approvals, security, and privacy / Grok Bot：审批、安全与隐私

- **Page title / 页面原文标题:** EN: “Approvals, security, and privacy” — [Grok Bot documentation](https://docs.x.ai/grok-bot/approvals-security-and-privacy). 中文：页面原文标题为 “Approvals, security, and privacy”——[Grok Bot 文档](https://docs.x.ai/grok-bot/approvals-security-and-privacy)。
- **Source type / 来源类型:** EN: Official Grok Bot product documentation/user guide. 中文：Grok Bot 官方产品文档/用户指南。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Last updated 2026-10-28; no version shown. 中文：最后更新于 2026-10-28；未标版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page says one user account has one shared cloud computer for its Bot roster, with files, browser sessions, and command-line credentials available across that roster. It says only the person whose message is being answered can approve a group-chat request and others can see whose approval is pending. 中文：页面称每个用户账户的 Bot 阵列共用一台云电脑，其文件、浏览器会话和命令行凭证可由该阵列访问。页面称群聊请求只有被回复消息所属用户可以批准，其他人可以看到待谁批准。
- **Does not establish / 来源不能证明:** EN: This vendor page is not an independent security audit. Its group-approval visibility account conflicts with “Message and collaborate”; do not present either page's approval statement as a reconciled rule. 中文：该厂商页面不是独立安全审计。其群聊审批可见性说法与 “Message and collaborate” 冲突；不得将任一页面的审批说法写成已调和的统一规则。

## Grok Build and xAI API / Grok Build 与 xAI API

Do not transfer claims among Grok Bot, Grok Build, and the xAI API.

不得在 Grok Bot、Grok Build 和 xAI API 之间移植能力主张。

### Grok Build: Skills, Plugins & Marketplaces / Grok Build：Skills、插件与市场

- **Page title / 页面原文标题:** EN: “Skills, Plugins & Marketplaces” — [Grok Build documentation](https://docs.x.ai/build/features/skills-plugins-marketplaces). 中文：页面原文标题为 “Skills, Plugins & Marketplaces”——[Grok Build 文档](https://docs.x.ai/build/features/skills-plugins-marketplaces)。
- **Source type / 来源类型:** EN: Official Grok Build product/engineering documentation. 中文：Grok Build 官方产品/工程文档。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Last updated 2026-08-11; no version shown. 中文：最后更新于 2026-08-11；未标版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page describes Build Skills as reusable folders with Markdown instructions, scripts, and resources; plugins can add skills, agents, hooks, MCP servers, and LSP servers, and the TUI Marketplace browses and installs plugins from configured sources. 中文：页面将 Build Skills 描述为包含 Markdown 指令、脚本和资源的可复用文件夹；插件可添加 skills、agents、hooks、MCP servers 和 LSP servers；TUI Marketplace 可浏览并从已配置来源安装插件。
- **Does not establish / 来源不能证明:** EN: It does not establish that these are Grok Bot Skills/routines, Bot shared-computer features, or the xAI API multi-agent feature. It is not independent compatibility, safety, or performance validation. 中文：该页不能证明这些功能就是 Grok Bot Skills/routines、Bot 共用电脑功能或 xAI API 多 Agent 功能，也不是独立的兼容性、安全性或性能验证。

### Grok Build: Subagents / Grok Build：Subagents

- **Page title / 页面原文标题:** EN: “Subagents” — [Grok Build documentation](https://docs.x.ai/build/features/subagents). 中文：页面原文标题为 “Subagents”——[Grok Build 文档](https://docs.x.ai/build/features/subagents)。
- **Source type / 来源类型:** EN: Official Grok Build product/engineering documentation. 中文：Grok Build 官方产品/工程文档。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Last updated 2026-07-21; no version shown. 中文：最后更新于 2026-07-21；未标版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page describes Build subagents as independent child sessions with their own context that return a summary to the parent when finished; it lists general-purpose, explore, and plan types. 中文：页面将 Build subagents 描述为拥有自身上下文的独立子会话，结束后向 parent 返回摘要；页面列出 general-purpose、explore 和 plan 类型。
- **Does not establish / 来源不能证明:** EN: It does not establish equivalence to Grok Bot group-chat Bots or xAI API agents, nor a universal numeric limit or isolation guarantee. 中文：该页不能证明其等同于 Grok Bot 群聊 Bot 或 xAI API agents，也不能证明通用数量上限或隔离保证。

### xAI API: Multi Agent / xAI API：Multi Agent

- **Page title / 页面原文标题:** EN: “Multi Agent” — [xAI API documentation](https://docs.x.ai/developers/model-capabilities/text/multi-agent). 中文：页面原文标题为 “Multi Agent”——[xAI API 文档](https://docs.x.ai/developers/model-capabilities/text/multi-agent)。
- **Source type / 来源类型:** EN: Official xAI API documentation/model-capability reference. 中文：xAI 官方 API 文档/模型能力说明。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Last updated 2026-10-10; feature marked beta; no version shown. 中文：最后更新于 2026-10-10；功能标记为 beta；未标版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page documents a beta Realtime Multi-agent Research API feature, with 4- or 16-agent configurations and leader-agent synthesis; it warns that the API interface and behavior may change. 中文：页面介绍 beta 版 Realtime Multi-agent Research API 功能，支持配置 4 或 16 个 agents 并由 leader agent 汇总；页面提醒 API 接口和行为可能变化。
- **Does not establish / 来源不能证明:** EN: Configuration counts are not measured optimal team sizes. The API page does not establish Grok Bot group-chat or Grok Build subagent behavior, or a final stable API contract. 中文：配置数量不是经测量得出的最优团队规模。该 API 页面不能证明 Grok Bot 群聊或 Grok Build subagent 的行为，也不能证明 API 契约已最终稳定。

## Claude Code Agent Teams / Claude Code Agent Teams

- **Page title / 页面原文标题:** EN: “Orchestrate teams of Claude Code sessions” — [Claude Code documentation](https://code.claude.com/docs/en/agent-teams). 中文：页面原文标题为 “Orchestrate teams of Claude Code sessions”——[Claude Code 文档](https://code.claude.com/docs/en/agent-teams)。
- **Source type / 来源类型:** EN: Official Claude Code product/engineering documentation. 中文：Claude Code 官方产品/工程文档。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Page undated; version requirements for individual features are not page publication dates. 中文：页面未注明日期；个别功能的版本要求不是页面发布日期。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page describes Agent Teams as experimental and disabled by default, with independent teammate sessions and direct messages. It recommends starting most workflows with 3–5 teammates. Shared task-list use is conditional on Task tools; the page also says there is one team per session and teams cannot be shared across sessions. 中文：页面称 Agent Teams 属于实验性功能且默认关闭，teammate 会话彼此独立并可直接发送消息；页面建议多数工作流先从 3–5 个 teammate 开始。共享任务列表以具备 Task tools 为条件；页面还称每个会话只有一个 team，且 team 不能跨会话共享。
- **Does not establish / 来源不能证明:** EN: The 3–5 suggestion is Claude Code product guidance, not an independent benchmark or general optimum. It does not establish that non-interactive sessions (including Agent SDK sessions) spawn teammates, nor universal team behavior on other hosts. 中文：3–5 人建议是 Claude Code 产品指导，不是独立基准或通用最优值。该页不能证明非交互会话（包括 Agent SDK sessions）会启动 teammate，也不能证明其他宿主具有相同团队行为。

## OpenAI Agents SDK / OpenAI Agents SDK

### Agent orchestration / Agent orchestration

- **Page title / 页面原文标题:** EN: “Agent orchestration” — [OpenAI Agents SDK documentation](https://openai.github.io/openai-agents-python/multi_agent/). 中文：页面原文标题为 “Agent orchestration”——[OpenAI Agents SDK 文档](https://openai.github.io/openai-agents-python/multi_agent/)。
- **Source type / 来源类型:** EN: Official OpenAI Agents SDK for Python documentation. 中文：OpenAI Agents SDK for Python 官方文档。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Page undated; no documentation or SDK version is shown. 中文：页面未注明日期，也未显示文档或 SDK 版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page distinguishes agents-as-tools, where a manager retains control, from handoffs, where a specialist becomes the active agent for the rest of the turn. It describes application-code orchestration of independent work, including `asyncio.gather`. 中文：页面区分 agents-as-tools（manager 保持控制权）与 handoff（specialist 在本轮剩余过程中成为当前 agent）。页面介绍通过应用代码编排独立工作，包括使用 `asyncio.gather`。
- **Does not establish / 来源不能证明:** EN: It does not establish automatic Runner-level parallel scheduling, durable background work, or equivalent behavior on no-code hosts or other platforms. 中文：该页不能证明 Runner 会自动并行调度、提供持久后台运行，或无代码宿主及其他平台具有相同行为。

### Human-in-the-loop / Human-in-the-loop

- **Page title / 页面原文标题:** EN: “Human-in-the-loop” — [OpenAI Agents SDK approvals guide](https://openai.github.io/openai-agents-python/human_in_the_loop/). 中文：页面原文标题为 “Human-in-the-loop”——[OpenAI Agents SDK 审批指南](https://openai.github.io/openai-agents-python/human_in_the_loop/)。
- **Source type / 来源类型:** EN: Official OpenAI Agents SDK for Python documentation. 中文：OpenAI Agents SDK for Python 官方文档。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Page undated; no documentation or SDK version is shown. 中文：页面未注明日期，也未显示文档或 SDK 版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page describes sensitive tool calls pausing a run for approval, recording an interruption, saving state as `RunState`, then approving/rejecting and resuming with the original top-level agent. It also describes programmatic approval callbacks for some tool types. 中文：页面介绍敏感工具调用可暂停运行并等待审批、记录 interruption、将状态保存为 `RunState`，之后批准/拒绝并使用原始顶层 agent 恢复；页面还说明部分工具类型支持程序化审批回调。
- **Does not establish / 来源不能证明:** EN: It does not establish that every tool call needs approval, that every approval must be manual, or that unrelated platforms use the same pause/resume flow. 中文：该页不能证明每次工具调用都需要审批、每项审批都必须由人工完成，或其他平台使用相同暂停/恢复流程。

### Running agents / Running agents

- **Page title / 页面原文标题:** EN: “Running agents” — [OpenAI Agents SDK Runner guide](https://openai.github.io/openai-agents-python/running_agents/). 中文：页面原文标题为 “Running agents”——[OpenAI Agents SDK Runner 指南](https://openai.github.io/openai-agents-python/running_agents/)。
- **Source type / 来源类型:** EN: Official OpenAI Agents SDK for Python documentation. 中文：OpenAI Agents SDK for Python 官方文档。
- **Publication/update/version date / 发布、更新或版本日期:** EN: Page undated; no documentation or SDK version is shown. 中文：页面未注明日期，也未显示文档或 SDK 版本。
- **Access date / 查阅日期:** EN: 2026-10-30. 中文：2026-10-30。
- **Exact supported claim / 来源明确支持的主张:** EN: The page documents asynchronous `Runner.run()`, synchronous `Runner.run_sync()`, and `Runner.run_streamed()`, and describes the per-run loop through final output, handoff, tool calls, or turn-limit errors. 中文：页面记录异步 `Runner.run()`、同步 `Runner.run_sync()` 和 `Runner.run_streamed()`，并说明每次运行如何循环处理最终输出、handoff、工具调用或轮次上限错误。
- **Does not establish / 来源不能证明:** EN: It does not establish that Runner itself schedules independent agents in parallel; the separate orchestration page assigns parallel task execution to application code. It does not establish lifecycle behavior for unrelated platforms. 中文：该页不能证明 Runner 自身会并行调度独立 agents；另一份编排页面将并行任务执行交由应用代码处理。该页不能证明其他平台具有相同生命周期行为。

## Evidence boundary / 证据边界

Use a vendor page as evidence about that named page and product surface, not as a general rule for agent systems. A source's silence is not evidence that a feature is impossible; when public documentation does not establish a Cue-specific detail, omit the claim or label it **not publicly verified**. Do not claim that importing this Skill enables any listed platform capability.

厂商页面只能作为关于该页面所述产品形态的证据，不是 Agent 系统的通用规律。来源未提及某项能力，不代表该能力不可能；公开文档未能证明某项 Cue 特定细节时，应删除该主张或明确标为**未获公开核实**。不得声称导入本 Skill 即可启用任何所列平台能力。
