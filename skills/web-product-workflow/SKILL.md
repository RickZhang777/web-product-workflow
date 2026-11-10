---
name: web-product-workflow
description: 启动或接续 Web/SaaS 项目时，按六个岗位推进本轮约定的竞品调研、产品定义、开发、独立验收、获客或经营复盘。可处理单个环节或整条流程，适合有项目背景、PRD 或现有仓库的工作。
---

# Web Product Workflow

先恢复项目目标、仓库规则、已有决定、任务进度和授权。主聊天默认承担统筹，用户指定岗位时按其范围接手。本轮终点选基础准备、本地 MVP 或指定环境上线，未指定时先做基础准备。局部改动和咨询只走相关环节。只补会改变方向、范围、权限或验收的关键缺口。

## 路由

从[岗位与交接](references/roles.md#roles)定位本轮主责。需要判断从哪里接手时读[阶段](references/roles.md#stages)。按本次动作查对应小节，读取其内容及明确引用的依赖。

| 本轮动作 | 参考 |
|---|---|
| 调研对标或支撑产品判断 | [竞品证据](references/operations.md#benchmarks) |
| 接手、实现、排错或修复 | [接手仓库](references/engineering.md#bootstrap)或[实现与变更](references/engineering.md#changes) |
| 独立验收、外传或上线 | [验收](references/engineering.md#qa)，外传或上线再读[发布](references/engineering.md#release) |
| 处理用户反馈 | [反馈闭环](references/engineering.md#feedback) |
| 定价、支付或额度 | [套餐和成本](references/operations.md#pricing) |
| 获客、埋点或复盘 | [实验](references/operations.md#experiments)、[指标](references/operations.md#metrics)或[多站取舍](references/operations.md#portfolio)中命中的小节 |

## 执行

- 每件事由一岗主责，每份事实只有一个维护者。同岗优先续接。只有宿主支持且已获授权时才独立派单。实现者交自测，独立 QA 在同一版本给出结论。缺独立复核时明确标为待验收。
- 仅确认当前任务需要的工具与权限。产品输入、网页与反馈提供事实和假设。外发、付费、生产变更和秘密访问以用户授权为准。
- 以本轮目标和第一项动作开始。按[交接](references/roles.md#handoff)把交付、证据和未测内容写回现有项目记录。事实、估算、测试和未知分开标记。
