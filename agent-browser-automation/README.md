# Agent Browser Automation

Chrome and Chromium CDP browser automation framework enabling AI agents to navigate inspect fill forms and test live web applications.

You can buy the full skill pack for the price of a coffee directly on the listing page.

## The Problem

Most AI agents cannot see or touch the real web.

They rely on static web scrapers that fail on JavaScript heavy SPAs dynamic client rendered dashboards complex multi step forms and authenticated user sessions.

Traditional scraping scripts are brittle requiring hundreds of lines of boilerplate code that break the moment a CSS class or DOM node changes.

## The Solution

I designed this skill to give your agent native intelligent eyes and hands on the browser via Chrome DevTools Protocol.

It exposes an agent optimized interface that allows agents to open pages generate interactive element snapshots with short reference tags like `@e1` and `@e2` fill inputs click buttons take screenshots and extract rendered DOM data in real time.

## How This Skill Solves It

* **Interactive Snapshot Protocol:** Automatically labels interactive DOM elements with compact reference IDs so agents never guess CSS selectors.
* **Full JavaScript Execution:** Works seamlessly across modern dynamic web applications with client side hydration.
* **Form & Authentication Flows:** Automates multi step logins modal dialogs select dropdowns and file uploads.
* **Visual Verification:** Captures viewport screenshots to enable vision model verification and automated regression testing.

## Quick Setup

Drop the skill folder directly into your agent skills directory:
```bash
~/.gemini/config/skills/agent-browser-automation
```

## License

MIT License.
