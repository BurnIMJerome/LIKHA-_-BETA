---
layout: default
---

<nav class="doc-home-link"><a href="https://burnimjerome.github.io/LIKHA-_-BETA/">&larr; Go back Home</a></nav>

# Agent Infrastructure

Agent Infrastructure is the set of Likha services that lets agents use AI and automation tools safely across local workstations, robot machines, and private VM environments.

## Infrastructure Layers

```text
User or business event
  -> Likha Agent (goal, context, planning, tool selection)
  -> Control Room (policies, flows, queues, jobs, logs, AI settings)
  -> Workflow engine (validated activity execution)
  -> Robot service and user agent (machine and Windows-session execution)
  -> Desktop apps, browsers, Excel, files, APIs, and enterprise systems
```

## Core Components

- **Agent runtime:** interprets the objective, manages the current task context, selects enabled tools, and evaluates results.
- **Tool and flow registry:** exposes approved Likha flows and activities that an agent is allowed to call.
- **Control Room:** manages flows, schedules, queues, robot jobs, global variables, logs, AI settings, and licensing.
- **Workflow engine:** executes deterministic activities and returns structured outputs to the agent.
- **Robot service:** receives and supervises unattended work on a robot machine.
- **Likha User Agent:** performs browser, desktop, mouse, keyboard, monitor, message, and AI Screen Control work inside the active Windows user session.
- **AI provider connection:** supplies the configured model through the Bring Your Own Key settings.
- **Operational records:** preserve job state, logs, outputs, errors, and queue status for monitoring and audit.

## Deployment Models

### Local

The agent, designer, workflow engine, and data run on one Windows workstation. This is suitable for building, testing, and attended agent-assisted work.

### Private Robot VM

Control Room assigns work to one or more Windows robot VMs. Each UI-capable robot needs an active session with Likha User Agent running.

### Distributed

A central Control Room coordinates agents, queues, schedules, flows, logs, and robot jobs while separate machines perform the actual automation. This keeps planning and governance separate from execution capacity.

## Guardrails

Production agent deployments should define:

- Which flows and activities each agent may use.
- Which machines, applications, files, queues, and APIs are in scope.
- Credential and secret access.
- Maximum steps, retries, runtime, and AI usage.
- Human approval points for sensitive or irreversible actions.
- Logging, retention, and redaction requirements.
- A safe stop and escalation path when the goal cannot be completed.

## Reliability Model

Likha combines adaptive AI decisions with deterministic automation boundaries. Use agent reasoning where the input or screen can vary; use validated activities and flows for actions that must be repeatable. Use verification steps after important UI or data changes, and prefer structured outputs over free-form text between tools.

## Related Documentation

- [Agents](21%20-%20Agents.html)
- [Distributed Control Room and VM Robot Setup](Distributed%20Control%20Room%20and%20VM%20Robot%20Setup.html)
- [Robot Service and User Agent](Robot%20Service%20and%20User%20Agent.html)
- [Orchestrator](17%20-%20Orchestrator.html)
- [AI Integration](10%20-%20AI%20Integration.html)

