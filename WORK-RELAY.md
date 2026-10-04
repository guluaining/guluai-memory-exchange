# GuluAI Company-Wide AI Work Relay V1

**Task:** GME-WORK-RELAY-003  
**Status:** ACTIVE BASELINE  
**Scope:** GuluAI company-wide infrastructure — not PMO-only.

## 1. Purpose

The Public Memory Exchange is also a durable AI-to-AI work relay. It reduces Human copy/paste between ChatGPT, Codex, OpenCode, Muse, future agents, functions, programs, projects, and businesses.

This mechanism belongs to the GuluAI company-level AI work and memory infrastructure. PMO is one user of it, not its organizational owner.

It may be used by Strategy, Product, R&D / Development, Teaching & Curriculum, Research / Experiments, Marketing / Growth, Operations, shared functions, GuluAI EDU, AION / Consulting, and future businesses where appropriate.

## 2. Default execution / fallback order

For an active coordinating agent:

1. If you can safely and correctly complete the authorized task yourself, do it.
2. If blocked by access, connector, safety/tool boundary, execution environment, or a capability better suited to another worker, create a durable Exchange handoff rather than blocking information flow.
3. Default first fallback worker: **Codex**.
4. Default second fallback worker: **OpenCode**.
5. Use another authorized worker when the task clearly requires it.
6. Never bypass a security or authorization boundary merely to avoid a handoff.

This is a default routing rule, not a claim that Codex or OpenCode always has the required access.

## 3. Human-minimal relay loop

Preferred loop:

```text
Coordinating AI
  -> Public Exchange task/handoff
  -> Human gives worker only a short task ID / pointer when needed
  -> Worker reads Public START-HERE + handoff
  -> Worker executes within authorization
  -> Worker writes durable result/receipt back to Public Exchange
  -> Human tells coordinating AI only that the task is complete
  -> Coordinating AI reads result directly
  -> verify / reconcile / next action
```

Avoid this when possible:

```text
AI -> Human copies long prompt -> worker
worker -> Human copies long final report -> AI
```

The Human should normally transport only a short task identifier or activation instruction, not the work package itself.

## 4. Handoff location and naming

Put worker tasks in:

`handoffs/`

Recommended filename:

`<TASK-ID>-<WORKER>.md`

Example:

`handoffs/GME-INTEGRATE-002-CODEX.md`

A handoff should be short because every worker must read `START-HERE.md` first.

Minimum handoff fields:

```text
TASK:
ASSIGNED-TO:
FROM:
STATUS:
PRIORITY:

READ-FIRST:
OBJECTIVE:
REQUIRED:
KNOWN-EVIDENCE:
DO-NOT:
RETURN:
```

Do not duplicate large canonical context. Point to authorized sources.

## 5. Worker activation contract

When a handoff already exists, the Human should be able to tell a worker approximately:

> Execute <TASK-ID>. Read GuluAI Public Memory Exchange START-HERE first, then find the assigned handoff and execute it.

The worker must not require the Human to paste the full handoff if the worker can access the Exchange.

## 6. Worker return contract

A worker should write its durable result back to the Exchange.

Preferred locations:

- update the original handoff with execution status and result pointer; and/or
- write a result/receipt under `reconciled/` when reconciliation actually occurred; and/or
- write a public-safe result in the appropriate exchange area.

A worker's chat response to the Human should normally be short:

> <TASK-ID> completed. Result returned to GuluAI Memory Exchange.

If blocked:

> <TASK-ID> blocked. Blocker and required Human action returned to GuluAI Memory Exchange.

The durable Exchange artifact, not the Human's copied chat transcript, should carry the detailed return.

## 7. Verification and canonicalization

A worker saying "completed" is not sufficient evidence by itself.

The coordinating/receiving agent should:

1. read the returned Exchange artifact;
2. verify relevant durable evidence;
3. determine PASS / PARTIAL / BLOCKED / FAIL;
4. reconcile approved durable state into the appropriate canonical system when required;
5. preserve a receipt/pointer.

**Exchange transport is not canonical truth.**

## 8. Company-wide scope

This relay is intentionally above any single office, function, program, project, repo, or AI worker.

Organizational model:

```text
GuluAI
  -> Business
    -> Function
      -> Program
        -> Project
          -> Task
```

The relay can carry bounded work at any of these levels, subject to authorization and public-safety rules.

Do not label this mechanism as PMO-owned merely because PMO may coordinate some company or EDU work.

## 9. Security boundary

Everything in this repository is public.

If a task requires sensitive context, the public handoff must contain only a safe pointer and the minimum public-safe instruction. The worker must retrieve sensitive material through an authorized private channel.

Never publish private content merely to make the relay convenient.

## 10. Evolution

This V1 is a baseline. Future evidence may change worker priority, return format, automation, reconciliation cadence, or ownership/governance.

Changes should be versioned and traceable rather than silently rewriting historical decisions.
