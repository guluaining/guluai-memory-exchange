# GuluAI Mobile-First AI Work Operating Model V0.1

**Task:** GME-MOBILE-FIRST-004  
**Status:** HUMAN-APPROVED EXPERIMENTAL BASELINE / IN VALIDATION  
**Scope:** GuluAI company-wide work operating model candidate  
**Date:** 2026-10-04

## 1. Hypothesis

GuluAI is testing a company-wide **Mobile-First / Chat-First AI Work** model.

The Human should be able to initiate, direct, review, approve, and continue a large portion of company work from a mobile phone, primarily through ChatGPT Chat, without needing to sit at a development workstation for routine coordination.

This is an operating-model experiment, not a permanent constitutional rule. Evidence should determine whether it is expanded, modified, or rolled back.

## 2. Default work ladder

Preferred escalation path:

```text
Human
  -> Mobile phone
  -> ChatGPT Chat
       -> execute directly when capable and authorized
       -> otherwise delegate / escalate
          -> ChatGPT Work OR Codex
          -> OpenCode / local engineering environment
          -> other specialized worker/tool when required
  -> durable result / evidence
  -> Human review / decision where required
  -> canonical reconciliation
```

Interpretation:

### Level 1 — Mobile + ChatGPT Chat

Default Human control surface.

Use for:
- discussion and decisions;
- planning and coordination;
- reading/review;
- lightweight connected-app actions;
- repository/document actions Chat can safely perform;
- delegation;
- verification;
- Human Gates;
- work-memory recovery.

Chat should execute directly when it has the capability, authorization, and evidence needed.

### Level 2 — ChatGPT Work / Codex

Preferred escalation when Chat cannot or should not complete the work directly.

Use Work for substantial multi-step work, browser/computer workflows, research, file/app workflows, or tasks benefiting from a longer autonomous execution environment.

Use Codex especially for bounded engineering/repository/code execution and durable task completion.

The exact choice is task-dependent; neither tool is universally superior.

### Level 3 — OpenCode / Local Engineering Environment

Use when work requires the local machine, persistent terminal/session context, local models/hardware, long-lived engineering environment, device/LAN access, or capabilities not available through Chat/Work/Codex.

OpenCode remains important, but routine company coordination should not require the Human to begin at a workstation if a higher-level mobile path can safely accomplish the task.

## 3. Mobile-First does NOT mean mobile-only

The principle is:

> Start at the highest-level, lowest-friction Human control surface that can safely complete or delegate the work.

It does not mean:
- all work must happen on a phone;
- engineering terminals are obsolete;
- Chat should pretend to have capabilities it lacks;
- security/authorization boundaries may be bypassed;
- Human review disappears.

## 4. Relation to Public Memory Exchange

The Public Memory Exchange makes Mobile-First practical.

When Chat delegates:

```text
Mobile Human
 -> ChatGPT Chat
 -> Exchange handoff
 -> Work / Codex / OpenCode
 -> Exchange result
 -> ChatGPT Chat reads and verifies
 -> Human sees decision-ready summary
```

The Human should normally move only a short task ID or activation instruction between environments.

Long prompts, context packages, and final reports should live in durable shared artifacts whenever practical.

## 5. Current default escalation preference

Current experimental preference:

1. ChatGPT Chat executes directly when possible.
2. If not, use ChatGPT Work or Codex according to task type.
3. If still unsuitable, use OpenCode / local engineering environment.
4. Use specialized agents/tools where they are the better fit.

This supersedes any overly simple interpretation that every Chat blocker must go directly to Codex. Codex remains the default engineering/repository fallback; Work may be the better Level-2 executor for non-code multi-step work.

## 6. Company-wide scope

This is not a PMO-only workflow.

It may apply across:
- executive/leadership work;
- strategy;
- product;
- PMO / architecture and planning;
- R&D / development;
- teaching and curriculum;
- research / experiments;
- marketing / growth;
- operations;
- shared services;
- GuluAI EDU;
- AION / Consulting;
- future businesses.

Different functions may use different execution depths while sharing the same Human-facing control model.

## 7. Evidence to collect

During validation, observe:
- how much useful work can start and finish from mobile;
- how often Chat must escalate;
- Work vs Codex suitability by task type;
- how often OpenCode/local access is genuinely required;
- Human copy/paste burden;
- recovery quality across agents;
- latency and cost;
- error/rework rate;
- security and permission failures;
- quality of durable evidence and canonical reconciliation;
- Human cognitive load and convenience.

## 8. Success direction

The experiment is promising if the Human can increasingly operate as:

```text
Intent / Voice / Decision / Approval
             |
          Mobile
             |
       ChatGPT Chat
             |
     AI execution fabric
             |
   durable organizational system
```

while preserving evidence, security, accountability, recoverability, and Human authority.

## 9. Evolution rule

Do not silently turn this experiment into permanent policy.

Future evidence may:
- promote it to a company operating standard;
- change the escalation order;
- specialize the ladder by function;
- add/remove execution agents;
- automate more handoffs;
- roll back parts that do not work.

Record meaningful changes with date, rationale, evidence, and Human decision.
