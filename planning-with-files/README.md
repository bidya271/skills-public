# Planning With Files

Autonomous Manus-style file-based state and execution planning for complex agent tasks and multi-hour research workflows.

You can buy the full skill pack for the price of a coffee directly on the listing page.

## The Problem

AI agents fail when tasks require more than five sequential tool calls.

They lose context window memory repeat already attempted shell commands forget original constraints and hallucinate progress. Long research tasks multi-file code refactors and complex migrations quickly drift off course and burn tokens without finishing.

## The Solution

Planning With Files forces your agent to maintain an external durable disk memory.

It implements Manus-style planning protocols where the agent maintains three living markdown files on disk: `task_plan.md` `findings.md` and `progress.md`. Before and after every tool invocation the agent checks and updates this external brain.

## How This Skill Solves It

* **Durable Task Plans:** Creates structured step-by-step milestones with explicit success criteria before executing code.
* **Continuous Findings Logging:** Appends discovered facts API responses and edge cases to `findings.md` so context is never lost.
* **Self-Healing Error Loops:** Automatically logs failed commands and updates strategy rather than getting stuck in repetitive error loops.
* **Resilient Context Compaction:** Survives agent restarts and memory truncations by reading file state upon initialization.

## Quick Setup

Drop the skill folder directly into your agent skills directory:
```bash
~/.gemini/config/skills/planning-with-files
```

## License

MIT License.
