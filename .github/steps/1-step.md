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

### ⌨️ Activity 1: Start a focused review-and-debug branch

1. Create a branch named `feature/review-debug-loop` and make a small intentional bug in any sample file under `src/`.
1. Ask Copilot CLI to review the change before you fix it. You can use `/review` or a natural-language prompt that explains the intended behavior and likely risk.
1. Start `artifacts/step1-workflow-report.md` and add a `## Review findings` section with the most useful review feedback you received.

### ⌨️ Activity 2: Debug, fix, and lock in regression coverage

1. Use Copilot CLI to isolate the root cause, propose a fix, and draft targeted edge-case tests.
1. Apply the fix and add or update tests in `tests/`.
1. Finish `artifacts/step1-workflow-report.md` with these headings:
   - `## Review findings`
   - `## Root cause`
   - `## Fix summary`
   - `## Edge-case assertion`
1. Commit your source, test, and report updates and push `feature/review-debug-loop`.

<details>
<summary>Having trouble? 🤷</summary><br/>

- If you do not have `src/` or `tests/` yet, create them before committing your sample changes.
- Keep the bug small so the review and debugging loop stays focused.
- Keep this branch alive for Steps 2, 3, and 4 so each new capability builds on the same work.
- Keep your report concise; one short paragraph or a short bullet list under each heading is enough.

</details>
