# Curriculum

Use the modules as a progression, not as a rigid lecture sequence. Skip a module only when the user demonstrates its capability with evidence.

## 1. Throughput and bottlenecks

Diagnose the limiting step using the three-minute-egg analogy. Distinguish code generated from valuable, verified work delivered. Identify work in progress and the user's attention bottleneck.

**Completion evidence:** the user correctly diagnoses a bottleneck in a real workflow and proposes a measurable intervention.

## 2. Verification first

Distinguish review, tests and executed behavioral verification. Explain why a green build is necessary but insufficient and why verification becomes stale after the patch changes.

**Completion evidence:** a verification plan maps each acceptance criterion to an observable check.

## 3. Verification skills

Design a reusable project-specific verification skill. For a Spring service, consider startup commands, authentication, fixtures, tenant context, API calls, database effects, asynchronous waiting, cleanup and evidence capture.

**Completion evidence:** another agent can follow the skill without relying on undocumented human knowledge.

## 4. Work decomposition and parallelism

Split work by independent outcomes and write scopes. Define dependencies, artifacts, checkpoints and integration checks. Reject fake parallelism that merely creates a larger review queue.

**Completion evidence:** a real change is divided into safe work units with explicit contracts.

## 5. Agent roles and handoffs

Use roles such as planner, implementer, reviewer and verifier only when they improve separation of concerns. Define inputs, outputs, authority and stopping conditions for each role.

**Completion evidence:** each handoff is auditable and no agent silently expands scope.

## 6. Supervised autonomy

Increase autonomy gradually: supervised execution, reusable verification, bounded multi-agent work, then longer orchestration. Keep consequential gates such as merge or production changes under explicit user control unless separately authorized.

**Completion evidence:** the workflow states what agents may do alone and where a human gate remains.

## 7. Personal orchestration system

Apply the course to a shared Git repository, Spec Kit, reusable skills and a router capable of selecting project, agent and workflow. Optimize for reproducibility and evidence rather than maximum agent count.

**Completion evidence:** run one end-to-end change and retrospectively measure lead time, waiting time, rework and verification quality.
