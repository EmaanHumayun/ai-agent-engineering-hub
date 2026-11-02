# Master AI Agent Engineering Roadmap

A structured 4-tier learning and implementation curriculum designed to build practical engineering competence in autonomous agents and multi-agent distributed systems.

---

## Level 1: Foundations of Agentic AI (Projects 01-05)
- **Goal**: Understand model inference mechanics, context management, prompt engineering, structured tool calling, database interactions, and vector retrieval.
- **Core Stack**: Python, Pydantic, SQLite, OpenAI / Anthropic / Gemini API, ChromaDB / FAISS.
- **Projects**:
  1. `01-intelligent-ai-chat-agent`: Terminal conversation agent with sliding-window history, token counting, and cost telemetry.
  2. `02-tool-calling-ai-agent`: Deterministic tool integration using Pydantic schemas, validation, and JSON function returns.
  3. `03-ai-research-assistant`: Web search extraction agent synthesizing external findings with source citations.
  4. `04-personal-productivity-agent`: Task automation agent interacting with a local SQLite database via CRUD tools.
  5. `05-document-qa-agent`: Retrieval-Augmented Generation (RAG) agent chunking text, querying vector embeddings, and answering grounded questions.

---

## Level 2: Stateful & Integrated Agents (Projects 06-10)
- **Goal**: Implement persistent short/long-term memory, external SaaS APIs with OAuth 2.0, hybrid vector retrieval, and code repository inspection.
- **Core Stack**: Python, FastAPI, PostgreSQL, Redis, pgvector, GitHub API, Gmail API, Pytest.
- **Projects**:
  6. `06-memory-enabled-personal-ai-agent`: Dual-layer memory architecture combining Redis working memory and PostgreSQL episodic memory.
  7. `07-ai-email-management-agent`: Gmail integration classifying inbound emails, drafting replies, and requiring human-in-the-loop approval.
  8. `08-ai-coding-assistant-agent`: Code repository analyzer parsing Abstract Syntax Trees (AST), identifying defects, and drafting PR summaries.
  9. `09-rag-based-knowledge-base-agent`: Advanced RAG platform combining BM25 keyword search, dense vector retrieval, and cross-encoder reranking.
  10. `10-api-integration-agent`: FastAPI orchestration gateway executing multi-step third-party API workflows with exponential backoff retries.

---

## Level 3: Planning, Multi-Agent Systems & Evaluation (Projects 11-15)
- **Goal**: Master state-machine planning, multi-agent collaboration topologies, text-to-SQL data pipelines, and quantitative agent evaluation.
- **Core Stack**: Python, LangGraph / StateGraph, Pydantic, Pandas, SQLAlchemy, Tracing (LangSmith / OpenTelemetry), Pytest.
- **Projects**:
  11. `11-autonomous-planning-execution-agent`: Goal decomposition engine executing plans via a Directed Acyclic Graph (DAG) state machine with automated replanning.
  12. `12-multi-agent-research-system`: Collaborative graph featuring Researcher, Analyst, Fact-Checker, and Report Writer agents.
  13. `13-multi-agent-software-dev-system`: SDLC agent team coordinating Product, Architect, Developer, Tester, and Documentation agents in sandboxed workspaces.
  14. `14-ai-data-analyst-agent`: Safe Text-to-SQL analyst inspecting schemas, validating queries against AST guards, executing read-only SQL, and generating charts.
  15. `15-agent-evaluation-testing-platform`: Automated test harness evaluating tool-selection accuracy, hallucination rates, latency, and token consumption across model versions.

---

## Level 4: Enterprise, DevOps & Autonomous Systems (Projects 16-20)
- **Goal**: Develop production-grade, observable, secure, and multi-tenant agent platforms deployed on cloud and containerized infrastructure.
- **Core Stack**: Python, FastAPI, Docker, Kubernetes, Helm, Prometheus, Grafana, OpenTelemetry, Envoy / Kong, GitHub Actions.
- **Projects**:
  16. `16-devops-ai-operations-agent`: AIOps incident triage engine parsing logs, correlating Prometheus alerts, suggesting remediation runbooks, and enforcing least privilege.
  17. `17-ai-customer-support-platform`: Multi-agent support engine handling intent triage, knowledge retrieval, CRM ticketing, and seamless human agent escalation.
  18. `18-ai-business-operations-platform`: Cross-system business process orchestrator automating invoice approval routing, audit logging, and role-based permissions.
  19. `19-autonomous-software-engineering`: End-to-end repository worker taking GitHub issues, exploring codebases, running tests in Docker, and opening draft pull requests.
  20. `20-enterprise-agentic-ai-platform`: High-availability, multi-tenant agent gateway featuring an agent registry, model router, distributed queues, RBAC, and OpenTelemetry tracing.
