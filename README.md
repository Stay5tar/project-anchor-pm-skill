# ⚓ Project Anchor PM (项目锚点管家)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Prompt: Project Management](https://img.shields.io/badge/Prompt-Project_Management-success)](#)
[![Language: Bilingual](https://img.shields.io/badge/Language-English%20%7C%20%E4%B8%AD%E6%96%87-orange)](#)

[English](#english-version) | [中文说明](#chinese-version)

---

<h2 id="english-version">🇬🇧 English Version</h2>

### 📌 Introduction
A system prompt skill that acts as a strict Agile Project Manager. It forces your focus back to the current development node by isolating any new ideas or feature creeps into a structured "Parking Lot" backlog.

Use it when you want to stop getting distracted by shiny new ideas, avoid project scope creep, or just need an AI to aggressively keep your indie project on track.

### ⚠️ The Problem
When building personal projects, developers often come up with brilliant new features on the fly. However, chasing these new ideas usually leads to:
- Disrupted "flow state" in coding.
- Loss of project logic and structure.
- Endless "Scope Creep" resulting in unfinished projects (Vaporware).

### 💡 The Solution: Dual-Track Agile + Parking Lot
This prompt enforces a strict framework:
1. **Focus Isolation:** Formats any new idea you dump into a 7-element "Parking Lot" card, then aggressively pulls the conversation back to the current milestone.
2. **Expedite Lane for Severe Bugs:** Only explicitly declared critical bugs can interrupt the current sprint.
3. **Resource Trade-off Rule:** If you insist on building a new feature *now*, the AI forces you to declare which current task will be delayed.

### 🚀 Install & Usage

Choose the language that fits your workflow. For English, use [`SKILL-EN.md`](./SKILL-EN.md).

**1. For standard web AIs (ChatGPT, Claude, Gemini):**
Copy the content of `SKILL-EN.md` and paste it into your AI's **Custom Instructions** or **Claude Projects**.

**2. For CLI agents (Claude Code, Codex, Workbuddy):**
Drop the `SKILL-EN.md` into your skills directory. You can rename it to `SKILL.md` if your tool requires it.

```bash
# For Claude Code
~/.claude/skills/project-anchor-pm/SKILL.md

# For Codex / Workbuddy
~/.codex/skills/project-anchor-pm/SKILL.md
```

Then trigger it by saying "I have a new idea" or asking the AI to record a new feature for the project.

---

<h2 id="chinese-version">🇨🇳 中文说明</h2>

### 📌 简介
一个扮演严厉敏捷项目经理的系统提示词技能。它通过将你的任何新想法或发散需求隔离到一个结构化的“停车场”积压任务中，强制把你的注意力拉回当前的开发节点。

当你不想再被突发奇想的新点子分散注意力、想要避免项目范围蔓延，或者单纯需要一个 AI 来强硬地推进你的独立项目进度时，请使用它。

### ⚠️ 痛点
在做项目的过程中，我们经常会突发奇想加入各种新功能。但这往往导致：
- 打断当前的开发心流（Flow State）。
- 项目主线偏离，逻辑变得混乱。
- 永远做不完，最终导致项目彻底烂尾。

### 💡 解决方案：双轨敏捷 + 停车场机制
此技能赋予 AI 以下强制约束力：
1. **焦点隔离：** 当你倾倒新想法时，AI 会将其格式化为“7要素需求卡”放入远期规划（停车场），并立刻输出“进度看板”把你的注意力强行拉回当前任务。
2. **紧急插队机制：** 只有你明确指出是“严重阻断性 Bug”，AI 才会停止主线推进，陪你救火。
3. **资源置换法则：** 想要立刻执行新需求？AI 会强制要求你明确“哪些现有工作顺延”，确保进度表永远符合物理逻辑。

### 🚀 安装与使用 (Install)

请根据你的工作流语言选择对应的提示词文件。中文环境请使用 [`SKILL-ZH.md`](./SKILL-ZH.md)。

**1. 常规网页端 AI (ChatGPT, Claude, Gemini)：**
直接复制 `SKILL-ZH.md` 里的所有内容，粘贴到 **自定义指令 (Custom Instructions)** 或 **Claude Projects 提示词** 中。

**2. 命令行 AI 工具 (Claude Code, Codex, Workbuddy)：**
将 `SKILL-ZH.md` 直接放入你所使用的 AI 工具的 skills 目录中（可视工具要求重命名为 `SKILL.md`）：

```bash
# Claude Code
~/.claude/skills/project-anchor-pm/SKILL.md

# Codex / Workbuddy
~/.codex/skills/project-anchor-pm/SKILL.md
```

安装完成后，当你遇到发散思维时，直接说“我有个新点子”，即可触发敏捷管理技能。

### 🎬 演示 (Showcase)

**User:** “我有个新点子，需要在当前的录入界面加一个内置计算器功能，方便边看边算。”

**AI Response:**
> **[新需求：内置计算器面板]**
> * **解决什么问题：** 用户无需切出应用即可进行金额计算，提升录入连贯性与转化率。
> * **属于哪一阶段：** 远期规划（停车场）。
> * **优先级及理由：** P2。属于锦上添花的体验优化。当前主线是跑通核心数据写入逻辑，不能因引入 UI 组件干扰主线。
> ... (剩余部分自动归档) ...
> 
> **[当前项目状态看板]**
> * **当前侧重：** 核心表单数据的提交验证与后端存储链路。
> * **进行到哪一步：** 聚焦于必填字段的正则校验逻辑。
> * **下一步及完成条件：** 继续攻克表单校验，直到成功将一条完整数据写入数据库并返回成功提示。
