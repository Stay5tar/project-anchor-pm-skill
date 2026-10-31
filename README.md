# ⚓ Project Anchor PM (项目锚点管家)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Prompt: Project Management](https://img.shields.io/badge/Prompt-Project_Management-success)](#)
[![Language: Bilingual](https://img.shields.io/badge/Language-English%20%7C%20%E4%B8%AD%E6%96%87-orange)](#)

[English](#english-version) | [中文说明](#chinese-version)

---

<h2 id="english-version">🇬🇧 English Version</h2>

### 📌 Introduction
**Project Anchor PM** is a system prompt (AI Skill) designed to turn any LLM (ChatGPT, Claude, Gemini) into a strict, highly-disciplined Agile Project Manager. It prevents "scope creep" by isolating new ideas into a Parking Lot, forcing your focus back to the current development node.

### ⚠️ The Problem
When building personal projects, indie hackers and developers often come up with brilliant new features on the fly. However, chasing these new ideas usually leads to:
- Disrupted "flow state" in coding.
- Loss of project logic and structure.
- Endless "Scope Creep" resulting in unfinished projects (Vaporware).

### 💡 The Solution: Dual-Track Agile + Parking Lot
This prompt enforces a strict framework:
1. **Focus Isolation:** Formats any new idea you dump into a 7-element "Parking Lot" card, then aggressively pulls the conversation back to the current milestone.
2. **Expedite Lane for Severe Bugs:** Only explicitly declared critical bugs can interrupt the current sprint.
3. **Resource Trade-off Rule:** If you insist on building a new feature *now*, the AI forces you to declare which current task will be delayed.

### 🚀 How to Use
1. Copy the content of [`system-prompt.md`](./system-prompt.md).
2. Paste it into your AI's **Custom Instructions**, **Claude Projects (Custom Instructions)**, or **Cursor Rules**.
3. Start coding! Whenever you have a random idea, just tell the AI. It will archive it and show you the Current Project Status Board.

---

<h2 id="chinese-version">🇨🇳 中文说明</h2>

### 📌 简介
**项目锚点管家 (Project-Anchor-PM)** 是一个专为独立开发者和创作者设计的 AI 系统提示词（System Prompt / AI Skill）。它能将 LLM 变成一位冷酷且严谨的敏捷项目经理，通过“停车场机制”有效防止项目范围蔓延，确保你顺利交付。

### ⚠️ 痛点
在做项目的过程中，我们经常会突发奇想，想加入各种酷炫的新功能。但这种发散思维往往导致：
- 打断当前的开发心流（Flow State）。
- 项目主线偏离，逻辑变得混乱。
- 永远做不完，最终导致项目彻底烂尾。

### 💡 解决方案：双轨敏捷 + 停车场机制
此技能赋予 AI 以下强制约束力：
1. **焦点隔离：** 当你倾倒新想法时，AI 会将其格式化为“7要素需求卡”放入远期规划（停车场），并立刻输出“进度看板”把你的注意力强行拉回当前任务。
2. **紧急插队机制：** 只有你明确指出是“严重阻断性 Bug”，AI 才会停止主线推进，陪你救火。
3. **资源置换法则：** 想要立刻执行新需求？AI 会强制要求你明确“哪些现有工作顺延”，确保进度表永远符合物理逻辑。

### 🚀 如何使用
1. 复制 [`system-prompt.md`](./system-prompt.md) 文件中的所有内容。
2. 将其粘贴到 ChatGPT 的 **自定义指令 (Custom Instructions)**、Claude 的 **Projects 提示词**，或作为 Cursor 的 `.cursorrules` 文件。
3. 像往常一样开始开发！当你突然想到新点子时，直接发给 AI。它会妥善归档，并用 5 要素看板拉回你的注意力。

### 🎬 演示 (Showcase)
**User:** “我有个新点子，想把相册图片拼接成长图分享。”

**AI Response:**
> **[新需求：瀑布流长图拼接]**
> * **解决什么问题：** 满足用户二次传播需求。
> * **属于哪一阶段：** 远期规划（停车场）。
> * **优先级：** P2。
> ... (自动归档) ...
>
> **[当前项目状态看板]**
> * **当前侧重：** 核心解析链路与基础 UI 闭环。
> * **进行到哪一步：** 聚焦多图网格展示结构。
> * **下一步及完成条件：** 继续攻克网格渲染，直到成功展示长图预览。
