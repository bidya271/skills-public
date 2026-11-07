# Codebase Memory and Graph Engine

Continuous shared codebase memory and architectural graph for AI coding agents.

You can buy the full skill pack for the price of a coffee directly on the listing page.

## The Problem

AI coding agents suffer from catastrophic context amnesia.

Every time you open a new session in Cursor Claude Code or Codex the agent starts completely from zero. It has no memory of the architecture decisions made yesterday the subtle database bugs fixed last week or the custom naming conventions your team follows.

Developers waste hours re-explaining the same project rules. Even worse agents repeat old mistakes reintroduce resolved bugs and burn thousands of tokens blindly re-reading massive code files just to locate basic function definitions.

## The Solution

This skill provides a zero-dependency shared memory and structural graph layer for your coding agents.

It maintains a persistent lightweight memory bank directly inside your project repository. Before writing any code your agent reviews past technical discoveries and navigates an indexed architectural graph of symbols and dependencies instead of burning tokens on full file scans.

## How This Skill Solves It

* **Persistent Team Learnings:** Automatically captures non-obvious architecture constraints bug fixes and team conventions so agents never repeat past errors.
* **Structural Symbol Graph:** Generates a concise map of system entrypoints core interfaces and service call flows without relying on heavy external background daemons.
* **Pre-Task Recall Protocol:** Reads past project rules before touching any source files to ensure every code change adheres to established team patterns.
* **Token Budget Conservation:** Navigates pre-indexed relationship maps instead of burning context window tokens re-scanning large directories.
* **Multi-Agent Continuity:** Enables seamless handoffs between Claude Code Cursor and Codex because project learnings live in standard durable files.

## Quick Setup

Drop the skill folder directly into your agent skills directory:
```bash
~/.gemini/config/skills/codebase-memory-graph
```

Call `/recall-memory` to inspect active project rules or `/map-codebase` to generate a structural symbol map.

## License

MIT License.
