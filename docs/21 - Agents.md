---
layout: default
---

<nav class="doc-home-link"><a href="https://burnimjerome.github.io/LIKHA-_-BETA/">&larr; Go back Home</a></nav>

# Agents

Likha Agents add an agentic AI layer to the platform. Instead of only running a fixed sequence of activities, an agent can receive a goal, use available context, choose an appropriate tool or workflow, inspect the result, and continue until it reaches a defined outcome or needs human input.

RPA and agents work together:

- The agent reasons about the goal and decides what should happen next.
- Likha flows provide reliable, reusable tools for desktop, browser, Excel, file, API, queue, and system work.
- AI Screen Control lets the agent understand and operate visible applications when a stable selector or API is unavailable.
- Control Room provides execution records, queues, robot capacity, schedules, and operational visibility.

## What an Agent Can Do

A Likha Agent can be configured to:

- Accept a natural-language objective and supporting instructions.
- Use approved Likha flows and activities as tools.
- Read screen, document, queue, file, API, and workflow context.
- Select the next action based on the current result.
- Pass structured outputs from one tool to the next.
- Retry or choose an alternate approved path when an action fails.
- Ask for human review when confidence is low or approval is required.
- Return a final result together with its execution history.

## Agent Execution Cycle

```text
Goal
  -> understand context
  -> plan or select the next approved tool
  -> execute through the Likha runtime
  -> observe the output and screen state
  -> continue, finish, or request human input
```

An agent is bounded by its instructions, enabled tools, credentials, limits, and approval rules. It does not automatically gain access to every flow or machine.

## Building Agent-Ready Flows

Flows used as agent tools should have:

- A clear name and a single, understandable purpose.
- Typed inputs and structured outputs.
- Predictable error handling and useful failure messages.
- Explicit timeout and retry behavior.
- No hard-coded credentials or sensitive values.
- A defined boundary for actions that require human approval.

## Example

Goal: `Review the next invoice and enter valid details into the finance application.`

The agent can:

1. Get the next queue item.
2. Extract invoice fields with an AI document activity.
3. Validate and normalize the extracted values.
4. Open the finance application.
5. Use AI Screen Control to locate the form and enter the approved values.
6. Verify the confirmation screen.
7. Update the queue item and return the result.

The document extraction and screen understanding are adaptive, while the queue update, validation, and submission rules remain deterministic and auditable.

## Related Documentation

- [Agent Infrastructure](22%20-%20Agent%20Infrastructure.html)
- [Architecture](04%20-%20Architecture.html)
- [AI Integration](10%20-%20AI%20Integration.html)
- [AI Screen Control](Activities/AI%20Screen%20Control/README.html)
- [Orchestrator](17%20-%20Orchestrator.html)

