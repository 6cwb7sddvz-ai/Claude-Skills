---
name: multi-agent-orchestrator-worker
description: Coordinate a lead agent that decomposes a task, delegates to worker agents, and synthesizes results.
---

# Multi-Agent: Orchestrator-Worker

Use this pattern for large tasks that can be split into parallel subtasks.

## Roles
- Orchestrator: plans, splits work, assigns subtasks, and merges outputs.
- Workers: each handles one focused subtask and returns a result.

## When to use
- The task has independent parts that can run in parallel.
- Subtasks need different tools or expertise.
- A single agent context would be overloaded.

## Workflow
1. Orchestrator analyzes the goal and defines subtasks with clear inputs and outputs.
2. Spawn one worker per subtask with only the context it needs.
3. Workers return structured results.
4. Orchestrator validates, resolves conflicts, and synthesizes the final answer.

## Tips
- Give each worker a narrow, well-specified brief.
- Define the output schema up front so results merge cleanly.
- Have the orchestrator double-check completeness before finishing.
