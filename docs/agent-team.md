# Project Pulse Agent Team

This team builds the Project Pulse dashboard. Each specialist is defined in `.github/agents/` and has a clear responsibility.

| Agent | Model | Definition | Responsibility |
| --- | --- | --- | --- |
| Orchestrator | Opus 5.5 | `.github/agents/orchestrator.agent.md` | Coordinates the team, delegates work, and owns the final handoff. |
| Planner | GPT-5.5 | `.github/agents/planner.agent.md` | Produces the Project Pulse implementation plan and file ownership. |
| Coder | Gemini 3.7 Flash | `.github/agents/coder.agent.md` | Implements the static dashboard files and launch configuration. |
| Designer | GPT-5.5 | `.github/agents/designer.agent.md` | Defines the dashboard layout, visual hierarchy, and card styling. |

The Orchestrator starts by asking the Planner for a phased plan. The Designer reviews the card and dashboard presentation before the Coder implements `app/index.html`, `app/styles.css`, `app/project-data.json`, and `.vscode/launch.json`. The team coordinates through Project Pulse context, validates the rendered fields, and records the final handoff.
