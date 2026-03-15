[中文版](./README.zh-CN.md)

# ICSkill

Curated AI Agent Skills for IC Design.

## What is this

ICSkill is a collection of verified AI Agent skill packs for chip design teams, compatible with Claude Code, Codex, OpenClaw, and other Agent platforms.

Each Skill is a self-contained task SOP package — with execution steps, constraints, references, and validation methods — enabling Agents to reliably perform specific R&D tasks.

## Principles

- **Secure & Controlled**: Every Skill declares its data boundaries and permission requirements
- **Strictly Curated**: Acceptance criteria prioritize verifiability and auditability
- **Production-Ready**: Not demos or proofs-of-concept — tools that fit into real R&D workflows

## Use Cases

Common tasks in chip design R&D, such as:
- Regression triage
- Spec-to-testplan conversion
- CDC/RDC report processing
- ECO impact analysis
- IP onboarding
- Release note generation

## Skill Structure

```
skills/
  <skill-name>/
    SKILL.md          # Scope, steps, constraints, output requirements
    references/       # Specs, templates, examples
    scripts/          # Executable logic
    assets/           # Samples, configs, resources
```

## License

MIT
