# Research PI Orchestrator

[中文](#中文) | [English](#english)

> Manage AI research teams like a PI: reduce coordination overhead, preserve shared research memory, and stay in control of critical research decisions.

An instruction-only Codex Skill for coordinating long-running research projects involving a human PI, multiple specialized AI Works, and an independent Writing Chat.

---

## 中文

### 这是什么

Research PI Orchestrator 帮助研究者像 PI（Principal Investigator）一样管理由多个 AI Work 共同参与的长期科研项目。

它解决的是多 Work 协作中的三个管理问题：

- **少协调**：降低任务分派、交接、同步和追踪成本；
- **能把控**：关键研究判断始终由研究者决定；
- **可追溯**：项目状态、证据、决策理由和写作材料都能恢复。

核心理念：

> **The goal is not to automate research. The goal is to scale the PI.**

> **Flat intellectual collaboration, centralized project memory.**

Research Orchestrator 是同步中心和共享项目记忆的维护者。

### 适合什么场景

- 建立或恢复一个长期科研项目；
- 协调 Literature、Theory、Design、Analysis、Reviewer 等多个专业 Work；
- 为每个 Work 建立 Read / Write / Report / Escalation 协议；
- 管理项目状态、任务闭环、决策升级和历史追溯；
- 从项目第一天开始为独立 Writing Chat 积累写作交接材料；
- PI 暂离项目后快速恢复方向、进度、风险和待决策事项。

以下场景通常不需要本 Skill：

- 一次性的文献检索；
- 单独的数据分析；
- 普通论文润色或直接起草正文；
- 不涉及项目级协作的一次性科研方法问题。

### 七条硬规则

1. 总控默认协调；新的实质研究知识优先交给专业 Work。
2. 每个 Work 加入项目前必须有明确的 Memory Contract。
3. 任务必须形成 `Assign → Execute → Update Files → Report → Review → Integrate` 闭环。
4. PI 可以直接访问任何 Work，但重要变化必须回流统一项目记忆。
5. 学术协作保持扁平；总控是同步中心，不是沟通瓶颈。
6. 默认提供 Dashboard；PI 需要时必须能够完整 Deep Dive。
7. **Chat is workspace. Files are memory.** 文件保存完整信息，对话只传增量信息。

### 项目记忆

总控默认维护以下核心文件：

- `project_state.md`：当前阶段、进度、风险、PI 待决策事项和下一里程碑；
- `team_structure.md`：团队结构、任务状态及各 Work 的 Memory Contract；
- `decision_log.md`：关键决策、备选方案、理由、影响及重新打开原因；
- `evidence_bank.md`：进入研究判断的证据、强度、边界、反证和用途；
- `writing_handoff.md`：研究故事、论证链、设计理由、结果边界、PI 判断及待讨论问题。

专业 Work 可按需维护 `literature_map.md`、`theory_notes.md`、`design_plan.md`、`analysis_plan.md`、`analysis_results.md`、`reviewer_notes.md` 等文件。不要为了结构完整而机械创建全部文件。

### 安装

#### 方法一：让 Codex 安装（推荐）

在 Codex 中调用 `$skill-installer`，然后输入：

```text
Install the skill from https://github.com/Guojiangjiang-psycho/research-pi-orchestrator
```

安装后，新建一个 Codex 任务即可使用。

#### 方法二：手动安装

```bash
git clone https://github.com/Guojiangjiang-psycho/research-pi-orchestrator.git
cp -R research-pi-orchestrator ~/.codex/skills/
```

然后重新打开 Codex，或开始一个新任务。

### 快速开始

在一个科研项目目录中调用：

```text
$research-pi-orchestrator
请作为本项目的 Research Orchestrator，读取现有材料，判断当前阶段，建立最小必要的项目记忆，并给我一个 PI Dashboard 和团队组建建议。
```

如果项目已经进行了一段时间，可以使用：

```text
$research-pi-orchestrator
请恢复这个科研项目：告诉我现在在哪里、已经决定了什么、还缺什么、下一步是什么。先给 Dashboard，需要时再 Deep Dive。
```

### Skill 结构

```text
research-pi-orchestrator/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── pi-interface.md
    ├── project-memory.md
    ├── roles-and-contracts.md
    ├── task-protocols.md
    └── validation-scenarios.md
```

主文件 [SKILL.md](SKILL.md) 只保留影响运行行为的核心规则；角色模板、Memory Contract、Dashboard、任务反馈模板和测试场景位于 [references](references/) 中。本 Skill 为 instruction-only，不包含脚本。

### 研究者始终拥有最终决定权

专业 Work 可以搜集证据、深入分析、质疑方案并提出建议，但不能静默修改研究问题、核心理论、核心构念、重大设计、关键结果解释或论文观点。涉及这些内容时，总控必须整理选项、权衡和建议，并升级给 PI 决定。

Writing Chat 也被有意保留为独立空间：它是 PI 参与研究故事、理论解释和高思考密度写作的 intellectual workspace，而不是普通专业 Work。

---

## English

### What it is

Research PI Orchestrator helps researchers manage long-running projects involving multiple AI Works as a Principal Investigator would.

Its purpose is not to automate the research process. It addresses three coordination problems:

- **Less coordination overhead** across delegation, handoffs, synchronization, and tracking;
- **Human control** over consequential research judgments;
- **Traceability** of project state, evidence, decisions, and writing rationale.

Core idea:

> **The goal is not to automate research. The goal is to scale the PI.**

The organizational model is not a rigid `PI → controller → subordinate Works` hierarchy. It is:

> **Flat intellectual collaboration, centralized project memory.**

The Research Orchestrator is a synchronization center and steward of shared project memory—not the academic superior of specialized Works.

### When to use it

- Establishing or recovering a long-running research project;
- Coordinating Literature, Theory, Design, Analysis, Reviewer, or other specialized Works;
- Defining Read / Write / Report / Escalation contracts for each Work;
- Managing project state, task closure, decision escalation, and historical traceability;
- Accumulating writing-ready material for an independent Writing Chat from day one;
- Restoring direction, progress, risks, and pending PI decisions after time away.

This Skill is usually unnecessary for:

- A standalone literature search;
- A one-off data analysis;
- Ordinary paper editing or direct manuscript drafting;
- A single research-method question without project-level orchestration.

### Seven non-negotiable rules

1. Coordinate by default; delegate the creation of substantive research knowledge.
2. No Work joins the project without a clear Memory Contract.
3. Every task closes through `Assign → Execute → Update Files → Report → Review → Integrate`.
4. The PI may access any Work directly, but material changes must return to shared project memory.
5. Intellectual collaboration stays flat; the orchestrator synchronizes rather than bottlenecks communication.
6. Use Dashboard mode by default and support a complete Deep Dive on request.
7. **Chat is workspace. Files are memory.** Files hold full context; chat carries deltas.

### Project memory

The orchestrator maintains five core files by default:

- `project_state.md`: stage, progress, risks, PI decisions needed, and next milestone;
- `team_structure.md`: team status, assignments, and each Work's Memory Contract;
- `decision_log.md`: decisions, alternatives, rationale, consequences, and reopening reasons;
- `evidence_bank.md`: decision-relevant evidence, strength, boundaries, counterevidence, and intended use;
- `writing_handoff.md`: research story, argument chain, design rationale, result boundaries, PI judgments, and unresolved questions.

Specialized Works may maintain files such as `literature_map.md`, `theory_notes.md`, `design_plan.md`, `analysis_plan.md`, `analysis_results.md`, and `reviewer_notes.md` when needed. Do not create every file mechanically.

### Installation

#### Option 1: Install through Codex (recommended)

Invoke `$skill-installer` in Codex, then enter:

```text
Install the skill from https://github.com/Guojiangjiang-psycho/research-pi-orchestrator
```

Start a new Codex task after installation.

#### Option 2: Install manually

```bash
git clone https://github.com/Guojiangjiang-psycho/research-pi-orchestrator.git
cp -R research-pi-orchestrator ~/.codex/skills/
```

Then reopen Codex or start a new task.

### Quick start

From a research project directory, invoke:

```text
$research-pi-orchestrator
Act as the Research Orchestrator for this project. Read the existing materials, identify the current stage, establish the minimum necessary project memory, and give me a PI Dashboard plus a team formation recommendation.
```

For an existing project:

```text
$research-pi-orchestrator
Recover this research project: tell me where we are, what has been decided, what is missing, and what should happen next. Start with a Dashboard and Deep Dive only when needed.
```

### Skill layout

```text
research-pi-orchestrator/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── pi-interface.md
    ├── project-memory.md
    ├── roles-and-contracts.md
    ├── task-protocols.md
    └── validation-scenarios.md
```

The main [SKILL.md](SKILL.md) contains only behavior-critical instructions. Role templates, Memory Contracts, Dashboard and reporting formats, and validation scenarios live under [references](references/). This is an instruction-only Skill with no scripts.

### The researcher remains the final decision-maker

Specialized Works may gather evidence, analyze deeply, challenge assumptions, and recommend changes. They must not silently alter the research question, core theory, central constructs, major design choices, key result interpretations, or the paper's position. The orchestrator must frame consequential choices, trade-offs, and recommendations for the PI to decide.

Writing Chat intentionally remains separate. It is the PI's intellectual workspace for shaping the research story, theoretical interpretation, and high-reasoning-density writing—not another routine specialist Work.
