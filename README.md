<div align="center">

# AI App Studio

**One master skill for planning, designing, building, and validating Android and desktop applications.**

`1 Master Skill` · `9 Internal Modules` · `Claude Code` · `OpenCode`

</div>

---

## About

Build maintainable native or cross-platform applications with polished user experience, appropriate architecture, reliable device integration, and verified builds.

This repository exposes one discoverable skill: `ai-app-studio`. Specialist playbooks live inside that skill's `references/` directory and are loaded by the master workflow as needed. You do not select each module separately.

## Quick start

### Project-local use

Copy this repository's `.claude/skills/ai-app-studio/` folder into the target project's `.claude/skills/` directory. Then invoke the master skill from your compatible coding agent.

### Claude Code

```text
/ai-app-studio
```

### OpenCode

```text
@ai-app-studio
```

Agent discovery behavior can vary by installed version and configuration. Confirm the skill appears in the agent's available skill list before relying on it.

## Internal specialist modules

| Module | Role |
|---|---|
| `android-app-engineer` | Internal specialist reference |
| `desktop-app-engineer` | Internal specialist reference |
| `android-architecture-engineer` | Internal specialist reference |
| `android-performance-engineer` | Internal specialist reference |
| `android-ai-app-engineer` | Internal specialist reference |
| `android-voice-engineer` | Internal specialist reference |
| `human-centered-product-design` | Shared human-centered quality reference |
| `design-quality-critic` | Shared human-centered quality reference |
| `product-experience-engineer` | Shared human-centered quality reference |

## Repository layout

```text
ai-app-studio/
├── .claude/skills/ai-app-studio/
│   ├── SKILL.md
│   ├── references/
│   ├── scripts/
│   ├── templates/
│   └── assets/
├── scripts/
├── README.md
├── README_BN.md
└── AGENTS.md
```

## Validation

Run: `python scripts/validate_pack.py`

The validator checks the master skill, expected reference files, frontmatter, basic link integrity, and accidental secrets. It does not prove provider/API availability or guarantee production behavior.

## Safety and service requirements

This repository contains agent instructions, reference playbooks, templates, and helper scripts. It is not itself a model, API subscription, cloud runtime, media-generation engine, or deployment service. Actual capabilities depend on tools, credentials, permissions, provider terms, quotas, dependencies, and hardware configured in your environment. Never commit secrets.

## Contribution and updates

Keep the master skill as the sole discoverable entry point. Add new specialist knowledge as internal references unless there is a deliberate decision to expose a new independent skill. Update the manifest and validation checks whenever modules change.
