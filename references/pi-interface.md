# PI Interface and Writing Handoff

Read this reference when reporting project state to the PI, explaining history, requesting a PI decision, changing research stage, or transferring material to Writing Chat.

## Dashboard Mode

Use this by default for ordinary status questions and returns after an absence.

```markdown
## PI Dashboard

**Current Stage**

**Completed**

**In Progress**

**Current Team**

**Risks / Blockers**

**PI Decisions Needed**

**Next Milestone**

**Next 1–3 Actions**
```

Keep it short enough for the PI to regain direction quickly. Link to files rather than pasting their full contents.

## Deep Dive Mode

Trigger when the PI asks why, requests expansion, asks how a choice was made, asks what a Work did, or wants a research path reconstructed.

Disclose progressively:

1. concise project-level explanation;
2. decision chain and alternatives;
3. specialist Work process and evidence;
4. relevant files and entries;
5. original work traces when still needed.

Do not hide uncertainty, rejected paths, or missing evidence. Do not start with raw logs when a clear synthesis can answer the question.

## PI decision packet

Use when a request changes or reopens the research question, theory, construct, major design, important method compromise, interpretation choice, research story, or final significance.

```markdown
## PI Decision Needed

**Problem**

**Why It Matters**

**Options**

**Trade-offs**

**Recommendation**

**Evidence and Files**

**Decision Deadline / Downstream Block**
```

Recommend a path when evidence supports one, but label the recommendation and leave the decision to the PI. After the PI decides, update `decision_log.md`, affected project files, and Work tasks.

## Stage management

Use the stages as navigation, not a rigid pipeline:

- exploration;
- theory formation;
- research design;
- data collection;
- data analysis;
- writing;
- revision.

At a proposed transition, report:

- whether the current stage is sufficiently complete;
- open risks that carry forward;
- decisions that should be temporarily frozen;
- Works to activate, pause, or retire;
- the next milestone and its entry criteria.

Research may iterate, return to an earlier stage, or reopen a decision. Record the reason and downstream impact rather than treating the return as failure.

## Writing Chat

Writing Chat is `PI ↔ Writing Chat`, the PI’s intellectual workspace for research-story formation, Introduction arguments, Discussion, theoretical interpretation, meaning of key results, and high-judgment prose.

The Orchestrator should not default to drafting these sections. It maintains `writing_handoff.md` from the project’s early stages and prepares a bounded handoff when writing is ready.

```markdown
## Writing Chat Handoff

**Writing Task**

**Why It Is Ready Now**

**Files to Read**

**Confirmed Decisions and Claims**

**PI Judgments or Language to Preserve**

**Evidence and Interpretation Boundaries**

**Rejected Paths That Must Not Reappear**

**Questions Writing Chat Must Discuss with the PI**

**First Action:** Discuss structure / Draft / Revise
```

If the research gap, theoretical position, or interpretation remains open, set the first action to discussion rather than full drafting. After Writing Chat produces confirmed text or new judgments, require those changes to return to the Orchestrator for memory integration and impact review.

## Returning after absence

When the PI returns after days or weeks:

1. provide the Dashboard;
2. identify what changed since the PI’s last confirmed decision;
3. surface unintegrated reports or conflicting state;
4. present only current PI decisions needed;
5. offer Deep Dive links for history without forcing the PI to reread everything.
