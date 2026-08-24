# Project Memory

Read this reference when initializing or recovering a project, creating files, assigning file ownership, resolving conflicting state, or preparing Writing Chat memory.

## Memory principles

- Chat is where work happens; files hold durable, reconstructable project memory.
- Chat carries deltas: assignments, new findings, questions, decisions, and next steps.
- Do not create files merely to mirror organizational roles. Create a specialist file when it will hold durable work with a clear owner.
- Keep project-level files concise enough to recover state quickly; keep detailed specialist work in owned specialist files.
- Never silently overwrite a frozen decision or resolve a file conflict by choosing the newest text without reviewing meaning.

## `project_state.md`

Owner: Research Orchestrator. This is a dashboard, not a knowledge repository.

```markdown
# Project State

## Research Goal and Intended Output

## Current Stage

## Completed

## In Progress

## Current Team

## Risks and Blockers

## PI Decisions Needed

## Next 1–3 Actions

## Next Milestone
```

Update after integration, a material status change, a stage transition, or a PI decision. Do not copy detailed evidence or analysis into it.

## `team_structure.md`

Owner: Research Orchestrator. This is both the team map and the information-flow map.

```markdown
# Team Structure

| Work | Status | Current Task | Primary Read Files | Primary Write Files | Report To |
|---|---|---|---|---|---|

## Memory Contracts

<!-- One contract per active Work; use roles-and-contracts.md -->
```

Use statuses such as Proposed, Active, Waiting, Blocked, or Inactive. Update when a Work joins, leaves, changes scope, accepts a task, or becomes blocked.

## `decision_log.md`

Owner: Research Orchestrator. Record decisions that shape the research route, interpretation, or writing.

```markdown
## <Date> — <Decision>

**Status:** Proposed / PI Confirmed / Frozen / Reopened / Superseded

**Problem**

**Options Considered**

**PI Decision**

**Reasoning and Evidence**

**Rejected Options and Why**

**Downstream Impact**

**Reopen Conditions**

**Related Files / Tasks**
```

A specialist recommendation is not a project decision until the PI or authorized project process confirms it. To reopen a frozen decision, record why the prior assumptions no longer hold; preserve the original entry.

## `evidence_bank.md`

Store evidence that actually informs a research judgment, not every paper encountered.

```markdown
## <Claim or decision supported>

**Source**

**Relevant finding**

**Evidence strength:** Strong / Moderate / Weak / Unverified

**Applicability boundary**

**Counterevidence or uncertainty**

**Potential use:** Theory / Design / Methods / Discussion / Limitations / Reviewer response

**Verification status and owner**
```

## Specialist files

Create only when active work needs them. Typical examples:

- `literature_map.md` — Literature Work;
- `theory_notes.md` — Theory / Construct Work;
- `design_plan.md` — Research Design Work;
- `analysis_plan.md` and `analysis_results.md` — Data Analysis Work;
- `reviewer_notes.md` — Reviewer Work.

Give each file one primary owner. Cross-Work updates require an explicit agreement in the relevant Memory Contracts. When ownership is unclear, write a report to the Orchestrator instead of editing opportunistically.

## `writing_handoff.md`

Owner: Research Orchestrator. Maintain from early project stages. It is the interface to Writing Chat, not a paper draft.

```markdown
# Writing Handoff

## The Question the Research Actually Seeks to Answer

## Current Research Story

## Core Argument Chain

## Key Evidence and Counterevidence

## Design and Why It Was Chosen

## Main Results and Interpretation Boundaries

## PI Judgments, Language, Doubts, and Intuitions

## Important Rejected Paths or Interpretations

## Unresolved Questions

## Current Writing Chat Task

## Files Writing Chat Should Read
```

Preserve the PI’s uncertainty and distinctive judgments. Do not smooth unresolved controversy into artificial consensus or reconstruct a post hoc story at writing time.

## Recovery and conflict handling

When recovering a project:

1. Read `project_state.md`, `team_structure.md`, and the latest relevant decision entries.
2. Check active specialist files and recent reports for work not yet integrated.
3. Compare chat claims with file state; treat unintegrated chat conclusions as pending, not authoritative.
4. Surface contradictions as explicit reconciliation items.
5. Restore a Dashboard and identify the next integration or PI decision needed.

When two files conflict, preserve both claims, identify their owners and dates, determine whether one is a proposal or confirmed decision, and escalate research-level ambiguity to the PI.
