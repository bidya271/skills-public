# Agent Browser Automation

Headless Chrome and Chromium CDP browser automation CLI for AI agents to navigate inspect fill forms and test live web applications.

You can buy the full skill pack for the price of a coffee directly on the listing page.

## The Problem

Most AI agents cannot see or touch the real web.

They rely on static web scrapers that fail on JavaScript-heavy SPAs dynamic client-rendered dashboards complex multi-step forms and authenticated user sessions.

Traditional Selenium or Puppeteer scripts are brittle requiring hundreds of lines of boilerplate code that break the moment a CSS class or DOM node changes.

## The Solution

Agent Browser gives your agent native intelligent eyes and hands on the browser via Chrome DevTools Protocol (CDP).

It exposes an agent-optimized command-line interface that allows agents to open pages generate interactive element snapshots with short reference tags (like `@e1` `@e2`) fill inputs click buttons take screenshots and extract rendered DOM data in real time.

## How This Skill Solves It

* **Interactive Snapshot Protocol:** Automatically labels interactive DOM elements with compact reference IDs so agents never guess CSS selectors.
* **Full JavaScript Execution:** Works seamlessly across modern React Next.js Vue and Angular applications with client-side hydration.
* **Form & Authentication Flows:** Automates multi-step logins modal dialogs select dropdowns and file uploads.
* **Visual Verification:** Captures viewport screenshots to enable vision model verification and automated regression testing.

## Quick Setup

Drop the skill folder directly into your agent skills directory:
```bash
~/.gemini/config/skills/vercel-agent-browser
```

## License

MIT License.
