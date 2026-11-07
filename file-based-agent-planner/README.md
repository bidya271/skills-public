# File Based Agent Planner

Architected by Bidya. Stop AI agents from losing context and getting trapped in repetitive error loops during complex long running tasks.

You can buy the full skill pack for the price of a coffee directly on the listing page.

## The Problem

Most AI agents fail when a task requires more than five tool calls.

They lose context window memory repeat the same failed bash commands forget original project boundaries and hallucinate completion. Long research tasks multi file refactors and deep migrations collapse because agents depend entirely on ephemeral chat memory.

When an agent hits token limits or restarts all accumulated context vanishes.

## The Solution

I designed this skill to force AI agents to maintain durable external disk memory throughout execution.

Instead of keeping state inside an ephemeral chat context the agent maintains three living markdown files directly in your repository: `task_plan.md` `findings.md` and `progress.md`. Before and after every tool invocation the agent reads and updates this external brain.

## How This Skill Solves It

* **Durable Task Plans:** Creates structured step by step milestones with explicit acceptance criteria before any code is modified.
* **Continuous Findings Logging:** Appends discovered API responses architectural quirks and technical facts to `findings.md` so discoveries survive context compaction.
* **Self Healing Error Loops:** Automatically logs failed attempts and updates the tactical plan rather than repeating the same failed command.
* **Restart Resilience:** Enables agents to resume long running jobs across multiple sessions simply by reading file state on startup.

## Quick Setup

Drop the skill folder directly into your agent skills directory:
```bash
~/.gemini/config/skills/file-based-agent-planner
```

## License

MIT License. Authored by Bidya.
