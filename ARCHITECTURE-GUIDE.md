# AI Agent Architecture Guide

Comprehensive reference detailing architectural patterns, state representations, cognitive loops, and security guardrails for agentic systems.

---

## 1. The Core Agent Loop (ReAct Pattern)

```
                     [ User Goal / Event ]
                               |
                               v
                     +-------------------+
                     | Context Assembly  | <--- [ Short/Long Memory ]
                     +-------------------+
                               |
                               v
                  +-------------------------+
                  |  LLM Cognitive Step     |
                  |  (Reasoning & Planning) |
                  +-------------------------+
                               |
            +------------------+------------------+
            |                                     |
    (Tool Call Required)                    (Goal Fulfilled)
            |                                     |
            v                                     v
+-----------------------+              +----------------------+
| Schema Validation     |              | Final Output Return  |
+-----------------------+              +----------------------+
            |
            v
+-----------------------+
| Deterministic Tool    |
| Execution             |
+-----------------------+
            |
            v
+-----------------------+
| Append Result to State|
+-----------------------+
            |
            +------------------+ (Loop back for next reasoning step)
```

---

## 2. Memory Architectures

### Short-Term (Working Context)
- Maintained inside the model's active context window.
- In-memory message queues trimmed via sliding-window algorithms or token-budget summarizers.

### Long-Term (Episodic & Semantic Memory)
- Stored externally in PostgreSQL (relational event history) and vector databases (semantic embeddings).
- Queried via cosine similarity to recall relevant past conversations or user preferences.

---

## 3. Human-in-the-Loop (HITL) Architecture

Destructive or sensitive actions (transmitting emails, modifying infrastructure, financial payments) must never execute autonomously without verified human review:

```
[ Agent proposes action ] ---> [ Action flagged as SENSITIVE ]
                                        |
                                        v
                            [ Save checkpoint to State ]
                            [ Send Approval Notification ]
                                        |
                            +-----------+-----------+
                            |                       |
                     (Approved)                 (Rejected)
                            |                       |
                            v                       v
               [ Execute Action Handler ]  [ Append Rejection Notice ]
                            |                       |
                            +-----------+-----------+
                                        |
                                        v
                          [ Resume Agent Execution ]
```
