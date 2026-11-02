# Learning Path & Progression Guide

This guide details the sequential progression of skills, theoretical concepts, and engineering milestones across the curriculum.

---

## Progression Flowchart

```
[ Level 1: Foundations ]
   - Prompt Engineering & Context Management
   - Function Calling & Tool Schemas (Pydantic)
   - In-Memory & SQLite Persistence
   - Basic Vector Embeddings & Similarity Search
         |
         v
[ Level 2: Stateful & Integrated Systems ]
   - Short-term (Redis) vs Long-Term (PostgreSQL) Memory
   - OAuth 2.0 & Human-in-the-Loop Safeguards
   - Repository AST Inspection & Code Analysis
   - Hybrid Search RAG (BM25 + Dense Vectors) + Reranking
         |
         v
[ Level 3: Planning, Multi-Agent & Evaluation ]
   - DAG State Machines & Replanning Loops (LangGraph)
   - Multi-Agent Orchestration & Task Delegation
   - Safe Text-to-SQL with AST Query Validation
   - Quantitative Evaluation Frameworks (Accuracy, Groundedness, Hallucination)
         |
         v
[ Level 4: Enterprise Production & Cloud Platforms ]
   - AIOps Infrastructure & Log Telemetry Integration
   - Multi-Tenant Isolation & Role-Based Access Control (RBAC)
   - Sandboxed Docker / Containerized Execution Environments
   - Distributed Tracing (OpenTelemetry) & Production Kubernetes Gateways
```

---

## Progression Criteria Between Levels

### Moving from Level 1 to Level 2
- Understand tokenization, context windows, and cost modeling.
- Implement structured tool schemas using Pydantic without schema errors.
- Construct a deterministic single-agent ReAct loop handling tool failure gracefully.

### Moving from Level 2 to Level 3
- Implement dual-layer memory architectures with automatic session context trimming.
- Build authenticated API integrations featuring token rotation and retry policies.
- Quantitatively evaluate retrieval recall and precision in a RAG pipeline.

### Moving from Level 3 to Level 4
- Build multi-agent coordination graphs with isolated state and message passing.
- Construct comprehensive automated evaluation suites asserting tool selection and groundedness.
- Enforce sandboxed execution and prompt injection defense on untrusted user inputs.
