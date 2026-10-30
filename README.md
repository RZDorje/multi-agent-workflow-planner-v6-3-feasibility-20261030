[简体中文](README.zh-CN.md)

# Multi-Agent Workflow Planner v6.3

This bilingual Agent Skill helps an assistant plan proportionate single- or multi-agent workflows. It provides instructions and reference material; it is not a platform integration and does not itself create agents, tools, permissions, background jobs, or runtime behavior.

## What it does

The Skill focuses on deliverables, hard requirements, verified host capabilities, human decisions, privacy, external-action authorization, validation, and stopping conditions. It preserves a light path for bounded, low-risk work and a full path for complex, risky, or multi-stage work.

## Install or import

1. The installable Skill is in `.github/skills/multi-agent-workflow-planner/`. Keep its `SKILL.md` and adjacent `references/` directory together because it uses relative links. The README and license notice remain at the package root.
2. In the GitHub Copilot project context documented by GitHub, `.github/skills/multi-agent-workflow-planner/` is a documented discovery path. Follow the active host's documentation for import steps and supported locations. The [Agent Skills format specification](https://agentskills.io/specification) describes the file format, while [GitHub's guide to adding agent skills for Copilot](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills) describes only GitHub-specific locations and CLI behavior. GitHub paths are not universal Agent Skills requirements.
3. Confirm that the active host loaded the Skill and that its relative reference links resolve. Importing a Skill does not grant the host new features or permissions.

## Verification status

- **Skill structure:** `quick_validate.py` passed for `.github/skills/multi-agent-workflow-planner/` in package revision v6.3.
- **Sources:** 25 public source URLs were opened directly, with no URL fetch failures reported. Some long pages returned partial extraction; relevant passages were checked. Remaining page-specific limits are recorded in the references, including the Manus blog's missing year beside “Monday, September 28,” the Help Center's relative-only update label, conflicting Grok Bot approval-visibility descriptions, the ICLR poster's missing exact posting date, and absent TMLR metadata on the listed arXiv HTML page.
- **Local links and privacy:** All relative Markdown links resolve. The scan found no prohibited source-history text, absolute workspace paths, or token-like credential strings.
- **Runtime/platform testing:** Not performed inside Cue, GitHub Copilot, Claude Code, or another host; no live runtime behavior is claimed.
- **Cross-platform testing:** Not performed on Windows or macOS. Markdown/YAML format and relative links do not guarantee host compatibility.

## Host capability boundary

A Skill provides instructions and bundled references only. Check the active host, account, version, and permissions for each task. Do not infer availability, sharing, isolation, retries, background execution, or authorization merely from an example in a reference.

## License and release gate

This package has no selected license; see [`LICENSE-CHOICE-REQUIRED.txt`](LICENSE-CHOICE-REQUIRED.txt). The repository is currently publicly viewable; no license has been selected, and no versioned release has been published. Before any distribution, the owner must choose the applicable terms and separately approve release. This README localization does not select a license or authorize public release.
