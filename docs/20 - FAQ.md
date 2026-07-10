---
layout: default
---

<nav class="doc-home-link"><a href="{{ '/docs/' | relative_url }}">&larr; Go back Home</a></nav>

# FAQ

## Is Likha attended or unattended?

Both. Use the desktop designer for attended building and testing. Use robot service, user agent, schedules, and triggers for unattended execution.

## Why does UI automation need a user session?

Desktop, browser, mouse, keyboard, monitor, and message box actions need an interactive Windows session. On robot VMs, `LikhaUserAgent` must run inside the logged-in robot account.

## Where are flows and runtime data stored?

Local MVP data is stored in SQLite under `data/`.

## How do I run a flow on a schedule?

Create a schedule in Control Room Scheduler. Scheduled runs are unattended jobs.

## How do I process many work items?

Use Queue Management with `Queue > Add Item`, `Queue > Get Next Item`, and `Queue > Update Item`.

See:

[Queue Management.md](Activities/Files%20Queues%20API%20and%20Scripting/Queue%20Management.html)

## How do I connect AI?

Configure Control Room AI Settings, then use AI activities such as AI Prompt.

See:

[AI Prompt.md](Activities/AI%20Capabilities/AI%20Prompt.html)

## Why did Excel blanks appear as None before?

Excel libraries report empty cells as `None`. Likha normalizes Read Range blanks to empty text and removes fully empty rows/trailing columns for cleaner DataTables.

## What should I use for browser selectors?

Prefer stable attributes such as `name`, `data-testid`, `aria-label`, or `placeholder`. Use ID only when it is stable.

## Where do I configure event triggers?

Open:

```text
Control Room > Robots > Event triggers
```

See:

[Event Triggers.md](Activities/Event%20Triggers/Event%20Triggers.html)

