---
name: multi-agent-handoff-protocol
description: A standard format for one agent to pass context and responsibility to another cleanly.
---

# Multi-Agent: Handoff Protocol

Use this pattern when work moves between agents and context must transfer without loss.

## Handoff payload
Include these fields when handing off:
- goal: the overall objective.
- completed: what has been done so far.
- current_state: relevant data, files, or results.
- next_action: what the receiving agent should do.
- constraints: limits, deadlines, and requirements.
- open_questions: unresolved items.

## When to use
- A task spans multiple specialized agents.
- A long task is split across sessions or context windows.
- Responsibility must transfer with a clear audit trail.

## Workflow
1. Sending agent summarizes state into the handoff payload.
2. Receiving agent confirms it understands goal and next_action.
3. Receiving agent proceeds and updates the shared state.
4. Repeat for each subsequent handoff.

## Tips
- Keep payloads concise but complete; omit irrelevant detail.
- Make next_action explicit and unambiguous.
- Preserve a handoff log so the chain can be reviewed.
