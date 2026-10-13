# Dave Kim

I build data foundations for production AI: the governed warehouse underneath, and the agent systems that run on top of it. Most of my own engineering now runs through a fleet of AI agents I operate from Slack and Discord, and the tooling below came out of running that fleet every day.

## What I'm building

[**anderton-agent**](https://github.com/davekim917/anderton-agent) is my personal agent fleet, built on NanoClaw. Each agent runs in its own container with its own identity, tools and secrets. It adds workgroups with shared memory, cross-workgroup read policy, fleet-wide MCP servers, a secret-intake form so keys never pass through chat, and fallback across Claude, Codex and OpenCode.

[**bootstrap**](https://github.com/davekim917/bootstrap) is a delivery workflow for Claude Code, Codex and OpenCode (`/team-plan → /team-build → /team-review → /team-ship`). Process scales with risk: a small mechanical change stays small, while a one-file credential change still gets security, rollback and verification review.

[**design-artifact-loop**](https://github.com/davekim917/design-artifact-loop) is a Claude Code and Codex plugin that turns a design brief into a reviewed single-file HTML mockup. It commits to a design system before writing markup, renders at desktop and mobile sizes, runs deterministic checks, and has a separate vision model critique the pixels.

## Elsewhere

[LinkedIn](https://www.linkedin.com/in/davidkim6/)
