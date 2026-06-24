## Step 2: Create Specialized AI Assistants

Now you need Copilot CLI output to consistently match team standards without rewriting prompt context every time.

### 📖 Theory: Specialization through repository instructions

Specialized assistant behavior comes from clear, reusable instructions that encode coding standards, testing expectations, and output conventions.

- Repository instructions reduce repeated prompt setup.
- Standardized response formats shorten review cycles.
- Explicit testing expectations improve generated test quality.

Read more:
- https://docs.github.com/en/copilot/how-tos/custom-instructions
- https://docs.github.com/en/copilot
- https://code.visualstudio.com/docs/copilot/overview

### ⌨️ Activity: Configure specialization for your workflow

1. Create `.github/copilot-instructions.md` with sections for coding standards, testing expectations, and output format.
1. Re-run one Copilot CLI prompt from Step 1 and compare response quality.
1. Create `artifacts/step2-specialization-comparison.md` with headings:
   - `## Before/after`
   - `## Improvements observed`
1. Commit the instruction file and comparison artifact.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Keep instructions specific and action-oriented; avoid vague style guidance.
- If your comparison is short, include at least one concrete difference in output structure.

</details>
