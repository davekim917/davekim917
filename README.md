# Dave Kim

I build and run a fleet of AI agents that does most of my engineering. Each agent lives in its own container, takes work from Slack or Discord, and ships through a plan, build, review and ship workflow I wrote for it. The first two repos below are that system. My background is data engineering, and my consulting work builds data foundations for production AI.

## What I'm building

[**anderton-agent**](https://github.com/davekim917/anderton-agent) is the fleet itself, built on NanoClaw. Every agent has its own identity, instructions, tools and secrets, and one person runs many of them at once. It adds workgroups that share a chat archive and durable memory, read access across workgroups granted by host policy, MCP servers added to every agent with one command, OAuth for remote MCP servers, a secret-intake form so API keys never pass through chat, and fallback across Claude, Codex and OpenCode when one provider stops answering.

[**bootstrap**](https://github.com/davekim917/bootstrap) is the delivery workflow those agents use, packaged as plugins for Claude Code, Codex and OpenCode: `/team-plan → /team-build → /team-review → /team-ship`. Process scales with risk. A four-file mechanical change stays small, while a one-file credential change or destructive migration still gets security, rollback and verification review. It also ships advisory skills for engineering judgment, a verification loop for analytics claims, and a test-authoring gate.

[**design-artifact-loop**](https://github.com/davekim917/design-artifact-loop) is a Claude Code and Codex plugin that turns a design brief into a reviewed single-file HTML mockup. It commits to a design system before writing markup, renders at desktop and mobile sizes, runs deterministic checks, and has a separate vision model critique the pixels.

## Elsewhere

[LinkedIn](https://www.linkedin.com/in/davidkim6/)
