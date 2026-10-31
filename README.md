[简体中文](README.zh-CN.md)

# Multi-Agent Workflow Planner v6.5

This bilingual Agent Skill helps an assistant plan proportionate single- or multi-agent workflows. v6.5 adds a concise, traceable current-state card for optional use in multi-phase/shared work; requires phase transitions and resumptions to refresh the state against original instructions and applicable rules; clarifies that the accountable coordinator may also handle a low-conflict work unit; and records bounded evidence about context, verification, coordination patterns, and role prompts. It provides instructions and references; it is not a platform integration and does not itself create agents, tools, permissions, background jobs, or runtime behavior.

## What it does

The Skill focuses on deliverables, hard requirements, verified host capabilities, human decisions, privacy, external-action authorization, validation, and stopping conditions. It preserves a light path for bounded, low-risk work and a full path for complex, risky, or multi-stage work. It assigns a clear owner to each deliverable and shared write without requiring a fixed team roster. A specific team charter's primary responsibilities are honored while compatible duties may be combined; a general-purpose workflow maps responsibilities to deliverables rather than imposing fixed seats.

**Design-source boundary:** The role/focus heuristic was distilled from the user's description of a shared ChatGPT conversation. That page mixes user ideas, model-generated synthesis, external product/research statements, and possible extraction noise. It is used only as design inspiration—not as independent research, evidence of platform capabilities, or a general-effect guarantee. Factual platform and research statements are bounded to their linked sources; the v6.5 research reference distinguishes retrieval-position studies, instruction-following evaluations, specific context-compaction experiments, vendor system examples, and framework-specific results. The coordination rules are design recommendations, not causal proof that one role arrangement always works best.

## Repository layout

- `.github/skills/multi-agent-workflow-planner/SKILL.md` — concise bilingual core rules and safety gates.
- `.github/skills/multi-agent-workflow-planner/references/platform-capability-examples.md` — dated, source-bounded platform documentation; not runtime test results.
- `.github/skills/multi-agent-workflow-planner/references/research-claim-boundaries.md` — evidence limits for claims about agent counts, topologies, context, roles, and collaboration effectiveness.
- `.github/skills/multi-agent-workflow-planner/references/workflow-templates.md` — optional task, work-unit, change, handoff, and current-state-card forms.
- `.github/skills/multi-agent-workflow-planner/references/behavior-checks.md` — optional behavior-test prompts; prompts are not evidence that tests were run.
- `LICENSE-CHOICE-REQUIRED.txt` — pending decision notice, not a license.

## Future install or import (instructions only)

1. The Skill files are in `.github/skills/multi-agent-workflow-planner/`. Keep its `SKILL.md` and adjacent `references/` directory together if an owner later chooses to import it, because it uses relative links. This v6.5 local draft has not been installed or loaded in a host. The README and license notice remain at the package root.
2. In the GitHub Copilot project context documented by GitHub, `.github/skills/multi-agent-workflow-planner/` is a documented discovery path. Follow the active host's documentation for import steps and supported locations. The [Agent Skills format specification](https://agentskills.io/specification) describes the file format, while [GitHub's guide to adding agent skills for Copilot](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills) describes only GitHub-specific locations and CLI behavior. GitHub paths are not universal Agent Skills requirements.
3. For any later import, confirm that the active host loaded the Skill and that its relative reference links resolve. Importing a Skill does not grant the host new features or permissions.

## Verification status

- **Skill structure:** `quick_validate.py` passed for the v6.5 Skill directory in this local copy.
- **Local static checks:** Passed — 7 Markdown files; all 12 relative Markdown links resolve; all 15 behavior checks have paired English/Chinese prompts and expectations; version/language markers, package layout, and privacy/absolute-path scan pass. v6.3/v6.4 hashes remain unchanged, and v6.5 contains no copied Git metadata.
- **Source links:** All 8 newly added source links are reachable. Across the package, 30 unique external Markdown links were checked; one carried-forward OpenAI guide returned HTTP 403 to the direct link checker, but its title and page content were successfully retrieved through the public-page reader. No broken external link was identified. The linked summaries do not establish universal coordinator-role, context-length, or multi-agent causal effects.
- **Behavior checks:** `references/behavior-checks.md` contains regression prompts. A v4 short Cue screen designated one new group for the v6.5 bilingual candidate; the visible group transcript did not show the selected package hash or per-turn Skill activation. The screen therefore does not confirm that this package was loaded or establish runtime behavior, stability, or causal effect. No actual search, delegation, or research was visible in the test group.
- **Runtime/platform testing:** Not performed for v6.5 inside Cue, GitHub Copilot, Claude Code, or another host; no live runtime behavior is claimed.
- **Cross-platform testing:** Not performed on Windows or macOS. Markdown/YAML format and relative links do not guarantee host compatibility.

## Host capability boundary

A Skill provides instructions and bundled references only. Check the active host, account, version, and permissions for each task. Do not infer availability, sharing, isolation, retries, background execution, or authorization merely from an example in a reference.

## License and release gate

This repository is public. The v6.5 bilingual package is the active Skill at `.github/skills/multi-agent-workflow-planner/` on `main`. No license has been selected; see [`LICENSE-CHOICE-REQUIRED.txt`](LICENSE-CHOICE-REQUIRED.txt), which is not a license. This change creates no Git tag or GitHub Release. Public visibility does not grant permission to use, modify, or redistribute the files.
