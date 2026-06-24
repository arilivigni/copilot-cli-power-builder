---
name: GitHub Skills Exercise
about: Template for creating a new GitHub Skills exercise
title: 'Copilot CLI Power Builder'
labels: 'skills'
assignees: ''

---

# Logistics

- **Exercise Title:** Copilot CLI Power Builder
- **Repo URL:** https://github.com/arilivigni/copilot-cli-power-builder
- **Experience Level**: Advanced
- **Recommended Grouping**: DevOps and Developer Workflow

### Relationships to other exercises

- **Previous Exercise:** https://github.com/github/copilot-cli-for-beginners
- **Next Exercise:** Advanced team-scale Copilot CLI governance and standardization

---

# Outline

## Story Plot

You are the lead engineer for a fast-moving platform team. Your mission is to turn Copilot CLI into a dependable advanced workflow engine by combining deep development assistance, specialization, automation, external context, and a complete end-to-end delivery flow.

## README

**Title:** Copilot CLI Power Builder

Build advanced Copilot CLI workflows that move from tactical coding help to repeatable, context-aware feature delivery. This exercise teaches how to combine development workflows, specialized assistants, reusable skills, MCP integrations, and full PR execution.

### Overview

1. Use Copilot CLI for high-signal code review, debugging, and targeted test generation.
1. Specialize Copilot behavior for your workflow with custom instructions.
1. Automate repetitive work with reusable Copilot CLI skills.
1. Connect Copilot CLI to GitHub and external systems through MCP.
1. Deliver a complete feature workflow that combines all advanced capabilities.

### What you will build

You will build an advanced workflow scaffold for a feature branch lifecycle, including instruction files, reusable skills, MCP configuration, and PR-ready artifacts. By the end, you will run a complete Copilot CLI-driven delivery loop with measurable validation points. The outcome is a reusable pattern your team can apply to real projects.

### Prerequisites

- Completion of GitHub Copilot CLI beginner content.
- Working knowledge of pull requests, branching, and GitHub Actions.
- Ability to run Copilot CLI locally and push commits to GitHub.
- Familiarity with JSON/YAML configuration and API concepts.

## Step 1 - Development Workflows with Copilot CLI

### Theory

Copilot CLI can accelerate advanced development loops by helping with structured code review, root-cause debugging, and test generation tied to code changes.

- A strong workflow starts by scoping prompts to a concrete change set and expected behavior.
- Debugging quality improves when prompts include failing scenarios and error context.
- Test generation is most useful when focused on edge cases and regressions introduced by current diffs.

### References

- https://docs.github.com/en/copilot
- https://docs.github.com/en/pull-requests
- https://github.blog/changelog/

### Activity: Run an advanced review-debug-test loop

1. Create a feature branch and make a small change with one intentional defect.
1. Use Copilot CLI to review the change, isolate likely root cause, and propose a fix.
1. Generate targeted tests for the fix and commit both code and tests.

### Transition

- **Actions Trigger:** [`push`](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#push)
- **Grading-Check:** Verify branch contains source and test file updates in the same commit range.
- **Grading-Check:** Verify tests include at least one new edge-case assertion linked to the change.

## Step 2 - Create Specialized AI Assistants

### Theory

Specialized assistants improve consistency by encoding project-specific expectations into Copilot context, so outputs align with team conventions.

- Custom instructions reduce repeated prompt setup and enforce stable response patterns.
- Specialization is most effective when it defines coding standards, testing expectations, and output format.
- Consistency enables faster review cycles and fewer prompt corrections.

### References

- https://docs.github.com/en/copilot/how-tos/custom-instructions
- https://docs.github.com/en/copilot
- https://code.visualstudio.com/docs/copilot/overview

### Activity: Configure specialization for your workflow

1. Add repository custom instructions focused on code quality and test expectations.
1. Re-run a Copilot CLI task from Step 1 and compare output alignment.
1. Commit the instruction files and document one measurable improvement.

### Transition

- **Actions Trigger:** [`push`](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#push)
- **Grading-Check:** Verify instruction files exist and include required keyphrases for quality and testing.
- **Grading-Check:** Verify comparison note is committed and references before/after behavior.

## Step 3 - Automate Repetitive Tasks with Skills

### Theory

Copilot CLI skills package repeatable prompting patterns into reusable building blocks, reducing manual repetition and improving output consistency.

- Skills work best when scoped to a recurring engineering activity with predictable outputs.
- Reusable workflows improve team-wide consistency for reviews, triage, and release prep.
- Clear output structure makes skill results easier to validate automatically.

### References

- https://docs.github.com/en/copilot
- https://docs.github.com/en/actions
- https://learn.github.com/skills

### Activity: Build and run a reusable skill

1. Define a skill that generates a PR risk and test-gap summary.
1. Run the skill against your active branch and produce a structured report artifact.
1. Commit the skill definition and generated artifact.

### Transition

- **Actions Trigger:** [`push`](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#push)
- **Grading-Check:** Verify skill definition file exists with required metadata fields.
- **Grading-Check:** Verify generated report artifact includes risk and test-gap sections.

## Step 4 - Connect to GitHub, Databases & APIs with MCP

### Theory

MCP servers let Copilot CLI access external context sources so responses can be grounded in live system information instead of local assumptions alone.

- External context improves prioritization and decision quality during feature development.
- MCP setups should define clear source boundaries and expected query outcomes.
- Validation logs help teams trust context-aware output during reviews.

### References

- https://docs.github.com/en/copilot
- https://docs.github.com/en/rest
- https://docs.github.com/en/graphql

### Activity: Add and validate MCP context

1. Configure one MCP server connection to a GitHub/API/database source.
1. Use Copilot CLI to produce a context-aware engineering summary.
1. Commit MCP configuration and a validation log that records query source and outcome.

### Transition

- **Actions Trigger:** [`push`](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#push)
- **Grading-Check:** Verify MCP configuration file exists and follows expected schema shape.
- **Grading-Check:** Verify validation log captures source queried and resulting action recommendation.

## Step 5 - Putting It All Together

### Theory

The highest leverage comes from chaining specialized instructions, reusable skills, and MCP context into one end-to-end PR workflow.

- End-to-end integration demonstrates operational value beyond isolated techniques.
- A complete feature loop should include implementation, tests, context checks, and review iteration.
- Repeatable validation criteria make the workflow suitable for team adoption.

### References

- https://docs.github.com/en/actions
- https://docs.github.com/en/pull-requests
- https://learn.github.com/skills

### Activity: Deliver a complete advanced feature workflow

1. Build a second small feature on a new branch using the specialized instructions.
1. Run your reusable skill and MCP context checks before opening the PR.
1. Open a PR, address one review round with Copilot CLI support, and update tests if needed.

### Transition

- **Actions Trigger:** [`pull_request_review`](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#pull_request_review)
- **Grading-Check:** Verify PR includes links or artifacts from Steps 2, 3, and 4.
- **Grading-Check:** Verify at least one post-review commit resolves feedback and keeps checks green.

## Review

This exercise built a full advanced Copilot CLI delivery system from targeted development assistance to integrated feature execution. Learners practiced specialization, automation, external context integration, and iterative PR delivery with quality checks.

- Running advanced review, debug, and test generation loops with Copilot CLI.
- Specializing AI assistant behavior for project standards.
- Automating recurring tasks through reusable skills.
- Integrating MCP context from GitHub and external systems.
- Executing end-to-end feature workflows with validation checkpoints.

### What's next?

- https://docs.github.com/en/copilot
- https://docs.github.com/en/actions
- https://learn.github.com/skills

# Future Considerations

- Add a team-scale variant with organization-level instruction and skill sharing.
- Introduce security and compliance gates as first-class workflow checks.
- Expand MCP usage to multi-source decision pipelines (issues, telemetry, and change history).
