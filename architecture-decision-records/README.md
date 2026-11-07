# Architecture Decision Records (ADR)

Architected by Bidya. Capture evaluate and maintain system architecture decisions and trade-offs with production grade documentation hygiene.

You can buy the full skill pack for the price of a coffee directly on the listing page.

## The Problem

Engineering teams suffer from catastrophic architectural amnesia.

Six months after shipping nobody remembers why a specific database queue architecture or authentication model was chosen. New engineers join and question decisions without knowing the constraints that forced them.

Decisions get buried in Slack threads or lost Google Docs. Teams end up revisiting the same technical debates repeatedly wasting engineering cycles and introducing system regressions.

## The Solution

I designed this skill to standardize how engineering teams capture debate and record system architecture decisions.

It enforces a structured decision record format guiding teams through context mapping alternative evaluation trade-off scoring and downstream consequence analysis before code is written.

## How This Skill Solves It

* **Standardized Decision Structure:** Formats decisions into Status Context Decision and Consequences blocks.
* **Trade-off Analysis:** Rigorously documents rejected alternatives and the exact reasons they were passed over.
* **Impact Mapping:** Tracks architectural consequences across security performance cost and developer ergonomics.
* **Onboarding Alignment:** Creates a living history of system evolution that accelerates new engineer ramp up.

## Quick Setup

Drop the skill folder directly into your agent skills directory:
```bash
~/.gemini/config/skills/architecture-decision-records
```

## License

MIT License. Authored by Bidya.
