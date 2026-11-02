# AI Agent Engineering Hub

A structured engineering curriculum and practical portfolio ecosystem dedicated to learning, building, testing, evaluating, and deploying AI Agents and Agentic Systems.

This repository serves as the central documentation directory, knowledge management hub, architectural guide, and progress tracker for 20 progressive projects spanning foundational LLM tool-calling to enterprise-grade multi-agent autonomous platforms.

---

## Professional Scope & Positioning

- **Engineering Discipline**: Software Engineer | Backend & DevOps
- **Specializations**: API Integrations, Workflow Automation, Systems Architecture, AI & Agentic Systems
- **Core Technology Stack**: Python, Pydantic, FastAPI, LangGraph, Redis, PostgreSQL, Docker, Kubernetes, OpenTelemetry

This curriculum is designed around engineering first principles: understanding model behavior, structuring deterministic tool contracts, managing state and context windows, evaluating agent reliability, and establishing security guardrails before deploying autonomous workflows.

---

## What are AI Agents and Agentic Systems?

An **AI Agent** is an autonomous or semi-autonomous software entity that perceives its environment, reasons over a goal using a language model, selects and executes tools, and iterates based on intermediate feedback until it fulfills a defined objective.

An **Agentic System** extends this capability to complex, multi-component architectures:
- **Perception & Ingestion**: Parsing structured and unstructured user inputs, webhooks, or system events.
- **Cognitive Loop (Reasoning & Planning)**: Decomposing complex goals into sequential or parallel subtasks using techniques like ReAct (Reason + Act) or state-machine DAGs.
- **Tool Orchestration**: Interacting with deterministic APIs, databases, command-line interfaces, and web search tools.
- **Memory Systems**: Maintaining short-term context across conversational turns and long-term semantic memory in vector and relational stores.
- **Reflection & Error Recovery**: Evaluating intermediate tool execution outputs, handling rate limits or API errors, and replanning dynamically.
- **Safety & Oversight**: Enforcing schema constraints, prompt injection defenses, and human-in-the-loop approvals for sensitive side effects.

---

## Repository Ecosystem Architecture

The curriculum is partitioned into four independent, progressive level repositories:

```
ai-agent-engineering-hub (Central Curriculum Hub & Architecture Guide)
|-- Level 1: ai-agents-beginner-projects (Projects 01-05)
|   |-- 01. Intelligent AI Chat Agent [Completed Reference]
|   |-- 02. Tool-Calling AI Agent
|   |-- 03. AI Research Assistant
|   |-- 04. Personal Productivity Agent
|   `-- 05. Document Q&A Agent
|
|-- Level 2: ai-agents-intermediate-projects (Projects 06-10)
|   |-- 06. Memory-Enabled Personal AI Agent
|   |-- 07. AI Email Management Agent
|   |-- 08. AI Coding Assistant Agent
|   |-- 09. RAG-Based Knowledge Base Agent
|   `-- 10. API Integration Agent
|
|-- Level 3: ai-agents-advanced-projects (Projects 11-15)
|   |-- 11. Autonomous Planning & Execution Agent
|   |-- 12. Multi-Agent Research System
|   |-- 13. Multi-Agent Software Development System
|   |-- 14. AI Data Analyst Agent
|   `-- 15. Agent Evaluation & Testing Platform
|
`-- Level 4: ai-agents-professional-projects (Projects 16-20)
    |-- 16. DevOps AI Operations Agent (AIOps)
    |-- 17. AI Customer Support Multi-Agent Platform
    |-- 18. AI Business Operations Agent Platform
    |-- 19. Autonomous Software Engineering Platform
    `-- 20. Enterprise Agentic AI Platform
```

---

## Level Repositories Index

| Tier | Repository | Focus Areas | Project Range |
| :--- | :--- | :--- | :--- |
| **Level 1: Beginner** | [**ai-agents-beginner-projects**](https://github.com/EmaanHumayun/ai-agents-beginner-projects) | System prompts, token tracking, function calling, tool schemas, SQLite persistence, basic RAG | Projects 01 - 05 |
| **Level 2: Intermediate** | [**ai-agents-intermediate-projects**](https://github.com/EmaanHumayun/ai-agents-intermediate-projects) | PostgreSQL/Redis memory, OAuth 2.0 email agents, code analysis, hybrid search RAG, API orchestration | Projects 06 - 10 |
| **Level 3: Advanced** | [**ai-agents-advanced-projects**](https://github.com/EmaanHumayun/ai-agents-advanced-projects) | State machine planning (LangGraph), multi-agent coordination, text-to-SQL, agent evaluation | Projects 11 - 15 |
| **Level 4: Professional** | [**ai-agents-professional-projects**](https://github.com/EmaanHumayun/ai-agents-professional-projects) | AIOps self-healing, customer support graphs, enterprise business ops, autonomous repo agents, enterprise gateway | Projects 16 - 20 |

---

## Learning Methodology

Every project follows an eight-stage engineering cycle:

```
Understand -> Explore -> Build -> Test -> Evaluate -> Document -> Deploy -> Explain
```

1. **Understand**: Review the problem statement, why an AI Agent is suitable, and architectural trade-offs.
2. **Explore**: Complete guided practical labs to inspect raw API calls, tool schemas, and token usage.
3. **Build**: Implement modular Python packages cleanly separating prompts, tools, memory, and services.
4. **Test**: Write automated unit tests for tools and integration tests for agent execution loops.
5. **Evaluate**: Measure response groundedness, tool-selection accuracy, token efficiency, and latency.
6. **Document**: Record system specifications, state machine transitions, and known failure modes.
7. **Deploy**: Package applications with Docker containers and environment configurations.
8. **Explain**: Articulate design decisions, limitations, and future architectural improvements.

---

## Navigation & Documentation Map

- [Roadmap](ROADMAP.md) - Comprehensive four-tier curriculum roadmap
- [Learning Path](LEARNING-PATH.md) - Systematic progression guide and prerequisites
- [Project Catalog](PROJECT-CATALOG.md) - Complete briefs, architectures, and deliverables for all 20 projects
- [Concept Mastery Index](CONCEPT-MASTERY-INDEX.md) - 50+ agentic concepts mapped across tiers
- [Technology Stack](TECHNOLOGY-STACK.md) - Runtimes, vector databases, frameworks, and tools
- [Architecture Guide](ARCHITECTURE-GUIDE.md) - Agent loops, state machines, memory architectures, and safety
- [Glossary](GLOSSARY.md) - Formal technical definitions of agentic and LLM terminology
- [Progress Dashboard](progress/overall-progress.md) - Authentic implementation progress across all 20 projects

---

## Security Policy & Credential Isolation

- **Zero Credential Persistence**: API keys, database credentials, and OAuth tokens must reside exclusively in local `.env` files (never committed).
- **Sanitized Templates**: Every project provides a clean `.env.example` with placeholder variables.
- **Untrusted Inputs**: Tool outputs, retrieved web pages, user uploads, and external emails are treated as untrusted and sanitized against prompt injection.
- **Least-Privilege Execution**: Tools execute with scoped, read-only permissions by default. Destructive actions require explicit human-in-the-loop confirmation.

---

## Author & Maintainer

- **Engineer**: Emaan Humayun
- **GitHub**: [@EmaanHumayun](https://github.com/EmaanHumayun)
- **Central Portfolio**: [engineering-portfolio](https://github.com/EmaanHumayun/engineering-portfolio)
