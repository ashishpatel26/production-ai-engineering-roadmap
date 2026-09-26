# Production AI Engineering Roadmap

🚀 Zero → AI Engineer Roadmap (2026)

Assumes basic ML/DL.

Goal: Learn to build and ship production LLM + agent systems.

## 1. LLM Internals

Resources:
- Karpathy — Neural Networks: Zero to Hero
- Jay Alammar — The Illustrated Transformer

Build:
- Implement a small GPT from scratch
- Understand attention, KV cache, tokenization, sampling

## 2. LLM APIs + Tool Calling

Resources:
- Anthropic — Prompt Engineering Guide
- OpenAI / Anthropic API docs
- Medium — LLM Function Calling Explained

Learn:
- Structured outputs
- Function/tool calling
- Streaming
- Retries, rate limits, token usage

Build:
- An API-based LLM application

## 3. RAG

Resources:
- Simon Willison — Embeddings / RAG
- Pinecone — RAG guides
- Medium — Modern RAG in 2026
- Medium — Reranking for RAG

Learn:
- Chunking
- Embeddings
- Hybrid search
- Reranking
- Metadata filtering
- Citations
- Query rewriting

Build:
- RAG over your own docs/PDFs

## 4. Evals

Resources:
- Hamel Husain — AI Evals
- Medium — Evaluating RAG Pipelines

Learn:
- Golden datasets
- Retrieval metrics
- LLM-as-judge
- Regression testing
- Failure analysis

Build:
- An eval suite for your RAG system

## 5. Agents

Resources:
- Anthropic — Building Effective Agents
- Sam Witteveen — Agents / Tool Use
- James Briggs — ReAct / Tool Use
- Medium — From LLMs to Agents

Learn:
- Tool use
- ReAct
- State
- Planning
- Retries
- Failure recovery
- Human-in-the-loop

Build:
- An agent with 3–5 real tools

## 6. Orchestration

Resources:
- LangGraph documentation
- Anthropic agent engineering articles

Learn:
- State machines
- Workflows vs agents
- Checkpoints
- Persistence
- Durable execution

Build:
- Convert your agent into an explicit stateful workflow

## 7. Context Engineering

Resources:
- Anthropic — Effective Context Engineering for AI Agents
- Medium — Context Engineering for Agentic Applications

Learn:
- Context selection
- Memory
- Compression
- Progressive disclosure
- Tool descriptions
- Long-context management

Build:
- A context layer for your agent

## 8. MCP

Resources:
- modelcontextprotocol.io
- Anthropic — MCP
- Medium — MCP Foundations
- Medium — MCP in Production

Build:
- One real MCP server for a tool you use
- Connect it to your agent

## 9. Inference Engineering

Resources:
- vLLM documentation
- SGLang documentation
- Hugging Face documentation

Learn:
- KV cache
- Batching
- Quantization
- Streaming
- Speculative decoding
- Model routing

Measure:
- TTFT
- Tokens/sec
- p50/p95 latency
- GPU memory
- Cost/request

## 10. AI Security

Resources:
- OWASP — LLM / GenAI Security
- Google Cloud — AI Security Evaluation
- Medium — AI Agent Security

Learn:
- Prompt injection
- Indirect prompt injection
- Tool poisoning
- Data exfiltration
- Excessive agency
- Authorization
- Sandboxing

## 11. Production

Learn:
- Observability
- Tracing
- Cost tracking
- Rate limiting
- Caching
- Load testing
- Guardrails
- Failure handling

Track:
- Quality
- Cost/request
- Latency
- Error rate
- Tool failures
- Task success rate

## Build 3 projects

1. Production RAG
2. Tool-using agent
3. Production agent platform

For every project, publish:
- Architecture
- Evaluation methodology
- Results
- Cost
- Latency
- Failure cases
- Tradeoffs

**Don't learn 10 frameworks.** Pick one stack and go deep.

**Don't build 15 toy chatbots.** Build 3 systems and measure them.

**Primary sources > AI roadmap listicles.** Medium is useful for implementation experience. Vendor docs, papers, specs, and engineering blogs should be your source of truth.

**Recommended book:** *AI Engineering* — Chip Huyen
