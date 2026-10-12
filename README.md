# AI-Assisted Learn Rules

## Why

Writing real, hands-on projects by hand is the best way to improve your programming skills. This project brings an AI Agent into the loop — not to write code for you, but to guide you. By giving the Agent a set of rules, it becomes a sustainable coach: it explains concepts, breaks the work into small tasks, and reviews your code read-only. You leverage the AI's capability, but the code is always written by you — so the skill truly becomes yours.

亲手编写实战项目，是提升编程技巧最好的方式。本项目引入 AI Agent，但并不是让 AI 直接替你完成编程，而是为 Agent 指定一套规则，让它成为可持续的引导：讲解知识、拆解任务、只读验收。你借力 AI 的能力，代码永远亲手完成，最终提升的是你自己的编程能力。

---

## Tutorial

### Step 1: Create a folder

Create an empty project folder (e.g. `my-project`) — this is where you and the AI will work.

### Step 2: Add the rules to your project

Copy either `AI-RULES.en.md` (English) or `AI-RULES.zh-cn.md` (Chinese) into the empty folder — no renaming, no extra folders:

```
my-project/
└── AI-RULES.en.md      # or AI-RULES.zh-cn.md
```

**This file is the AI's playbook** — the AI reads it at the start of every session and follows it strictly.

### Step 3: Open your AI agent tool

Open your AI agent tool (e.g. Claude Code, Cursor, OpenCode) inside `my-project` and start a session.

### Step 4: Say "Initialize"

Type in the chat:

> **"Initialize"**

The AI will generate 5 initialization artifacts:

| # | Artifact | Path |
|---|----------|------|
| 1 | Project design docs | `docs/project/` |
| 2 | Task backlog | `docs/tasks/backlog.md` |
| 3 | Progress master | `docs/progress.md` |
| 4 | Meta-rules pointer | `AGENTS.md` |
| 5 | Teaching notes | `docs/knowledge/` |

> Check: initialization is done when all 5 artifacts exist and the progress master says "ready to break down".

### Step 5: Start the collaboration loop

```
Break down → Start task → Explain → You code → Self-check → Review → Record
```

Common commands: `Break down tasks` / `Start Txxx` / `I finished Txxx` / `Progress` / `Explain <topic>`

---

## 使用教程

### 第 1 步：创建文件夹

新建一个空的项目文件夹（例如 `my-project`），这是你和 AI 协作的工作区。

### 第 2 步：把规则放进项目

选择中文版 `AI-RULES.zh-cn.md` 或英文版 `AI-RULES.en.md`，直接复制进空文件夹即可——不用改名，也不用建子文件夹：

```
my-project/
└── AI-RULES.en.md      # 或 AI-RULES.zh-cn.md
```

**这份文件就是 AI 的工作手册**，AI 会在每个会话开始时先读它，并严格遵守。

### 第 3 步：打开 AI 工具

在 `my-project` 文件夹里打开你常用的 AI Agent 工具（如 Claude Code、Cursor、OpenCode 等），进入会话。

### 第 4 步：说「初始化」

在对话里输入：

> **「初始化」**

AI 会自动生成 5 项初始化产物：

| # | 产物 | 路径 |
|---|------|------|
| 1 | 项目设计文档 | `docs/project/` |
| 2 | 任务池 | `docs/tasks/backlog.md` |
| 3 | 进度总表 | `docs/progress.md` |
| 4 | 元规则指针 | `AGENTS.md` |
| 5 | 教学笔记目录 | `docs/knowledge/` |

> 验证：5 项全部生成后，进度总表会标注"待拆解"，说明初始化完成。

### 第 5 步：进入协作循环

```
拆任务 → 开始任务 → 讲解背景 → 你写码 → 你自检 → AI 只读验收 → 记录推进
```

常用指令：`拆任务` / `开始 Txxx` / `我完成了 Txxx` / `进度` / `讲解 <主题>`
