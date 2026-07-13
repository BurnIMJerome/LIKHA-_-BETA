---
layout: default
---

<nav class="doc-home-link"><a href="https://burnimjerome.github.io/LIKHA-_-BETA/">&larr; Go back Home</a></nav>

# Product Overview

Likha is a Windows-first agentic AI and RPA automation platform for building, running, and monitoring intelligent agents and deterministic workflows.

It combines AI reasoning with a low-code Process Designer, reusable automation flows, AI Screen Control, Control Room, and robot runtimes. Teams can use traditional RPA for predictable steps and agents for work that requires context, tool selection, and adaptation.

It supports:

- Goal-driven agents that use approved Likha flows and activities as tools.
- Agent infrastructure for context, tool execution, robot capacity, queues, logs, and human approval boundaries.
- Desktop automation through Windows UI Automation, OCR/image fallback, and hardware input.
- Browser automation through Playwright-powered browser instances.
- Excel, files, data tables, queues, API calls, scripts, and flow control.
- AI activities using Control Room AI settings.
- AI Screen Control for understanding, extracting details from, and operating visible applications.
- Designer runs for interactive development.
- Unattended jobs through robot service and user agent components.
- Schedules, event triggers, robot jobs, logs, and queues.

## Main Applications

`desktop.py` starts the pywebview desktop shell.

`app/main.py` hosts the FastAPI Control Room and designer routes.

`app/engine.py` runs workflow activities.

`static/studio.html`, `static/studio.js`, and related CSS provide the process designer.

`data/` stores SQLite runtime data locally.

## Primary User Roles

- Builder: creates flows in Process Designer.
- Agent builder: defines an agent's purpose, instructions, tools, limits, and approval points.
- Operator: monitors runs, queues, schedules, and robot status in Control Room.
- Robot VM administrator: configures `LikhaRobotService`, `LikhaUserAgent`, and remote robot settings.

## Existing References

- [README.md](../README.html)
- [Agents](21%20-%20Agents.html)
- [Agent Infrastructure](22%20-%20Agent%20Infrastructure.html)
- [Robot Service and User Agent.md](Robot%20Service%20and%20User%20Agent.html)
- [Distributed Control Room and VM Robot Setup.md](Distributed%20Control%20Room%20and%20VM%20Robot%20Setup.html)
- [Event Triggers.md](Activities/Event%20Triggers/Event%20Triggers.html)

