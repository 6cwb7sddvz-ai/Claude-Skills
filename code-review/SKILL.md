---
name: code-review
description: Perform structured code reviews covering correctness, style, security, performance, and tests.
---

# Code Review

Use this skill when reviewing code changes or pull requests.

## Review checklist
- Correctness: does the code do what it claims? Edge cases handled?
- Readability: clear naming, small functions, sensible structure
- Security: input validation, no secrets, safe dependencies
- Performance: avoid needless allocations, N+1 queries, tight loops
- Tests: adequate coverage for new and changed behavior
- Docs: comments and docs updated where needed

## Workflow
1. Read the PR description and understand intent.
2. Review file by file, leaving specific, actionable comments.
3. Prefer suggestion blocks so authors can apply fixes in one click.
4. Summarize with an overall verdict: approve, comment, or request changes.
