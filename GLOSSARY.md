# AI Agent Engineering Glossary

Formal definitions of core terms across LLM inference, cognitive loops, tool calling, and multi-agent systems.

- **AI Agent**: A software component that uses an LLM to reason, plan, and autonomously execute actions via tools to achieve a specified goal.
- **Agent Loop**: The iterative execution cycle wherein an agent perceives state, queries a model, executes chosen tools, and reflects on outcomes.
- **Context Window**: The maximum sequence of tokens (prompt + completion) an LLM can process in a single inference call.
- **Function / Tool Calling**: A capability allowing models to output structured JSON arguments matching a predefined schema to invoke external functions.
- **Groundedness**: The degree to which an agent's claims are directly supported by retrieved context rather than unverified internal model weights.
- **Hallucination**: Generated model output that presents incorrect, ungrounded, or fabricated information as factual.
- **Human-in-the-Loop (HITL)**: A system design pattern requiring explicit manual authorization before an agent can execute high-stakes or irreversible actions.
- **Prompt Injection**: A security vulnerability wherein untrusted inputs manipulate an LLM into ignoring instructions and executing malicious commands.
- **Retrieval-Augmented Generation (RAG)**: Architecture enriching prompt context with relevant documents retrieved from external knowledge bases.
- **Token**: The atomic unit of text (typically 3-4 characters in English) processed by language models.
