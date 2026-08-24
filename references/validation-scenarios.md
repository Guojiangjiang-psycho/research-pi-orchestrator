# Validation Scenarios

Read this reference only when creating, revising, or auditing the skill. Test observable behavior, not exact wording.

## A. New project initialization

Prompt: “我要做一个关于 X 的研究。”

Pass if the Orchestrator:

- identifies itself;
- clarifies intended output and stage from available context;
- creates or proposes the minimum project memory;
- recommends only currently useful Works;
- defines Memory Contracts before specialist work begins;
- returns a Dashboard and next actions.

Fail if it launches all role templates, starts doing deep research itself, or creates a large empty file bureaucracy.

## B. Specialist completion

Situation: Literature Work finishes a literature map.

Pass if the flow includes file update, report, Orchestrator review, integration, and status update. Fail if the Work only writes a file or the Orchestrator accepts conclusions without review.

## C. Specialist request sent to Orchestrator

Prompt: “系统比较这三种测量方案。”

Pass if the Orchestrator routes substantive comparison to the appropriate Work with a contract-aware assignment. A tiny temporary clarification may be answered directly. Fail if capability alone causes the Orchestrator to absorb the full specialist task.

## D. PI-direct specialist task

Situation: The PI asks Analysis Work for an extra analysis.

Pass if the Work completes and reports, the Orchestrator reviews and integrates it, and a changed conclusion becomes a PI decision point. Fail if direct access bypasses shared memory.

## E. Work-to-Work collaboration

Situation: Theory Work needs evidence already held by Literature Work.

Pass if they share declared files or collaborate directly without asking the PI to copy context, then synchronize important conclusions. Fail if the Orchestrator becomes a message relay or shared files are edited without ownership rules.

## F. PI returns after absence

Prompt: “现在做到哪里了？”

Pass if the Orchestrator gives a short Dashboard with current stage, work, risks, decisions, milestone, and next actions. Fail if it dumps full logs or cannot distinguish integrated from pending work.

## G. Historical Deep Dive

Prompt: “为什么当时放弃方案 B？”

Pass if the Orchestrator first answers concisely, then can unfold the decision, alternatives, evidence, related Work, files, and original traces. Fail if the rationale was not retained or the response begins with raw history instead of synthesis.

## H. Writing transition

Situation: Writing Chat receives `writing_handoff.md`.

Pass if it can recover why the study exists, how the question and design formed, key evidence and rejected paths, result boundaries, PI judgments, and unresolved issues. Fail if it must invent the research story at writing time or treats the handoff as a draft.

## Cross-scenario acceptance criteria

The skill passes only if all are true:

1. The PI remains the final research decision-maker.
2. Substantive knowledge creation is delegated by default.
3. Every active Work has Read / Write / Report / Escalation rules.
4. Specialist tasks cannot close before report, review, and integration.
5. Direct access and flat collaboration do not fracture project memory.
6. Dashboard and Deep Dive provide two distinct information densities.
7. Durable state lives in files and can be reconstructed after time away.
8. Trigger wording does not attract standalone literature, analysis, drafting, or method questions.
