# Automated Changelog Generator

Architected by Bidya. Automate customer ready release notes and changelogs directly from git history and pull requests with zero manual editing.

You can buy the full skill pack for the price of a coffee directly on the listing page.

## The Problem

Writing production release notes is a chore that developers consistently rush through or ignore.

Teams ship critical updates but summarize them with unhelpful one liners like bug fixes and performance improvements. Customers and internal stakeholders have no idea what broke what changed or what features were added.

Manually combing through dozens of merged pull requests and git commit hashes before each release burns hours of engineering time that should go toward building product.

## The Solution

I designed this skill to turn your raw git commits into clean professional changelogs automatically.

It extracts merged pull request metadata strips out developer noise categorizes changes into Added Changed Fixed and Security sections and formats everything into crisp customer facing documentation.

## How This Skill Solves It

* **Automated Git Parsing:** Scans commit histories and pull request bodies to pull out meaningful user facing changes.
* **Semantic Release Categorization:** Automatically buckets updates into clear sections following industry standard versioning conventions.
* **Breaking Change Alerts:** Prominently highlights breaking API changes along with required migration steps.
* **Semantic Version Recommendation:** Suggests patch minor or major version increments based on the severity of merged changes.

## Quick Setup

Drop the skill folder directly into your agent skills directory:
```bash
~/.gemini/config/skills/automated-changelog-generator
```

## License

MIT License. Authored by Bidya.
