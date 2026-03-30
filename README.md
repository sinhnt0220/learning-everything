# Knowledge Architect (Ms. Nguyen Persona)

An autonomous AI agent skill that transforms your standard AI into **Ms. Nguyen**—a rigorous, structured, and Socratic Learning Director. It stops the AI from simply "answering questions" and forces it to build structured curriculums, test your understanding, and debug your logic.

## 🌟 Overview

Tired of linear, shallow AI tutorials? The Knowledge Architect skill forces you to learn via First Principles. 

- **Socratic Diagnosis:** It refuses to just teach you. It asks you what you already know first, and brutally points out your misconceptions.
- **Universal & PKM Friendly:** Supports plain computer folders OR can automatically inject YAML frontmatter to power up your Obsidian/Logseq Knowledge Graph.
- **Ruthless Debugging:** You must complete an "Active Recall Sandbox" before moving on. The AI will point out logical flaws directly (trigger warning: zero flattery).

## 🚀 Installation

Install this skill globally to any standard open agent runtime (like Claude Code, Antigravity, AutoGPT) via the Skills CLI:

```bash
npx skills add <YOUR-GITHUB-USERNAME>/<REPO-NAME>@.agents/skills/feifei-os-public
```
*(You will replace the username and repo name above with your actual GitHub info once you publish it).*

## 💡 How to Use

Start a chat with your AI Agent and trigger the workflow using these commands:

### 1. The Entry Point: `/learn [Subject]`
Ask the AI to design a course.
> **Example:** `/learn Systems Thinking`
The AI will ask you a few diagnostic questions and prompt you for a Root Folder on your machine. It then generates a Master `Learning_Map_MoC.md`.

### 2. Start a Lesson: `/start-module [Module Name]`
Tell the AI to begin one of the modules in the learning map.
> **Example:** `Attach your MoC file, then type: /start-module 01-Introduction` 
It will generate a structured lesson with a blank "Active Recall Sandbox". Do the homework.

### 3. Get Graded: `/complete-module`
Submit your homework for ruthless grading.
> **Example:** `Attach your Module file + MoC file, then type: /complete-module`
Ms. Nguyen will debug your logic, leave an assessment in the file, and automatically update your Master Map's status.

### 4. Deep Dives: `/define [Concept]`
Extract a standalone concept.
> **Example:** `/define Emergence`
The AI will break it down by definition, mechanism, multi-disciplinary impact, and analogies, saving it into your folder.

---
*Built with strict pedagogy from the heart of Vietnam.*
