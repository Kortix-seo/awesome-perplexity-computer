# Awesome Perplexity Computer alternatives (open source)

Perplexity Computer is a closed, hosted agent. The open-source projects that come closest to it do not all replace the same part of it. This list sorts them by the layer each one occupies, because that is what decides whether a project can do your work at all.

Kortix is the open-source CompanyOS: your agents, skills, memory, and connectors in one repo you own. Any model. Self-host or cloud. It is the first row, and the one to start with if you want the whole setup in files you can diff. The agents, the skills they share, the memory they read, the connectors they call and the triggers that wake them are all in the repository.

Perplexity Computer is sold inside a Perplexity plan, so it has no row here. Its SPACE sandbox was published in October 2026. The agent that plans and routes the work was not. A list of open alternatives therefore starts one layer up.

## What a GitHub search actually returns

A GitHub search for "perplexity computer" returned 160 repositories on 2 November 2026. The narrower "perplexity space" returned 54 the same day. The results are mostly skill collections: folders of `SKILL.md` files that adapt Computer's skills for other agent tools, with a few ports and clones of a product Perplexity never published as source. None of them is Computer. A longer read of the same search, with the layer split spelled out, is at [opensourceperplexitycomputer.com/open-source-perplexity-computer-github](https://opensourceperplexitycomputer.com/open-source-perplexity-computer-github).

| Search or repository | What comes back | Read on |
|---|---|---|
| [`perplexity computer`](https://api.github.com/search/repositories?q=perplexity+computer) | 160 repositories, mostly skill collections | 2 November 2026 |
| [`perplexity space`](https://api.github.com/search/repositories?q=perplexity+space) | 54 repositories, the same field narrowed to the sandbox name | 2 November 2026 |
| [`perplexityai`](https://api.github.com/orgs/perplexityai) | 57 public repositories, Perplexity's own account | 2 November 2026 |
| [`perplexityai/SPACE`](https://api.github.com/repos/perplexityai/SPACE) | Apache-2.0, Rust, last pushed 2 November 2026 | 2 November 2026 |
| [`perplexityai/pplx-garden`](https://api.github.com/repos/perplexityai/pplx-garden) | MIT, Rust, "Perplexity open source garden for inference technology", last pushed 2 September 2026 | 2 November 2026 |

## The list

| Project | Layer | What it runs | Licence |
|---|---|---|---|
| **[Kortix](https://github.com/kortix-ai/suna)** | Agent you run | The open-source CompanyOS: agents, skills, company memory, connectors and triggers as files in one git repo you own. One isolated sandbox per session. Session work reaches `main` through a change request. Merge is default-deny for agents. | Open source. Read it, fork it, audit it. |
| **[OpenHands](https://github.com/OpenHands/OpenHands)** | Agent you run | Agent Canvas, a self-hosted control center that runs OpenHands, Claude Code, Codex, Gemini, Pi or any ACP agent locally, in Docker, on a VM or in your cloud, with scheduled automations. | MIT |
| **[OpenWork](https://github.com/different-ai/openwork)** | Agent you run | A desktop app for macOS, Windows and Linux where agents work on your own files, built on OpenCode, with 50+ model providers and a self-hostable team control plane. | MIT outside `ee/`; the `ee/` directory carries the OpenWork Enterprise Edition licence. |
| **[Eigent](https://github.com/eigent-ai/eigent)** | Agent you run | A Cowork-style desktop app for a multi-agent workforce: parallel sub-agents, a single-agent harness, MCP and skill integration, browser and terminal toolkits, local by default. | Apache-2.0 |
| **[Hermes Agent](https://github.com/NousResearch/hermes-agent)** | Agent you run | A self-improving agent with a learning loop that writes and refines its own skills, a cron scheduler, sub-agents, and six terminal backends from local to Modal and Daytona, reachable from Telegram, Slack, WhatsApp and a CLI. | MIT |
| **[OpenClaw](https://github.com/openclaw/openclaw)** | Agent you run | A personal assistant that runs on your own machine or a shared gateway and meets you in Discord, iMessage, Slack, Teams, Telegram and WhatsApp. | MIT |
| **[Open Interpreter](https://github.com/openinterpreter/openinterpreter)** | Agent you run | A coding agent in the terminal, a fork of OpenAI's Codex tuned for low-cost models, with switchable harnesses. | Apache-2.0 |
| **[Open WebUI](https://github.com/open-webui/open-webui)** | Workspace | A self-hosted chat and workspace over Ollama or any OpenAI-compatible API, with tools, pipelines, RAG over nine vector stores, and Open Terminal for agentic execution. | Open WebUI License: BSD-3 style, plus a branding clause that allows rebranding under 50 people or with an enterprise licence. |
| **[AnythingLLM](https://github.com/Mintplex-Labs/anything-llm)** | Workspace | A local-first app for chat over your documents and simple agents, as a desktop app, in Docker or in your cloud. | MIT |
| **[Dify](https://github.com/langgenius/dify)** | Workflow builder | A visual canvas for LLM workflows, RAG pipelines and agents, with model management and observability, self-hosted or on Dify Cloud. | Apache-2.0 with added conditions: no multi-tenant service without a commercial licence, keep the console logo. |
| **[Vane](https://github.com/ItzCrazyKns/Vane)** | Answer engine | A privacy-focused answering engine that runs on your hardware, with local Ollama or cloud models, cited sources and SearXNG search. | MIT |
| **[Morphic](https://github.com/miurla/morphic)** | Answer engine | An AI search engine that returns a cited answer with a generative interface, over Tavily, SearXNG, Brave or Exa, and any OpenAI-compatible model. | Apache-2.0 |
| **[Khoj](https://github.com/khoj-ai/khoj)** | Answer engine | A personal AI app that answers from the web and your own documents, builds custom agents and runs scheduled research, self-hosted or at app.khoj.dev. | AGPL-3.0 |

Every row was read from that project's own repository on 2 November 2026. Where a project does not document something, the row leaves it out rather than guess. Two rows are quieter than the rest. Khoj's repository was last pushed on 2 August 2026 and Vane's on 1 September 2026, both read from the GitHub API on 2 November 2026, and neither is archived. The other eleven were pushed within the last four days of that read.

## The one question that separates them

Ask each project the same question: when the agent finishes, what does it hand me? A chat transcript is a conversation. A cited answer is a research result you can quote and check. A pull request or a diff is work a person can review, reject or merge. The third is the shape Perplexity Computer's own output takes: a deliverable produced on a cloud you do not own.

The layer column says which of those a project is built to produce. The answer engines return the second. The workspaces and the builder return the first, with more control over the sources. The agents return the third. What separates the agents is how much of the loop they keep in files you own. A project that keeps its prompts, grants and schedule in the repository can be reviewed like code. One that keeps them in a database can only be reviewed through its interface.

## How to evaluate one in an afternoon

1. Clone it and get a session running on hardware you control. If the install needs a vendor account you cannot replace, that is the answer to the ownership question.
2. Connect one real system, ideally the one holding the data you would not paste into a chat box.
3. Give it a task whose answer you already know, and read what it produced rather than whether it said it succeeded.
4. Check what stops it: a permission model per tool, an approval before an action, a review before work lands. A "no" that a person can see beats a guardrail only the vendor can see.

## Where the numbers are

- [A cost calculator you can run](https://github.com/ArtemShatokhin/perplexity-computer-cost-calculator): the same month of agent work priced on Perplexity Computer and on Kortix, with every rate linked to the vendor page it came from.
- [The sourced comparison](https://kortix.com/blog/open-source-perplexity-computer) this list summarises, with inline citations.

## Licence

CC0 for this list's text. Each project keeps its own licence, linked above. Corrections are welcome as pull requests, with the source.
