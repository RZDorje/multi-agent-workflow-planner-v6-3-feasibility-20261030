[简体中文](README.zh-CN.md)

# Multi-Agent Workflow Planner v6.4

This bilingual Agent Skill helps an assistant plan proportionate single- or multi-agent workflows. v6.4 adds deliverable/work-unit-first ownership, roles assigned only as needed with evidence-responsive focus shifts and explicit handoffs, risk/value-based independent review, and one coordinator for deduplicated user/group reporting. It provides instructions and reference material; it is not a platform integration and does not itself create agents, tools, permissions, background jobs, or runtime behavior.

## What it does

The Skill focuses on deliverables, hard requirements, verified host capabilities, human decisions, privacy, external-action authorization, validation, and stopping conditions. It preserves a light path for bounded, low-risk work and a full path for complex, risky, or multi-stage work. It assigns a clear owner to each deliverable and shared write without requiring a fixed team roster.

**Design-source boundary:** The role/focus heuristic was distilled from the user's description of a shared ChatGPT conversation. That page mixes user ideas, model-generated synthesis, external product/research statements, and possible extraction noise. It is used only as design inspiration—not as independent research, evidence of platform capabilities, or a general-effect guarantee. Any factual platform or research statement must be checked against the corresponding primary source.

## Repository layout

- `.github/skills/multi-agent-workflow-planner/SKILL.md` — concise bilingual core rules and safety gates.
- `.github/skills/multi-agent-workflow-planner/references/platform-capability-examples.md` — dated, source-bounded platform documentation; not runtime test results.
- `.github/skills/multi-agent-workflow-planner/references/research-claim-boundaries.md` — evidence limits for claims about agent counts, topologies, or collaboration effectiveness.
- `.github/skills/multi-agent-workflow-planner/references/workflow-templates.md` — optional task, work-unit, change, and handoff forms.
- `.github/skills/multi-agent-workflow-planner/references/behavior-checks.md` — optional behavior-test prompts; prompts are not evidence that tests were run.
- `LICENSE-CHOICE-REQUIRED.txt` — pending decision notice, not a license.

## Future install or import (instructions only)

1. The Skill files are in `.github/skills/multi-agent-workflow-planner/`. Keep its `SKILL.md` and adjacent `references/` directory together if an owner later chooses to import it, because it uses relative links. This v6.4 local draft has not been installed or loaded in a host. The README and license notice remain at the package root.
2. In the GitHub Copilot project context documented by GitHub, `.github/skills/multi-agent-workflow-planner/` is a documented discovery path. Follow the active host's documentation for import steps and supported locations. The [Agent Skills format specification](https://agentskills.io/specification) describes the file format, while [GitHub's guide to adding agent skills for Copilot](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills) describes only GitHub-specific locations and CLI behavior. GitHub paths are not universal Agent Skills requirements.
3. For any later import, confirm that the active host loaded the Skill and that its relative reference links resolve. Importing a Skill does not grant the host new features or permissions.

## Verification status

- **Skill structure:** `quick_validate.py` passed for `.github/skills/multi-agent-workflow-planner/` in the local v6.4 copy.
- **Local static checks:** Passed — all 12 relative Markdown links in 7 Markdown files resolve; package naming/layout and bilingual version/content markers pass. The privacy scan found no absolute local paths or credential-like strings.
- **Sources:** The platform and research references are carried forward from v6.3. This revision did not refresh or independently revalidate their external-source claims.
- **Behavior checks:** `references/behavior-checks.md` contains regression prompts. One exploratory Cue group was associated with v6.4. The visible transcript did not expose the selected package hash, per-turn Skill activation, or model/version; therefore, it does not confirm that this package was loaded or establish runtime behavior, stability, or causal effect. No actual search, delegation, or research was visible in the test group.
- **Runtime/platform testing:** Not performed for v6.4 inside Cue, GitHub Copilot, Claude Code, or another host; no live runtime behavior is claimed.
- **Cross-platform testing:** Not performed on Windows or macOS. Markdown/YAML format and relative links do not guarantee host compatibility.

## Host capability boundary

A Skill provides instructions and bundled references only. Check the active host, account, version, and permissions for each task. Do not infer availability, sharing, isolation, retries, background execution, or authorization merely from an example in a reference.

## License and release gate

This repository is public. The v6.4 package is the active Skill at `.github/skills/multi-agent-workflow-planner/` on `main` in this commit. No license has been selected; see [`LICENSE-CHOICE-REQUIRED.txt`](LICENSE-CHOICE-REQUIRED.txt), which is not a license. This change creates no Git tag or GitHub Release. Public visibility does not grant permission to use, modify, or redistribute the files.
