# Developer Instructions

This document contains instructions for developing and maintaining the System Prompts in this repository.

## Getting Started

### Step 1: Get the Code

**Method A: Download as ZIP (No GitHub Account Required)**

1. Click the green **"Code"** button at the top of this repository page.
2. Select **"Download ZIP"**.
3. Extract the ZIP file to a folder on your computer and open it.

**Method B: Use as Template or Fork (For GitHub Users)**

1. Click the green **"Use this template"** button at the top of the page to create a new repository in your account.
2. OR click **"Fork"** in the top-right corner if you want to contribute back.

### Step 2: Start Developing

If you don't already have an agentic editor of choice, I recommend **[Antigravity](https://antigravity.google/)**, which automates the entire development process for you. If you'd like to use it:

1. **Install Antigravity**: Download it from [antigravity.google](https://antigravity.google/).
2. **Open the Project**:
    - Launch Antigravity.
    - Click **"Open Folder"**.
    - Select the folder you just extracted (from Step 1).
3. **Initialize the Agent**:
    - In the chat interface, type: **"Read PROTOCOL.md"**.
    - The AI will read the instructions and ask you to define the purpose and goals of your Custom GPT.

**If you prefer to use another AI assistant** (GitHub Copilot, Claude Code, OpenAI Codex, or Custom ChatGPT):

1. **Open the Project**: Open the extracted folder in your preferred IDE or code editor.
2. **Access the AI Assistant**: Open the chat/assistant interface in your tool.
3. **Initialize the Workflow**:
    - Paste the contents of **PROTOCOL.md** into the chat, or ask the AI to read it.
    - The AI will guide you through defining your Custom GPT's purpose and goals.
    - Follow the same iterative process outlined below.

## Purpose

Developing a high-quality Custom GPT requires iteration. This repository provides a structured way to:

1. **Version Control your Prompts**: Keep a history of every change to the system instructions.
2. **Collaborate with AI**: Use the `PROTOCOL.md` file to instruct any AI assistant (Antigravity, GitHub Copilot, Claude Code, OpenAI Codex, or Custom ChatGPT) on how to effectively manage this workflow.
3. **Test Systematically**: Use valid test cases and specific "skills" (personas) to ensure reliability.

## Directory Structure

```text
.
├── PROTOCOL.md               # Meta-instructions for the AI (Antigravity/Gemini/Claude)
├── prompts/                  # Directory containing versioned system prompts
│   ├── Prompt_v0.00.md       # Template Version
│   └── Prompt_v0.01.md       # ...
├── skills/                   # Knowledge base and testing personas
│   ├── Prompt_Engineering.md # Best practices checklist
│   ├── Testing_Personas.md   # Personas to simulate users
│   └── Iterative_Improvement.md # Protocol for testing and refining prompts
├── GEMINI.md                 # Development instructions (This file)
└── README.md                 # Product landing page
```

## How to use this Template

> **Pro Tip**: It is highly recommended to dictate to this tool instead of typing. This will make you much more productive and allow for a more natural conversation flow.

1. **Start a new Session**: When you open this repository with any AI assistant (Antigravity, GitHub Copilot, Claude Code, OpenAI Codex, Gemini, or Custom ChatGPT), ask it to "Read PROTOCOL.md" first.
2. **Test the Prompt**:
    - The AI will create test situations based on the testing personas and skills in this repository.
    - Run the test scenario with the current Custom GPT and capture the output.
    - Bring the output back into this environment for analysis.
3. **Analyze & Iterate**:
    - Discuss what worked and what didn't.
    - Identify gaps or areas for improvement in the prompt.
    - The AI will generate the *next* version number (e.g., `Prompt_v0.01.md`) with refined instructions if necessary.
4. **Repeat**: Continue testing and refining until the Custom GPT performs as expected.
5. **Deploy**: Once satisfied, copy the latest prompt file into your Custom GPT's "Instructions" field.

## Maintenance Guidelines

### Updating the Changelog
>
> **CRITICAL**: Whenever a new prompt version is created (e.g., `prompts/Prompt_v0.01.md`), the `CHANGELOG.md` file MUST be updated immediately.

**Instructions**:

1. Open `CHANGELOG.md`.
2. Add a new section for the new version number (e.g., `## [v0.01] - YYYY-MM-DD`).
3. List all substantive changes, improvements, and fixes included in that version.
