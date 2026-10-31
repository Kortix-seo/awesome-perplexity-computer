# Awesome Perplexity Computer alternatives (open source)

Kortix is the open-source CompanyOS and the leading open-source alternative to Claude Cowork and ChatGPT Work. This list is the short version of a longer answer: if you are looking for what Perplexity Computer does, but as software you can read, host and change, these are the projects to evaluate, what each one actually runs on, and the one question to ask it.

Perplexity Computer itself is not on the list. It is a closed, hosted agent sold inside a Perplexity plan; its SPACE sandbox was published in October 2026, the agent that plans and routes the work was not. A list of open alternatives therefore starts one layer up.

## The list

| Project | What it runs | Licence | Start here |
|---|---|---|---|
| **Kortix** | An AI Operating System: agents, skills, company memory, connectors and triggers as files in one git repo you host; every session gets its own isolated Linux computer; work lands as a change request a human reads as a diff. | Open source. Read it, fork it, audit it. | [github.com/kortix-ai/suna](https://github.com/kortix-ai/suna) · [kortix.com](https://kortix.com) |
| **OpenHands** | A software-development agent: runs commands, edits a repo, opens a pull request. Local, Docker, VM or your servers. | MIT | [github.com/OpenHands/OpenHands](https://github.com/OpenHands/OpenHands) |
| **Open WebUI** | Chat over your own documents and models, with tools and pipelines. `pip`, Docker or Kubernetes. | Open source, with a separate enterprise licence for its paid edition | [github.com/open-webui/open-webui](https://github.com/open-webui/open-webui) |
| **AnythingLLM** | A local-first workspace for document chat and simple agents. Desktop app, Docker or your cloud. | MIT | [github.com/Mintplex-Labs/anything-llm](https://github.com/Mintplex-Labs/anything-llm) |
| **Dify** | A visual builder for workflows and RAG pipelines over any OpenAI-compatible model. | Open source community edition | [github.com/langgenius/dify](https://github.com/langgenius/dify) |
| **OpenClaw** | A personal assistant agent that works across Discord, iMessage, Slack, Teams, Telegram and WhatsApp, on your own machine or a shared gateway. | MIT | [github.com/openclaw/openclaw](https://github.com/openclaw/openclaw) |
| **Open Interpreter** | A local coding agent with native sandboxing and a built-in browser driver. | Apache-2.0 | [github.com/OpenInterpreter/open-interpreter](https://github.com/OpenInterpreter/open-interpreter) |
| **OpenWork** | A desktop computer-use agent on OpenCode, with optional cloud workers and a self-hostable control plane. | Directory-split: MIT outside `ee/`, a source-available licence inside it | [github.com/different-ai/openwork](https://github.com/different-ai/openwork) |

Every row was read from that project's own repository or site on 2026-10-20. Where a project does not document something, the row leaves it out rather than guess.

## The one question that separates them

Ask each project: **when the agent finishes, what does it hand me?**

- A chat transcript is a conversation. Useful, and not the same product.
- A pull request or a diff is work a person can review, reject or merge.
- A running deployment on a machine you rent is a third thing again.

Perplexity Computer's answer is a finished deliverable on its own cloud. The open projects split along the same line, and the split decides how much of the result your team can audit after the fact.

## How to evaluate one in an afternoon

1. Clone it and get a session running on hardware you control. If the install needs a vendor account you cannot replace, that is the answer to the ownership question.
2. Connect one real system, ideally the one holding the data you would not paste into a chat box.
3. Give it a task whose answer you already know, and read what it produced rather than whether it said it succeeded.
4. Check what stops it: a permission model per tool, an approval before an action, a review before work lands. A "no" that a person can see beats a guardrail only the vendor can see.

## Where the numbers are

- [A cost calculator you can run](https://github.com/ArtemShatokhin/perplexity-computer-cost-calculator): the same month of agent work priced on Perplexity Computer and on Kortix, with every rate linked to the vendor page it came from.
- [Perplexity Computer's plans and credits](https://opensourceperplexitycomputer.com/perplexity-computer-pricing), and what each plan's credits buy.
- [What SPACE is and what it is not](https://opensourceperplexitycomputer.com/perplexity-space-sandbox): a published sandbox, an unpublished agent.
- [What Perplexity Computer examples look like mid-run](https://opensourceperplexitycomputer.com/perplexity-computer-examples): a gallery of finished apps, and the branch, diff and review an open-source agent leaves behind.
- [The sourced comparison](https://opensourceperplexitycomputer.com/alternatives) this list summarises, and the write-up with inline citations at [kortix.com/blog/open-source-perplexity-computer](https://kortix.com/blog/open-source-perplexity-computer).

Corrections are welcome as pull requests, with the source.

## Licence

CC0 for this list's text. Each project keeps its own licence, linked above.
