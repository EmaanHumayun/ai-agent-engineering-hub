# Technology Stack & Rationale

This document defines the toolchain, libraries, and infrastructure components used across the AI Agent Engineering curriculum.

---

## Technology Progression Matrix

| Category | Beginner (01-05) | Intermediate (06-10) | Advanced (11-15) | Professional (16-20) |
| :--- | :--- | :--- | :--- | :--- |
| **Programming Language** | Python 3.10+ | Python 3.10+ | Python 3.10+ (Async) | Python 3.11+, Bash |
| **Web Framework** | - | FastAPI, HTTPX | FastAPI | FastAPI, Uvicorn, Gunicorn |
| **Data Validation** | Pydantic v2 | Pydantic v2 | Pydantic v2 | Pydantic v2 |
| **Database & Persistence** | SQLite | PostgreSQL, Redis | PostgreSQL | PostgreSQL, Redis, MinIO |
| **Vector Storage** | ChromaDB / In-Memory | pgvector / Qdrant | Qdrant / FAISS | Milvus / pgvector |
| **Agent Orchestration** | Pure Python loops | Custom Dispatchers | LangGraph / StateGraph | LangGraph, Celery, K8s |
| **Static & SQL Analysis** | - | AST, GitPython | SQLGlot | AST, Docker SDK, Paramiko |
| **Testing & Evaluation** | Pytest | Pytest, Mock APIs | Pytest, Ragas, Tracing | Pytest, Testcontainers |
| **Infrastructure & DevOps**| Local environment | Docker | Docker Compose | Docker, Kubernetes, Helm |
| **Observability** | Console logs | Structured JSON logs | OpenTelemetry, Traces | Prometheus, Grafana, OpenTelemetry |

---

## Tool Rationale

### Why Python?
Python is the undisputed industry standard for AI, machine learning, and agentic workflows. Its native support for dynamic typing, rich AST inspection, mature async runtimes, and universal SDK adoption across major model providers makes it ideal for building robust agent loops.

### Why Pydantic?
Pydantic v2 offers ultra-fast C-extension data validation and automatic JSON Schema generation. In agentic systems, Pydantic models guarantee that LLM function call arguments strictly adhere to expected types before tool execution.

### Why LangGraph for Advanced Tiers?
Unlike rigid sequential pipelines, LangGraph models agent reasoning as a Directed Acyclic Graph (DAG) with cycles. This enables deterministic state persistence, branching, human-in-the-loop pause/resume checkpoints, and multi-agent cyclic loops.
