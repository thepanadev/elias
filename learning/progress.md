# Learning progress

## Current position

- Module: 5 — Agent roles and handoffs
- Status: in progress
- Last session: 2026-09-11
- Completed modules: 4 of 7
- Overall progress: 57%

## Open exercise

Design planner, preparer, scenario workers and independent verifier roles with explicit inputs, outputs, authority, write scopes and stopping conditions.

## Evidence

- Module 1 completed with a real workflow diagnosis.
- The critical path begins before functional testing: JFrog artifact checks and conditional Jenkins rebuilds, Helm deployment (~45 minutes), base seed data (~1 hour), then scenario-specific manual data.
- The user distinguished fixed latency, variable rework and knowledge held by the human operator.
- Module 2 completed through a worked reference contract mapping artifact availability, deployment health, seed postconditions, scenario prerequisites and deployed-change identity to observable checks.
- Deployment identity is modeled as commit SHA → Jenkins build → artifact checksum → image digest → Helm release → running pod image ID. This is a target design to investigate, not a claim about the current company setup.
- Module 3 completed through a worked two-skill design: `prepare-environment` owns bounded mutations and checkpoints; `verify-environment-ready` remains observational and independently emits PASS, FAIL or BLOCKED with evidence.
- Module 4 completed through a worked decomposition of cancellation, stock reception and order-search scenarios into isolated tenants, order IDs, PU codes and read/write scopes while sharing the immutable base environment.

## Next action

Define auditable handoff contracts so that each agent receives only the context and authority needed for its role.
