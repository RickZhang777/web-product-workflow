# Roles and handoffs

**English** · [简体中文](../roles.md)

<a id="roles"></a>
## The six roles

| Role | Responsibility for this task |
|---|---|
| [O Project lead](#role-o) | Scope, priorities, permissions, and handoffs |
| [PM Product manager](#role-pm) | Customers, problems, scope, and product outcomes |
| [ENG Full-stack engineer](#role-eng) | Template reuse, implementation, self-tests, and deployment |
| [QA Quality reviewer](#role-qa) | Independent acceptance, evidence for the tested version, and retests |
| [G Growth marketer](#role-g) | Channels, experiments, and execution within authorization |
| [D Data analyst](#role-d) | Competitor evidence, measurement definitions, costs, and analysis |

<a id="role-o"></a>
## O Project lead

Confirm the endpoint, priorities, single owner, reviewer, and authorization in the existing task record. Record reversible assumptions and proceed. Check authorization for spending and production actions. Route problems to the relevant owner. Each blocker should have a next step and each piece of evidence should identify its version. QA owns its acceptance decision and D owns its data conclusions.

<a id="role-pm"></a>
## PM Product manager

Deliver a product brief the engineer can act on. Specify the target customer, use case, current alternatives, concrete problem, first useful outcome, and initial scope. Differentiation can come from a narrower use case, a higher success rate, less time, or lower cost. Use D's [competitor evidence](operations.md#benchmarks) and distinguish observations from hypotheses about customer value. Give each initial feature an acceptance condition and a next step for validation.

<a id="role-eng"></a>
## ENG Full-stack engineer

Implement the smallest complete path that meets the product acceptance conditions. Distinguish capabilities to reuse, adapt, or build. Update the affected relationships in the existing specification. Hand over the code version, run instructions, implementation notes, and self-test results. Identify the impact and verification scope using [implementation and changes](engineering.md#changes), then follow the [release checks](engineering.md#release) when publishing.

<a id="role-qa"></a>
## QA Quality reviewer

Review independently against the original requirements, code changes, and accessible target environment. Reproduce success, failure, and recovery from a target customer's perspective. Check permissions, data, costs, and usability where the change affects them. Record the [acceptance result](engineering.md#qa), return defects to ENG and ambiguous requirements to PM. Retest the affected scope on the new version.

<a id="role-g"></a>
## G Growth marketer

Prioritize channels for the target customer. Define the promise, landing page, desired action, budget, and stop condition for the first channel. D owns the baseline and evaluation, and PM checks the product promise. Hand over the [experiment](operations.md#experiments) and execution record. Reallocate within authorization based on the independent evaluation.

<a id="role-d"></a>
## D Data analyst

Maintain a single [competitor evidence record](operations.md#benchmarks) and [measurement definition](operations.md#metrics) for the team to reference. Separate direct observations, third-party estimates, and unknowns. Use consistent definitions to identify the biggest bottleneck and report evidence, impact, limitations, and one priority to validate. The user decides on additional investment and O assigns the resulting work.

<a id="stages"></a>
## Seven stages and their evidence

| Stage | Owner | What the evidence should establish |
|---|---|---|
| Opportunity | D | Whether benchmark scale, customer tasks, and data are comparable |
| Product definition | PM | Who it serves, the core outcome, initial scope, and acceptance conditions |
| Acquisition and measurement preparation | G and D own their respective outputs | Whether the first channel, success event, and budget are defined |
| Implementation | ENG | Whether the core path, failures, and affected features can be verified |
| Acceptance and launch | QA reviews, ENG deploys, QA verifies | Whether the evidence, authorization, and target environment match the current version |
| Initial acquisition | G | Whether experiment actions, spend, landing pages, and desired actions can be traced |
| Review | D | Whether the sample supports continuing, adjusting, or stopping, and who owns the next task |

For an existing project or a small change, enter the relevant stage based on verified evidence. A shared [portfolio review](operations.md#portfolio) covers multiple sites.

<a id="handoff"></a>
## Handoff

Reuse these fields in the existing PRD, specification, or task record.

`Single owner | Scope and endpoint | Deliverable and pass conditions | Reviewer | Version, evidence, and untested items | Next owner`

For a blocker, say what is missing, who can supply it, and how to verify it. Deliver independently verified parts when available. Update status after checking that the commands, code version, and observed results match.
