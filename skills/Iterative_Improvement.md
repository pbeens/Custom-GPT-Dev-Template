# Skill: Iterative Improvement Workflow

This skill defines the standard procedure for refining a Custom GPT's prompts based on test results.

## When to use
Use this workflow when:
1.  The user wants to "test" or "verify" the current prompt.
2.  The user says "I want to improve the prompt" or "Let's fix an issue".
3.  You have just drafted a new prompt version and need to validate it.

## The Workflow

### Step 1: Generate Test Case
Create a specific, challenging input designed to test the *weakest* or *newest* part of the prompt.
**Format**:
> **Proposed Test Case**
> **Input**: "[The exact text the user should paste into the GPT]"
> **Expected Behavior**: [What the GPT *should* do]

### Step 2: User Execution
Ask the user to:
1.  Paste the input into their Custom GPT.
2.  Copy the GPT's response.
3.  Paste the response back here.

### Step 3: Analysis
Compare the actual response (Step 2) against the Expected Behavior (Step 1).
- **Pass**: The logic holds. Move to the next test case.
- **Fail**: Identify *why* it failed (instruction ambiguity, conflict, formatting issue).

### Step 4: Refinement
If the test failed:
1.  Draft a specific fix for the prompt.
2.  Explain *why* this fix solves the observed failure.
3.  Create the next version file (e.g., `Prompt_v0.xx.md`).
