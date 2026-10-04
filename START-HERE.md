# GuluAI Memory Exchange — START HERE

You are entering the GuluAI AI-native working system.

This public repository is the **company-wide** universal entry, exchange, and work-relay layer for GuluAI humans, AI agents, and authorized external reviewers. It is not owned by or limited to PMO, R&D, EDU, or any single function, program, project, or AI worker. A zero-context agent should start here before assuming anything about GuluAI memory, access, or current project state.

This repository is public. Treat everything here as permanently visible to the world.

## 1. What This Repository Is

`guluai-memory-exchange` is a public access, routing, and exchange layer.

It exists so that ChatGPT, Codex, OpenCode, Muse, future AI agents, and reviewers can recover the GuluAI memory-access model without needing a long verbal explanation.

Use it to:

- discover the correct memory path for your access level;
- exchange public-safe work products;
- create handoffs when private canonical write access is unavailable;
- mark public-safe memory candidates for later reconciliation;
- preserve traceability between public exchange work and canonical memory;\n- relay bounded work between AI agents with minimal Human copy/paste. See [`WORK-RELAY.md`](WORK-RELAY.md).

## 2. What This Repository Is Not

This repository is not the canonical GuluAI organizational memory.

It is not a private knowledge base, project vault, student record system, contract archive, or place to mirror private repositories.

Do not treat public exchange status as canonical status.

## 3. Minimal GuluAI Context

GuluAI is an AI-native education organization led by Ning / Ma Ning / moluoxiong. GuluAI works on education products, curriculum, teaching operations, teacher development, student growth records, AI-assisted teaching workflows, and organizational memory systems.

Current organizational interpretation:

GuluAI -> Business -> Function -> Program -> Project -> Task

GuluAI EDU functions include Strategy, PMO / Architecture & Planning, Product, R&D / Development, Teaching & Curriculum, Research / Experiments, Marketing / Growth, and Operations.

## 4. Memory Planes

### Public Exchange

This repository.

Role: mailbox, bus, universal front door, public-safe exchange area.

Canonical: no.

### Private Canonical GitHub

Current canonical repository:

`guluaining/guluai-development`

Primary canonical entry:

`START-HERE.md`

Role: brain, final reconciled organizational memory.

Canonical: yes, when accessed through authorized private GitHub permissions.

The historical repository name `guluai-development` does not mean Development is the organizational parent. It currently serves as the private canonical organizational memory location.

### Google Drive Shared Memory

Role: shared Human + AI workspace, review plane, human-readable memory gateway, working evidence.

Existing gateway:

`GuluAI Shared Memory Gateway — START HERE V0.1`

URL:

https://docs.google.com/document/d/1PY4AjyRzlX7HuNia8f8ErkxxWvsnpjn7MLNh8K0TAYw/edit

GitHub canonical remains the final reconciled organizational authority.

### Agent-Local Memory

Examples: local `MEMORY.md`, local `START-HERE.md`, agent profile notes.

Role: address book and router only.

Agent-local memory should remain thin. It should point to shared or canonical memory rather than duplicate it.

### Chat

Role: temporary working memory.

A conversation is not canonical organizational memory.

## 5. Access Paths

### If You Have Private GitHub Access

Follow this route:

Public `START-HERE.md`
-> private `guluaining/guluai-development/START-HERE.md`
-> relevant canonical artifacts
-> Google Drive only where needed for shared work, review, or evidence
-> perform the task
-> reconcile important results into canonical memory

### If You Do Not Have Private GitHub Access

Follow this route:

Public `START-HERE.md`
-> Shared Drive Gateway or authorized Drive/files/packages
-> perform bounded work
-> mark canonical uncertainty
-> leave public-safe work in this exchange or authorized Drive
-> return the work for canonical reconciliation

Use this exact marker when a claim requires private canonical verification that you cannot perform:

`CANONICAL VERIFICATION PENDING`

## 6. Standard Rules

Do not guess private state.

Do not infer that public exchange status equals canonical status.

Do not copy private repository contents wholesale into this public repository.

Do not publish secrets, private student information, confidential business information, or unauthorized third-party material.

If you are uncertain whether something is safe to publish, do not publish it here. Use an authorized private channel or ask the Human.

The Human remains the final authority.

## 7. Where To Put Public-Safe Work

Use the smallest appropriate location:

- `inbox/` for unclassified incoming information and AI outputs.
- `handoffs/` for explicit AI-to-AI or Human-to-AI work handoffs.
- `research/` for public-safe research and candidate technology findings.
- `review-packs/` for public-safe review packages for independent agents or reviewers.
- `memory-pending/` for non-sensitive information believed to deserve durable memory but not yet reconciled into canonical memory.
- `reconciled/` for receipts or pointers showing an exchange item was reconciled.

Prefer pointers and receipts over duplicating canonical private content.

## 8. Exchange Item Header

Use this simple metadata header for exchange items:

```text
ID:
CREATED:
CREATED-BY:
WORK-TYPE:
TARGET:
SENSITIVITY:
STATUS:
CANONICAL-DESTINATION:
RELATED-SOURCES:
```

Sensitivity values:

- `PUBLIC`
- `PUBLIC-SAFE`
- `REVIEW-REQUIRED`

Anything actually sensitive must not be committed here.

Exchange status values:

- `NEW`
- `TRIAGED`
- `IN-REVIEW`
- `READY-FOR-RECONCILIATION`
- `RECONCILED`
- `DEFERRED`
- `REJECTED`

Remember: public exchange status does not equal canonical status.

## 8.1 Company-Wide AI Work Relay\n\nThis Exchange is also the default durable AI-to-AI work relay across GuluAI company levels. PMO is one user, not the owner.\n\nWhen a coordinating AI cannot complete an authorized task, the default fallback order is **Codex first, OpenCode second**, unless another worker is clearly more appropriate. Create a short durable handoff under `handoffs/`; the worker reads this START-HERE and the handoff, executes, and writes the detailed result back to the Exchange. The Human should normally carry only the task ID / activation instruction between agents.\n\nFull protocol: [`WORK-RELAY.md`](WORK-RELAY.md).\n\n## 9. Reconciliation Model

Agents without canonical write access must not be blocked.

They may:

- write public-safe information to this exchange;
- write authorized collaborative material to Drive;
- produce handoff packages;
- mark memory-pending items;
- state `CANONICAL VERIFICATION PENDING` when needed.

Later, an authorized agent or Human may reconcile the material into the canonical private repository.

Important decisions should be reconciled promptly. Routine exchange material may be reconciled periodically. No automated schedule is defined in this V1 repository.

## 10. Reconciliation Receipt

After an item is reconciled, preserve traceability. A receipt should ideally record:

```text
Exchange Item ID:
Original location:
Canonical destination:
Canonical commit / artifact:
Reconciled by:
Reconciled date:
Result:
Notes:
```

Do not delete history merely because reconciliation completed.

## 11. Front-Door Contract

Reusable instruction for future AI agents:

Read first:

https://github.com/guluaining/guluai-memory-exchange/blob/main/START-HERE.md

Recover the GuluAI working and memory-access context from that file.

Do not assume access to private resources.

Follow the access path available to you.

Do not guess private canonical state.
