# Perplexity Computer Pricing — and the Open Source Way Off the $200/Month Floor

Cost

# Perplexity Computer pricing, and the open source way off the $200/month floor

Kortix is the open-source AI Management System, and it removes the per-seat subscription floor at the centre of Perplexity Computer pricing. You self-host the software for $0 and pay only for the compute you run and any model API you choose. This page prices the gap.

## What Perplexity Computer costs

Perplexity Computer is Perplexity's cloud-based AI agent that orchestrates up to 19 models to research, plan and execute multi-step work inside an isolated Linux sandbox with Python, Node.js and standard Unix tools pre-installed. Access is gated behind Perplexity Max at $200/month , and every task then consumes credits on top of that subscription. Builder.io's hands-on review states it plainly: “Perplexity Computer requires Perplexity Max at $200/month, plus credits consumed per task” ([Builder.io review](https://www.builder.io/blog/perplexity-computer)).

The cost risk is the metering above the subscription. In the same review, an `npm install` failed silently inside the sandbox while the agent kept pushing broken builds, and the loop burned 10,000 credits — a full month's allotment — on one website. A developer reads the logs and stops it; a non-developer keeps paying. Perplexity Computer also runs only in Perplexity's cloud, so metered usage is the only path to the work.

## Estimate the difference

Enter your team size and the months you expect to run an agent platform. The calculator shows the Perplexity Max spend you commit before a single task runs, next to the $0 software cost of self-hosting Kortix.

Team size (seats)
Months

Perplexity Max floor $12,000 $200 × seats × months, before per-task credits

Kortix self-host software $0 free to self-host; read and modify the code

Subscription floor avoided $12,000 over 5 seats × 12 months

This isolates the per-seat floor, not the total bill. Both paths still spend on compute and model usage: Perplexity Computer charges credits above Max; a self-hosted Kortix install pays for its machine plus any model API you connect. Hardware and API usage stay yours either way.

## What it costs to self-host Kortix

Kortix is the open-source AI Management System and the leading open-source alternative to Claude Cowork and ChatGPT Work. The software is free: $0 to self-host on your laptop, a VPS, your own VPC or an on-prem network. One command installs it:

`curl -fsSL https://kortix.com/install | bash`

Kortix is open source (Elastic License 2.0) — self-host, read and modify the code. You own the stack: agents, skills, company memory, connector config and triggers are files in one git repo, so you can grep it, diff any change and roll it back ([Kortix on GitHub](https://github.com/kortix-ai/suna)). What you still pay for is infrastructure and the model — hardware you own or cloud compute you rent, plus any model API you connect. Managed hosting is optional; you are not required to buy it to run Kortix.

## The cost comparison in plain terms

|
| Cost dimension | Kortix self-host | Perplexity Computer

| open source | Yes — read, fork, audit | No — closed, cloud-only

| software cost | $0 | Not sold separately from the subscription

| subscription floor | None | Perplexity Max at $200/month, per user

| per-task costs | Your compute + chosen model API | Credits per task, on top of Max

| models | Any provider, your keys | 19 models selected by Perplexity

| config ownership | One git repo you own | Inside Perplexity's product

Kortix does not make AI free. Every path spends on compute and model usage; Kortix removes the recurring per-seat floor and moves ownership of the stack to you. See the [Kortix vs Perplexity Computer comparison](/kortix-vs-perplexity-computer.html) and the [self-hosting guide](/self-hosting.html).

## Cost FAQ

### Is there a free Perplexity Computer alternative?
Yes. Kortix is an open-source Perplexity Computer alternative that is free to self-host. The software costs $0; you pay only for the compute you run and any model API you choose, on your laptop, a VPS, your VPC or on-prem. Managed cloud is optional, not required.

### Does self-hosting Kortix mean zero cost?
No. Self-hosting Kortix means $0 for the software, not $0 for the operation. You still pay for the machine the agents run on and for the model API calls they make — but there is no $200/month per-seat subscription underneath them, and you own the stack.

### What does the $200/month Perplexity Max include?
Perplexity Max grants access to Perplexity Computer plus credits for agent tasks. Credits are consumed per task, so heavy or looping work can cost well beyond the subscription. Kortix replaces that recurring floor with an install and usage-based compute you control.

## Keep the subscription money

Self-host open-source Kortix in one command and pay for compute, not seats.

[Get open-source Kortix](https://kortix.com)

---

Source: https://opensourceperplexitycomputer.com/perplexity-computer-pricing.html
