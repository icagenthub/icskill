[English](./README.md)

# ICSkill

面向 IC 设计领域的 AI Agent Skills 集合。

## 这是什么

ICSkill 收录经过筛选和验证的 AI Agent 技能包（Skills），供芯片设计团队在 Claude Code、Codex、OpenClaw 等 Agent 平台中使用。

每个 Skill 是一个独立的任务 SOP 包，包含执行步骤、约束条件、参考资料和验证方法，让 Agent 能够可靠地完成特定研发任务。

## 定位

- **安全可控**：每个 Skill 明确声明数据边界和权限要求
- **严格筛选**：收录标准优先考虑可验证性和可审计性
- **面向生产**：不是 demo 或概念验证，是能进入研发流程的工具

## 适用场景

芯片设计研发中的常见任务，例如：
- Regression triage
- Spec 转 testplan
- CDC/RDC 报告处理
- ECO 影响分析
- IP onboarding
- Release note 生成

## Skill 目录结构

```
skills/
  <skill-name>/
    SKILL.md          # 场景、步骤、边界、输出要求
    references/       # 规范、模板、历史案例
    scripts/          # 可执行逻辑
    assets/           # 样例、配置、素材
```

## 许可证

MIT
