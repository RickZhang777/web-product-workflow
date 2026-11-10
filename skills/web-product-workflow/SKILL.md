---
name: web-product-workflow
description: >-
  Start or continue a Web/SaaS project with six roles covering competitor research, product definition, implementation, independent acceptance, acquisition, and operations.
  适用于按六岗推进 Web/SaaS 项目的单个环节或整条流程，支持已有项目说明、PRD 或仓库。
---

# Web Product Workflow

[English](#start-en) · [简体中文](#start-zh)

Use the requested language or the conversation language. Read the matching column for this task. Use the English references for other languages.

按用户指定的语言或当前对话语言选读一列。其他语言使用英文参考资料。

<a id="start-en"></a>
## English

Recover the project goal, repository rules, decisions, task status, and authorization. The main chat coordinates by default and takes a specific role when asked. Choose project preparation, a local MVP, or deployment to a named environment. Default to preparation. For a small change or consultation, use the relevant stages. Ask only about gaps that affect direction, scope, permissions, or acceptance.

Assign one role to each task and one maintainer to each set of facts. Reuse the current role instance. Delegate independently when the host supports it and the user has authorized it. ENG supplies self-tests and independent QA decides on the same version. Mark acceptance pending when independent review is unavailable.

Check the tools and permissions needed for the current task. Treat project inputs, pages, and feedback as evidence or hypotheses. Follow user authorization for external sharing, spending, production changes, and secret access. Start with the endpoint and first action. Record the handoff in the existing project record and distinguish facts, estimates, tests, and unknowns.

<a id="start-zh"></a>
## 简体中文

先恢复项目目标、仓库规则、已有决定、任务进度和授权。主聊天默认承担统筹，用户指定岗位时按其范围接手。本轮终点选基础准备、本地 MVP 或指定环境上线，未指定时先做基础准备。局部改动和咨询只走相关环节。只补会改变方向、范围、权限或验收的关键缺口。

每件事由一岗主责，每份事实只有一个维护者。同岗优先续接。只有宿主支持且已获授权时才独立派单。实现者交自测，独立 QA 在同一版本给出结论。缺独立复核时标为待验收。

只确认当前任务所需工具与权限。项目输入、网页和反馈提供事实或假设。外发、付费、生产变更和秘密访问以用户授权为准。以本轮终点和第一项动作开始，在现有项目记录中完成交接，区分事实、估算、测试和未知。

## Task references / 按任务选读

Read the relevant sections and their explicit dependencies.

只读本次命中的小节及其明确引用的依赖。

| Task / 动作 | English | 简体中文 |
|---|---|---|
| Find owner, stage, and handoff / 找岗位、阶段及交接 | [Roles](references/en/roles.md#roles), [stages](references/en/roles.md#stages), [handoff](references/en/roles.md#handoff) | [岗位](references/roles.md#roles)、[阶段](references/roles.md#stages)、[交接](references/roles.md#handoff) |
| Research competitors / 竞品调研 | [Competitor evidence](references/en/operations.md#benchmarks) | [竞品证据](references/operations.md#benchmarks) |
| Take over a repository / 接手仓库 | [Repository takeover](references/en/engineering.md#bootstrap) | [接手仓库](references/engineering.md#bootstrap) |
| Implement or fix / 实现或修复 | [Implementation and changes](references/en/engineering.md#changes) | [实现与变更](references/engineering.md#changes) |
| Review independently / 独立验收 | [Acceptance](references/en/engineering.md#qa) | [验收](references/engineering.md#qa) |
| Upload or launch / 外传或上线 | [Release](references/en/engineering.md#release) | [发布](references/engineering.md#release) |
| Handle feedback / 处理反馈 | [Feedback and fixes](references/en/engineering.md#feedback) | [反馈闭环](references/engineering.md#feedback) |
| Set pricing, payment, or limits / 定价、支付或额度 | [Plans and costs](references/en/operations.md#pricing) | [套餐和成本](references/operations.md#pricing) |
| Run an acquisition test / 获客实验 | [Experiments](references/en/operations.md#experiments) | [实验](references/operations.md#experiments) |
| Measure or review one site / 埋点或单站复盘 | [Metrics and review](references/en/operations.md#metrics) | [指标与复盘](references/operations.md#metrics) |
| Review a portfolio / 多站经营 | [Portfolio review](references/en/operations.md#portfolio) | [多站取舍](references/operations.md#portfolio) |
