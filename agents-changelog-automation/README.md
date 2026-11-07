# Changelog Automation

Automate production release notes and changelogs from commits and pull requests following Keep a Changelog and Conventional Commits standards.

You can buy the full skill pack for the price of a coffee directly on the listing page.

## The Problem

Writing release notes is tedious and consistently neglected.

Engineers rush through deployment and write lazy unhelpful release summaries like "bug fixes and improvements". Users and customers have no idea what broke what changed or what new capabilities were added.

Manually combing through dozens of merged pull requests and git commits before a release takes hours of developer time that could be spent shipping features.

## The Solution

This skill automates the extraction categorization and drafting of release notes directly from your codebase history.

It parses Conventional Commits filters out noise categorizes changes into Added Changed Deprecated Removed Fixed and Security sections and outputs clean customer-facing markdown.

## How This Skill Solves It

* **Automated Git Parsing:** Scans commit histories and PR metadata to extract meaningful change descriptions.
* **Keep a Changelog Standardization:** Automatically categorizes updates into standard semantic versioning sections.
* **Breaking Change Alerts:** Highlights breaking API changes and migration instructions prominently.
* **Semantic Version Bumping:** Recommends patch minor or major version increments based on change severity.

## Quick Setup

Drop the skill folder directly into your agent skills directory:
```bash
~/.gemini/config/skills/agents-changelog-automation
```

## License

MIT License.
