# Hey, I'm Soham 👋

MS Computer Science @ UC Santa Cruz — building at the intersection of AI agents, enterprise infrastructure, and developer tooling. Previously interned twice at HPE/Juniper Networks, where I built AI agent systems and CI/CD automation for production engineering teams.

---

## Currently Building

### [OpenClaw Gateway](https://github.com/sohamrajadh/openclaw-gateway) — Enterprise security proxy for AI agents
AI agents have unrestricted access to tools, file systems, and APIs with zero governance — which is why enterprises won't touch them. OpenClaw Gateway is an open-source MCP (Model Context Protocol) security proxy that sits between your LLM and its tools, enforcing enterprise-grade controls without changing a line of agent code.

- **Audit logging** — every agent action captured to PostgreSQL with full context, parameters, and results
- **Multi-layer guardrails** — regex pattern matching for known-dangerous commands (rm -rf, fork bombs, disk wipes) + LLM-based semantic analysis for novel threats
- **Human-in-the-loop approval** — high-risk actions paused and routed to a human reviewer via Slack, email, or webhook before execution
- Built with: `Python` `FastAPI` `PostgreSQL` `LangGraph` `Docker`

### [OpenGrove](https://github.com/sohamrajadh/opengrove) — Local-first AI conversation manager
A privacy-focused alternative to cloud AI chat interfaces. Bring your own API keys, keep your data local, and get features that hosted tools don't offer.

- Multi-provider support: OpenAI, Anthropic, Google, Ollama — switch mid-conversation
- Conversation branching with a subchat system for non-linear exploration
- Multi-agent discussion mode: query models in parallel, orchestrate cross-model debates
- RAG-powered semantic search across your full conversation history
- PII redaction pipeline using local models to sanitize prompts before any cloud API call
- Built with: `Python` `SQLite` `React` `FastAPI`

---

