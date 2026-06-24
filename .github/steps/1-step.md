## Step 1: Development Workflows with Copilot CLI

You are kickstarting a high-signal engineering workflow and need to prove Copilot CLI can help review changes, debug issues, and drive focused test generation.

### 📖 Theory: Review, debug, and test as one loop

Copilot CLI can accelerate advanced development loops when prompts are scoped to concrete diffs and expected behavior.

- Structured prompts improve code-review signal by focusing on change intent and risk.
- Debug prompts become more reliable when they include failing behavior and error context.
- Test prompts are strongest when asking for edge-case and regression coverage tied to the fix.

Read more:
- https://docs.github.com/en/copilot
- https://docs.github.com/en/pull-requests
- https://github.blog/changelog/

### ⌨️ Activity: Run an advanced review-debug-test loop

1. Create a branch named `feature/step-1-workflow` and make a small intentional bug in any sample file under `src/`.
1. Use Copilot CLI to identify root cause, propose a fix, and draft targeted edge-case tests.
1. Apply the fix and add tests in `tests/`.
1. Create `artifacts/step1-workflow-report.md` with these headings:
   - `## Root cause`
   - `## Fix summary`
   - `## Edge-case assertion`
1. Commit your source, test, and report updates and push your branch.

<details>
<summary>Having trouble? 🤷</summary><br/>

- If you do not have `src/` or `tests/` yet, create them before committing your sample changes.
- Keep your report concise; one short paragraph under each heading is enough.

</details>
