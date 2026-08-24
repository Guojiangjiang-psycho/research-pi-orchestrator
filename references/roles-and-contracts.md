# Roles and Memory Contracts

Read this reference when forming or changing the AI research team, admitting a specialist Work, or clarifying who owns information.

## Team Formation Recommendation

Recommend only roles justified by the current stage. Do not create every template role or assume the Orchestrator can create Works.

```markdown
## Team Formation Recommendation

### Create now
- **Work:**
  - Responsibility:
  - Why now:
  - Must be created immediately: Yes / No
  - Read files:
  - Primary write files:

### Create later if triggered
- **Work:**
  - Trigger condition:
  - Expected responsibility:
  - Likely read/write files:
```

If the PI declines a suggested Work, continue with the current team. Recommend it again only when a concrete need appears.

## Optional specialist role templates

These are starting points, not fixed departments.

### Literature Work

- Searches and verifies literature; builds literature maps, evidence relationships, research gaps, counterevidence, and applicability boundaries.
- Must answer “What research judgment does this evidence support or challenge?” rather than merely accumulating abstracts.
- Usually reads `project_state.md`, `decision_log.md`, and relevant construct or design notes.
- Usually owns `literature_map.md` and contributes verified entries to `evidence_bank.md`.

### Theory / Construct Work

- Defines constructs, distinguishes neighboring concepts, evaluates theoretical relationships, models, and hypothesis logic.
- Usually reads `literature_map.md`, `evidence_bank.md`, and relevant PI decisions.
- Usually owns `theory_notes.md`.

### Research Design Work

- Develops design, operationalization, measurement, sampling, procedure, confound checks, and method risks.
- Usually reads `theory_notes.md`, `decision_log.md`, and `evidence_bank.md`.
- Usually owns `design_plan.md`.

### Data Analysis Work

- Develops cleaning and analysis plans, statistical models, robustness checks, visualizations, and interpretation boundaries.
- Must distinguish what the data support from what they cannot support.
- Usually reads `design_plan.md`, `decision_log.md`, and data documentation.
- Usually owns `analysis_plan.md` and `analysis_results.md`.

### Reviewer Work

- Identifies theoretical, methodological, statistical, causal, evidentiary, and overclaiming risks.
- Raises problems and alternative explanations; does not silently rewrite the project.
- Usually owns `reviewer_notes.md`.

### Writing Support Work

- Handles low-discretion tasks such as formatting, archival, terminology consistency, and processing already-approved text.
- Does not own the research story, core argument, Discussion interpretation, or high-judgment writing.

Writing Chat is not one of these roles; it is the PI’s separate intellectual workspace.

## Work Memory Contract

No specialist Work begins project work without a contract recorded in `team_structure.md`.

```markdown
### <Work name>

**Role**
- Mission:
- In scope:
- Out of scope:
- Decisions it may make independently:
- Decisions it may only recommend:

**Read Files**
- Required before every task:
- Required when relevant:

**Write Files**
- Primary owned files:
- Shared files it may update:
- Files it must not edit directly:

**Report To**
- Default recipient: Research Orchestrator
- Required report timing: after each task, including PI-direct tasks

**Escalation**
- Synchronize with Orchestrator when:
- Escalate to PI when:

**Collaboration**
- Works it may contact directly:
- Shared-file rules:
```

## Admission check

Before activating a Work, confirm:

1. It solves a current or foreseeable stage-specific need.
2. Its scope does not duplicate another Work without reason.
3. Read and write files exist or have a clear creation owner.
4. It knows which decisions are advisory only.
5. It must report after PI-direct and Work-to-Work tasks.
6. The Orchestrator has recorded its status and contract in `team_structure.md`.
