# AGENTS.md

These rules apply to the entire `enxpower/agim.ca` repository.

## Read first

1. `docs/STANDING_ENGINEERING_AUTHORITY.md`
2. `README.md`, when present
3. task-relevant local governance, architecture, operations, security, and VWS documents
4. the current Issue/PR and live repository/runtime evidence

Current external evidence outranks stale documentation and chat history.

## Authority and workflow

Within the approved product, budget, environment, and system boundaries, routine technical work is standing-authorized through:

`Issue/task → branch → implementation → tests → PR/review → merge → reversible existing-environment deployment → live verification → rollback when needed → VWS`.

Use required checks and repository-local review. Do not pause for a ceremonial Owner signature when gates pass. Escalate only an R3 Owner-decision exception in `docs/STANDING_ENGINEERING_AUTHORITY.md`.

## Non-negotiable protections

- Preserve repository-specific product, architecture, safety, privacy, finance, transaction, legal/tax, credential, permission, destructive-action, and public-communication controls.
- Never weaken tests or hide failures to obtain green status.
- Never expose secrets or sensitive data.
- Keep changes focused, auditable, and reversible.
- Verify actual live behavior; `merged != deployed != verified`.
- Only externally verified facts enter VWS Completed.

Older repository wording that requires separate Owner approval for routine PR creation, merge, deployment, publication, or already-approved scheduled execution is superseded by the standing policy. True R3 business/authority exceptions remain Owner decisions.
