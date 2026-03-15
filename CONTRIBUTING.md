[中文版](./CONTRIBUTING.zh-CN.md)

# Contributing

## Skill Acceptance Criteria

Every Skill submitted to ICSkill undergoes a security review before being merged.

### Submission Requirements

1. Each Skill goes in its own `skills/<skill-name>/` directory
2. Must include a `SKILL.md` that declares:
   - Target use cases
   - Execution steps
   - Data access scope (which files/directories are read)
   - Tool invocation scope (which commands are executed, whether network requests are made)
   - Output format and boundaries
3. Skills imported from external sources must include an `ORIGIN.md` with source URL, version, and upstream reference
4. All scripts must be readable — no obfuscation

### Security Review

All Skills are reviewed before merge. Reviews are conducted by the maintainer team. Specific review criteria are not public.

Review outcomes:
- **Approved**: Merged into the main branch
- **Changes Requested**: Modification requirements noted in the PR
- **Rejected**: Does not meet acceptance criteria

### Safety Tiers

Each approved Skill is labeled with a safety tier:
- `safe` — Read-only analysis and generation; no command execution or file writes
- `controlled` — Involves command execution or file writes, with explicit constraints
- `review-required` — Involves elevated permissions; human confirmation recommended per use

### Update Policy

Skills imported from external sources are not auto-synced with upstream. Every update requires a new PR and a fresh security review.
