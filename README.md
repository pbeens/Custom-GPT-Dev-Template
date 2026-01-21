# Custom GPT Template Repository

This repository serves as a template and workspace for developing, versioning, and testing System Prompts for Custom GPTs.

## Getting Started

### Step 1: Get the Code

**Method A: Download as ZIP (No GitHub Account Required)**
1.  Click the green **"Code"** button at the top of this repository page.
2.  Select **"Download ZIP"**.
3.  Extract the ZIP file to a folder on your computer and open it.

**Method B: Use as Template or Fork (For GitHub Users)**
1.  Click the green **"Use this template"** button at the top of the page to create a new repository in your account.
2.  OR click **"Fork"** in the top-right corner if you want to contribute back.

### Step 2: Start Developing with Antigravity
1.  Open the folder in **Antigravity** (or your preferred AI coding assistant).
2.  Instruct the AI to **"Read gemini.md"** to initialize the session.
3.  The AI will ask you to define the purpose and goals of your Custom GPT.

## Purpose

Developing a high-quality Custom GPT requires iteration. This repository provides a structured way to:
1.  **Version Control your Prompts**: Keep a history of every change to the system instructions.
2.  **Collaborate with AI**: Use the `gemini.md` file to instruct an AI assistant (like me) on how to effectively managing this workflow.
3.  **Test Systematically**: Use valid test cases and specific "skills" (personas) to ensure reliability.

## Directory Structure

```text
.
├── gemini.md                 # Meta-instructions for the AI assistant developing this repo
├── prompts/                  # Directory containing versioned system prompts
│   ├── Prompt_v0.01.md       # Initial Version
│   └── Prompt_v0.02.md       # ...
├── skills/                   # Knowledge base and testing personas
│   ├── Prompt_Engineering.md # Best practices checklist
│   ├── Testing_Personas.md   # Personas to simulate users
│   └── Iterative_Improvement.md # Protocol for testing and refining prompts
└── README.md                 # This file
```

## How to use this Template

1.  **Start a new Session**: When you open this repository with an AI assistant (like Gemini/Antigravity), ask it to "Read gemini.md" first.
2.  **Iterate**: 
    - The AI will look at the latest prompt in `prompts/`.
    - Discuss improvements.
    - The AI will generate the *next* version number (e.g., `Prompt_v0.02.md`).
3.  **Copy to GPT**: Once satisfied, copy the content of the latest prompt file into your Custom GPT's "Instructions" field.

## Security Policy

All prompts generated in this repository adhere to a strict security policy to prevent the leakage of system instructions. This policy is automatically appended to every version.

## Contributing & Feedback
This template is a living document. If you have recommendations for improving this process—such as new skills, better testing workflows, or prompt engineering tips—please suggest them!

**Recommendation Loop**:
1.  Use the `Iterative_Improvement.md` skill to test your changes.
2.  If you find a gap in the process, ask the AI to "Add a new skill" or "Update the README".
