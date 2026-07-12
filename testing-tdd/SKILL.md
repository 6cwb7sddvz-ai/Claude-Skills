---
name: testing-tdd
description: Write tests and follow test-driven development to scaffold reliable, well-covered code.
---

# Testing / TDD

Use this skill when adding tests or building features test-first.

## Principles
- Red-green-refactor: write a failing test, make it pass, then clean up.
- Test behavior, not implementation details.
- Keep tests fast, isolated, and deterministic.
- Cover happy paths, edge cases, and error handling.

## Recommended tools
- pytest (Python), Jest or Vitest (JS/TS), JUnit (Java)
- Coverage tools: coverage.py, c8/nyc

## Workflow
1. Write a small failing test that describes the desired behavior.
2. Implement the minimum code to pass it.
3. Refactor with tests green.
4. Check coverage and add tests for uncovered branches.
