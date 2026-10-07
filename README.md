### Kevin Thakkar · I build and evaluate AI agents

I'm a product leader who builds. This is where the building happens.

> **No agent beats a bad agent.** A bad agent costs more than the work it replaces, because once people stop trusting it, they stop trusting the next one too. That's why I write the evals before I ship.

### What I'm interested in right now

- **Agents that take action inside real workflows.** The interesting work starts when an agent has to decide something and live with the result.
- **Agents in advertising.** Ad platforms are full of decisions an agent could make: which audience to target, which landing page test to run next, when to shift budget. I spent 13 years on those decisions by hand.
- **Agents for personal finance.** Agents that track spending, optimize savings and support investment decisions, with a human approving anything that moves money.
- **Evals as the product spec.** If I can't say what a good output looks like and measure it, I'm not ready to ship.
- **Small agents for my own life.** Each one removes a chore I'd otherwise do every week.

### What I like to build

Tools for problems I hit every week, then hardened like production software: scheduled runs, alerts when something fails, and evals before I trust the output.

| Project | Why I built it |
|---|---|
| [Daily Digest](https://github.com/kthakkar81/daily-digest) | Too many newsletters, too little time. An agent reads them each morning, sorts them by topic with the Claude API and sends me the few items worth reading. |
| [Tastytrade Logger](https://github.com/kthakkar81/tastytrade-logger) | I wanted every options trade journaled without typing it in. It classifies strategies, links rolls and calculates P&L on a schedule. A run that finishes without reporting in counts as a failure. |
| [Kids Rewards App](https://github.com/kthakkar81/kids-rewards-app) · [prototype](https://kthakkar81.github.io/kids-rewards-app/) | A problem from home: replacing nagging with a points loop my kids respond to. I wrote the PRD and wireframes before any code, and the README lists the known gaps. |

### How I evaluate agents

1. **Read real outputs first.** Before writing any metric, I look through a sample of actual traces and note what goes wrong.
2. **Turn failures into a taxonomy.** I group what I find and fix the most common failure first.
3. **Use code checks where I can and an LLM judge where I must.** Anything deterministic gets a code check. Judgment calls get an LLM judge, calibrated against my own labels before I trust it.
4. **Keep a golden dataset.** Every change runs against it, so a fix in one place can't quietly break another.
5. **Watch it in production.** Failed or silent runs alert me.

Tools: Braintrust, Inspect AI, Langfuse, Claude API, Claude Code, Cursor.

[kevinthakkar.com](https://kevinthakkar.com) · [LinkedIn](https://linkedin.com/in/kevin-thakkar-135508)
