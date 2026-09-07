# Standing Engineering Authority Policy

Status: group-wide default for active enxpower repositories.

## Purpose

The Owner keeps ownership, control, business judgment, and the emergency stop. Routine technical correctness is decided through evidence, checks, and accountable engineering execution rather than ceremonial Owner approval.

## Standing authorization

Within an already approved product objective, budget, environment, and system boundary, an authorized engineering agent or maintainer may complete the full routine lifecycle without asking the Owner at each step:

`Issue/task → branch → implementation → tests → PR → review → merge → existing-environment deployment → live verification → rollback when needed → VWS update`.

This standing authorization covers:

- focused bug fixes, maintenance, documentation, tests, CI repair, and governance alignment;
- review resolution and squash merge after required checks pass;
- reversible deployment to an existing environment when the target, rollback path, and success signals are known;
- scheduled automation already approved by policy;
- fail-closed recovery and rollback inside an existing runbook.

A PR is still required when repository-local rules require one. Required CI, security checks, separation of duties where configured, and production verification remain mandatory. The change is that routine technical execution no longer waits for an Owner signature.

## Owner decision exceptions

Stop and escalate only when the decision is genuinely an Owner/business decision or authority must expand:

1. product identity, business scope, binding commercial terms, or material acceptance criteria change;
2. new or materially increased spend, contract, payment, refund, trade, advertising budget, banking, tax, or legal commitment;
3. destructive or materially irreversible data action, unrecoverable migration, service retirement, repository deletion, or domain transfer;
4. new credential model, material permission expansion, ownership transfer, secret exposure response, or loss of the recovery path;
5. new external customer, supplier, employee, investor, public, or regulatory communication not already covered by an approved policy/template;
6. live transaction or physical-safety action outside an existing bounded policy envelope;
7. production change with no verified rollback or with uncertain blast radius beyond the repository's accepted risk envelope;
8. conflict between governing authorities that cannot be resolved from current evidence.

Do not escalate a question merely because it is technical, difficult, or unfamiliar to the Owner. Obtain competent technical review or fail closed.

## Risk tiers

- **R0 — Read/document:** inspect, document, triage, plan, and update non-executable governance. Execute autonomously.
- **R1 — Routine reversible engineering:** code/CI/PR/merge and reversible existing-environment deployment with green gates. Execute autonomously and report evidence.
- **R2 — Elevated but bounded:** security-sensitive or operational change inside an existing approved envelope. Require stronger technical review, canary/backup/rollback, and evidence; Owner approval is not required unless an exception above applies.
- **R3 — Owner decision:** an exception above. Present the business choice, exposure, alternatives, and recommendation; wait for the Owner.

## Evidence gates

Before merge or deployment, as applicable:

- exact target and scope are resolved;
- diff is reviewed and unrelated changes are excluded;
- required CI/tests/guards pass;
- secrets and sensitive-data exposure checks pass;
- rollback/recovery is defined and usable;
- deployment uses the reviewed revision;
- live behavior and critical routes are verified;
- failures trigger rollback or a fail-closed stop;
- VWS records only externally verified current state.

`merged != deployed != verified`.

## Precedence and compatibility

This policy supersedes older repository wording that requires separate Owner approval for routine PR creation, merge, deployment, publication, or scheduled execution.

It does not waive repository-specific business, finance, transaction, safety, privacy, legal, credential, destructive-action, public-communication, or product-constitution controls. Those controls remain effective and are interpreted through the exception list above.

The Owner may pause, narrow, or revoke standing authorization at any time. Account ownership, billing ownership, recovery credentials, and kill switches remain Owner-controlled.
