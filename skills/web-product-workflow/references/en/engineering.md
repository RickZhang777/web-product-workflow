# Engineering and acceptance

**English** · [简体中文](../engineering.md)

<a id="bootstrap"></a>
## Take over a repository

ENG reads the project rules, relevant code, dependency manifest, lockfile, and environment variable examples, then records a runnable baseline. Identify what can be reused, adapted, or added for authentication, database, billing, and storage. Follow the repository's package manager, module format, and deployment target. Record the purpose, variable names, and environments for dependency or configuration changes. The user supplies credentials through environment configuration or a secret manager.

<a id="changes"></a>
## Implementation and changes

Use the simplest implementation for the known requirements. Give each function one clear responsibility and let a coordinating function call the steps of a larger operation. Preserve transaction, idempotency, and retry boundaries when splitting code. Reuse existing modules and tools. Evaluate an abstraction once concrete use cases repeat.

For changes to a shared flow, record the affected feature IDs, entry points, interfaces or data, business constraints, code locations, and verification steps in the existing specification. Before implementing, state what changes, what it affects, what must still hold, and how to test it. Update only the affected scope for a small change.

Cover failure cases for payments, permissions, quotas, and critical writes. Report model, network, and data errors according to the business rules, and guard against incorrect billing and sample output counted as success. If the feature promises streaming, verify that results appear incrementally before the request completes. Before destructive data operations, verify the target, authorization, and expected impact.

<a id="qa"></a>
## Independent acceptance

ENG hands over the change scope, code and configuration versions, self-tests, and untested items. QA checks that a user can find the entry point, complete the core task, understand wait and error states, and recover. Cover affected failure cases, data ownership, repeated requests, related features, and costs. Exercise the flow with a browser or an equivalent tool and supplement it with static evidence.

Record the version, environment, steps or commands, observed results, and decision. Report passed, failed, and untested items separately. Return blocking defects to ENG and retest the affected scope on the new version. Keep acceptance pending when an independent reviewer is unavailable.

<a id="release"></a>
## External uploads and launch

Before uploading, confirm the destination, authorization, and exact contents. Use existing checks to scan files and commits for credentials, personal information, and internal material. Before deployment, inspect the matching build and API responses for leaks through client bundles, serialization, logs, or errors. Use fictional examples or material approved for public use.

Base the release decision on the actual scan scope, target version, and results. Pause the relevant action if a sensitive finding remains, a required check fails, or the evidence refers to a different version. Automate deterministic checks through existing CI or hooks and have QA verify where they apply. Once release is authorized, ENG retains a rollback option and QA verifies the core flow in the target environment.

<a id="feedback"></a>
## Feedback and fixes

Group and deduplicate feedback by symptom and feature. Retain the minimum evidence needed to reproduce it. Send product questions to PM, defects to ENG, and analysis to D. O assigns work and sets priorities. After [independent acceptance](#qa), update the issue and communicate the outcome within authorization. For automated fixes, define the allowed scope, retry limits, and spending limits, and verify actions in isolation.
