# Task Routing and Lifecycle Protocols

Read this reference whenever classifying a PI request, assigning specialist work, receiving a completion report, reviewing results, or synchronizing direct PI–Work and Work-to-Work collaboration.

## Delegation threshold

Use this test:

1. Is the request primarily management or integration of existing project knowledge? The Orchestrator handles it.
2. Is it a small, temporary question that creates no durable research asset and cannot change a project judgment? The Orchestrator may answer directly.
3. Does it create substantive research knowledge, require specialist depth, form a durable asset, or plausibly change a research judgment? Route it to a specialist Work.
4. Does it require choosing or reopening a core research judgment? Prepare a PI decision packet.

Examples of direct orchestration: update project state, summarize Work status, prioritize tasks, integrate results, generate a Dashboard, maintain files, organize handoffs, or explain current state.

Examples of specialist work: systematic literature search, deep theoretical comparison, construct definition, design, measurement comparison, data analysis, robustness testing, or reviewer simulation.

Do not delegate tiny questions mechanically. Do not absorb substantial specialist work merely because the Orchestrator is capable of doing it.

## Lifecycle

Every specialist task follows:

`Assign → Execute → Update Files → Report → Review → Integrate`

The task closes only after integration or an explicit decision that no project-level integration is needed.

### Assign

```markdown
## Task Assignment

**Current Task**

**Why This Work Owns It**

**Necessary Context**

**Read Files**

**Write Files**

**Task Boundary / Out of Scope**

**Decision Authority**

**Expected Report**

**Escalation Triggers**

**Acceptance Criteria**
```

Pass only necessary context and file locations; do not paste the complete project history.

### Execute and update files

The Work performs the task within its contract and writes detailed, durable results to owned or explicitly shared files. It marks proposals as proposals and records evidence limits.

### Report

Silent completion is prohibited. The Work reports after every task, including tasks assigned directly by the PI or another Work.

```markdown
**Task Status:** Completed / Partial / Blocked

**Completed Work:**

**Updated Files:**

**Key Findings:**

**Risks / Open Questions:**

**Impact on Project:**

**PI Decision Needed:** None / <decision>

**Suggested Next Step:**
```

### Review

The Orchestrator checks:

1. Did the Work answer the assigned question and stay within scope?
2. Are evidence, methods, and uncertainty sufficient and traceable?
3. Did it introduce a logical jump, overclaim, or unexamined alternative?
4. Does it conflict with a frozen decision or another file?
5. Does another Work need to review or continue it?
6. Does it create a PI decision point?
7. Which shared memory files need integration?

If incomplete, request targeted revision and keep status Partial or Blocked. Do not integrate unreviewed claims as confirmed project state.

### Integrate

Update only the files affected:

- `project_state.md` for status, risks, priorities, and milestones;
- `team_structure.md` for Work status and current tasks;
- `decision_log.md` for proposed, confirmed, frozen, reopened, or superseded decisions;
- `evidence_bank.md` for decision-relevant evidence;
- `writing_handoff.md` for material that shapes future writing;
- relevant specialist files for detailed technical content.

Record the task as closed only after integration. Tell the PI when integration creates a new decision, risk, or milestone change.

## Direct PI access synchronization

The PI may talk directly to any Work. The Work need not report purely temporary exploration that changes nothing. It must report when the conversation creates or changes any of the following:

- a task or deliverable;
- evidence that affects a research judgment;
- research direction, theory, or construct;
- design, measurement, analysis, or interpretation;
- a prior decision;
- a durable file or result;
- a risk, blocker, or PI decision point.

The report follows the standard format and identifies that the task was PI-direct. The Orchestrator reviews and integrates it like any other task.

## Work-to-Work collaboration

Works may collaborate directly when this lowers coordination cost. Before collaborating, make explicit:

- which question is shared;
- which files each Work reads and may write;
- which Work owns the final report;
- which findings require PI escalation.

Important conclusions must return to the Orchestrator. Direct collaboration never grants authority to change a frozen PI-level decision.

## Exceptions

If the PI explicitly asks the Orchestrator to execute a normally specialist task, state the routing exception briefly, use the appropriate specialist file schema, preserve evidence and uncertainty, and integrate the result. Do not silently turn the exception into the default operating model.
