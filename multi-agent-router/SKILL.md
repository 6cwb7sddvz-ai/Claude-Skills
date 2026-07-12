---
name: multi-agent-router
description: Classify an incoming request and route it to the most suitable specialized agent.
---

# Multi-Agent: Router / Dispatcher

Use this pattern when different requests need different specialized agents.

## Roles
- Router: classifies the request and selects the target agent.
- Specialists: agents each optimized for a domain (coding, research, writing, etc.).

## When to use
- Requests fall into distinct categories with different handling.
- You want a cheap, fast classifier in front of expensive specialists.
- Routing logic should be centralized and easy to update.

## Workflow
1. Router receives the request and extracts intent and key features.
2. Match against a routing table or classifier.
3. Forward to the chosen specialist with the needed context.
4. Return the specialist's answer; fall back to a default if no match.

## Tips
- Keep categories mutually exclusive where possible.
- Log routing decisions for auditing and improvement.
- Provide a sensible default agent for unclassified requests.
