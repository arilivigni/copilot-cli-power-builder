## Step 4: Connect to GitHub, Databases & APIs with MCP

You now need context-aware Copilot CLI outputs that incorporate external system data rather than local assumptions only.

### 📖 Theory: MCP as a context bridge

MCP servers let Copilot tools query external systems (GitHub, APIs, databases) so recommendations are grounded in real state.

- External context improves prioritization and decision quality.
- Controlled MCP configuration keeps data sources explicit and auditable.
- Validation logs help reviewers trust context-aware recommendations.

Read more:
- https://docs.github.com/en/copilot
- https://docs.github.com/en/rest
- https://docs.github.com/en/graphql

### ⌨️ Activity: Add and validate MCP context

1. Add MCP configuration at `.vscode/mcp.json` for one source (GitHub API, an API endpoint, or a database integration).
1. Use Copilot CLI to produce a context-aware summary that combines branch work and MCP source data.
1. Create `artifacts/step4-mcp-validation-log.md` with headings:
   - `## Source queried`
   - `## Context returned`
   - `## Action recommendation`
1. Commit MCP configuration and validation log.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Start with one MCP source only; keep scope narrow for easier validation.
- Include enough detail in the log so a reviewer can understand where context came from.

</details>
