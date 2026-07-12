---
name: multi-agent-reviewer-executor
description: Pair an executor agent that does the work with a reviewer agent that validates before finalizing.
---

# Multi-Agent: Reviewer-Executor

Use this pattern when output quality matters and mistakes are costly.

## Roles
- Executor: performs the task and produces a draft result.
- Reviewer: checks the result against requirements and quality criteria.

## When to use
- Code changes, content, or decisions need a quality gate.
- You want to catch errors before they reach the user.
- A second, independent perspective improves reliability.

## Workflow
1. Executor completes the task and returns a draft plus its reasoning.
2. Reviewer evaluates correctness, completeness, and adherence to requirements.
3. If issues are found, Reviewer returns specific feedback to the Executor.
4. Iterate until the Reviewer approves, then finalize.

## Tips
- Give the Reviewer explicit acceptance criteria.
- Keep executor and reviewer roles independent to avoid bias.
- Cap the number of revision loops to prevent stalling.
