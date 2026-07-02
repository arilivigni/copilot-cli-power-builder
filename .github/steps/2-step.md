## Step 2: Create Specialized AI Assistants

Now you need Copilot CLI output to consistently match team standards without rewriting prompt context every time.

### 📖 Theory: Specialization through agents and repository instructions

Specialized assistant behavior comes from reusable prompts and instructions that encode coding standards, testing expectations, and output conventions.

- Custom agents give Copilot CLI a focused role for a specific kind of work.
- Repository instructions reduce repeated prompt setup across every session.
- Standardized response formats shorten review cycles and improve generated test quality.

Read more:
- https://docs.github.com/en/copilot/how-tos/custom-instructions
- https://docs.github.com/en/copilot
- https://code.visualstudio.com/docs/copilot/overview

### ⌨️ Activity 1: Create a specialist for the branch you already started

1. Stay on `feature/review-debug-loop` so you can improve the same workflow from Step 1 instead of starting over.
1. Create `.github/agents/workflow-reviewer.agent.md` for a specialist that reviews workflow changes, test expectations, and artifact completeness.
1. Run that agent against the Step 1 work on `feature/review-debug-loop`.
1. Capture the agent you used in `artifacts/step2-specialization-comparison.md` under `## Agent used`.

### ⌨️ Activity 2: Add always-on repository guidance

1. Create `.github/copilot-instructions.md` with sections for coding standards, testing expectations, and output format.
1. Re-run one Copilot CLI prompt from Step 1 and compare how the response changes after adding your repository instructions.
1. Finish `artifacts/step2-specialization-comparison.md` with these headings:
   - `## Agent used`
   - `## Before/after`
   - `## Improvements observed`
1. Commit the agent file, instruction file, and comparison artifact to `feature/review-debug-loop`.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Keep both the agent and instructions specific and action-oriented; avoid vague style guidance.
- If your comparison is short, include at least one concrete difference in output structure or test expectations.
- The goal is to improve the exact workflow you established in Step 1, not to invent a separate exercise branch.

</details>
