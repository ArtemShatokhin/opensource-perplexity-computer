# Self-Hosting an Open Source Perplexity Computer Alternative

How-to

# Self-hosting an open source Perplexity Computer alternative

Kortix is the self-hosted pick: install it on a laptop, a VPS, your VPC or on-prem, and every agent, skill, memory file and connector stays in one git repo you own. Here is what self-hosting actually takes, project by project, and where the hard parts are.

## What “self-host” buys you

Perplexity Computer runs entirely in Perplexity's cloud. Four things change when you move to a self-hosted agent: your data and credentials stay on hardware you control; you choose the models, including local ones; you can audit and modify the code; and there is no per-seat subscription floor. The cost is operational — you own uptime, upgrades and isolation. Kortix carries all four without giving up the system behind them.

- Pick the project. Own the whole company system → Kortix, the open-source AI Management System: agents, skills, memory, connectors and triggers in one git repo, a real agent harness powered by OpenCode, an isolated Linux machine per session, and every change landing as a change request a human reads as a diff. Personal agent on your own machine → OpenClaw (MIT). Multi-agent workstation → Eigent (Apache 2.0), Docker + FastAPI + PostgreSQL with 200+ MCP tools.

- Prepare a host. Anything that can run containers works: a laptop, a VPS or a private cloud. Kortix installs with one command (curl -fsSL https://kortix.com/install | bash) and runs on a laptop, VPC or on-prem; it expects a git-backed project and a host that can run Linux machines for the sandbox fleet. OpenClaw is happiest on a machine that is on when you want the assistant. Eigent expects a reachable server — Docker images and a database.

- Choose models. All three are model-agnostic: point them at a hosted API with your own keys or at a local model. Kortix sets the model per agent, per session or per message — Claude, OpenAI, Gemini or your own OpenAI-compatible endpoint. Model choice is the single biggest lever on both privacy and cost.

- Harden and review. Keep credentials out of the model's context — Kortix brokers connectors server-side, so keys never enter the session machine, and you set allow / ask / block per tool call. Gate consequential actions: Kortix lands work only through a change request a human reads as a diff. Treat inbound messages as untrusted input and approve channel pairings rather than auto-accepting them.

◆
Why Kortix is the self-hosted pick. A closed cloud agent gives you managed convenience and a $200/month floor, with no source to audit and no machine you own. Kortix gives you the code, the models and the machine: one repo for the whole system, an isolated Linux computer per session, credentials brokered server-side, and a human gate on every change. Kortix is open source (Elastic License 2.0) — self-host, read and modify the code. Start at [kortix.com](https://kortix.com).

Next: [price the difference](/perplexity-computer-pricing.html) · [Kortix vs Perplexity Computer](/kortix-vs-perplexity-computer.html) · [FAQ](/faq.html).

---

Source: https://opensourceperplexitycomputer.com/self-hosting.html
