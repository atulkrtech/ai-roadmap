# AWS AI Engineer Learning Path

**Target Role:** AWS AI Engineer
**Estimated Timeline:** ~8–9 months (10–15 hrs/week) | ~5 months (20+ hrs/week)

---

## Phase 1: Deep Learning Foundations (Weeks 1–3)

### Course Options

| Course | Instructor |
|--------|-----------|
| PyTorch for Deep Learning & Machine Learning | Daniel Bourke |
| Deep Learning A-Z 2.0 | Kirill Eremenko / Hadelin de Ponteves |

### Topics Covered

- Neural networks fundamentals
- Convolutional Neural Networks (CNNs)
- Recurrent Neural Networks (RNNs) / LSTMs
- Training loops and optimization
- Prerequisite knowledge for understanding transformers & fine-tuning

---

## Phase 2: Foundations of Modern GenAI (Weeks 4–6)

### 2.1 NLP & Transformer Architecture

| Course | Instructor |
|--------|-----------|
| Hugging Face Transformers: From Zero to Hero | — |

**Topics Covered:**

- Text encoding & tokenization (BPE, WordPiece, SentencePiece)
- Transformer architecture (self-attention, positional encoding, encoder-decoder)
- Embeddings, vector space & similarity measures
- Word, contextual, and sentence embeddings
- Classical encoding techniques and the shift to word embeddings

### 2.2 Generative AI Core Concepts

| Course | Instructor |
|--------|-----------|
| Generative AI for Beginners: A Comprehensive Introduction | — |
| Master Generative AI with LLMs (alternative) | Lazy Programmer |

**Topics Covered:**

- What GenAI is and how LLMs work at a high level
- LLMs vs SLMs vs Multimodal models
- Major LLM families: GPT, Gemini, Claude, LLaMA, Mistral, Qwen
- Small & efficient models: Phi, Gemma
- Specialized models: CodeLLaMA, StarCoder, DeepSeek-Coder, LLaVA, BLIP, CLIP
- Model selection strategy (task type, cost, latency, modality, deployment)

---

## Phase 3: LLM APIs & Prompt Engineering (Weeks 7–9)

### Course

| Course | Instructor |
|--------|-----------|
| ChatGPT, LangChain, & LLM APIs: Build GenAI Apps | — |

### Topics Covered

**LLM API Ecosystem:**

- OpenAI, Anthropic, Gemini, Groq, OpenRouter APIs
- Making API calls: prompt → request → response
- Parameters: temperature, max tokens
- Streaming vs non-streaming
- Token usage, pricing models, cost control strategies
- Provider switching & abstraction layers (OpenAI ↔ Groq ↔ OpenRouter)
- AWS Bedrock as the enterprise-managed API layer

**Prompt Engineering:**

- System vs User prompts
- Zero-shot, few-shot prompting
- Chain-of-Thought (CoT), self-consistency, ReAct (Reason + Act)
- Task-wise and domain-specific prompting
- Prompt libraries, Jinja2 templates, YAML-based prompt configuration
- JSON/YAML outputs, schema-based prompts, guarded output enforcement
- Token cost optimization and context window optimization

---

## Phase 4: RAG Systems (Weeks 10–13)

### Courses

| Course | Instructor |
|--------|-----------|
| LangChain — Develop LLM powered applications with LangChain | Eden Marco |
| RAG (Retrieval Augmented Generation) — Build AI Apps | — |

### Topics Covered

**Core RAG:**

- Why LLMs hallucinate & why RAG is needed
- End-to-end RAG system architecture: ingestion → indexing → retrieval → generation → response
- Data ingestion & parsing: PDFs, docs, web data, structured vs unstructured
- Chunking strategies: when to chunk, when NOT to chunk, overlap trade-offs
- Embeddings & vector databases: Pinecone, Chroma, FAISS, Weaviate
- Metadata design, schemas, filters, and scoped retrieval
- Retrieval, ranking & re-ranking: similarity search, MMR, cross-encoder
- Prompting with retrieved context: context injection, grounding, citation-aware prompting

**Advanced RAG:**

- Context engineering & memory management
- Caching & performance optimization: response caching, embedding cache
- RAG evaluation & reliability: faithfulness, relevance, retrieval quality
- Multimodal RAG systems: text + image retrieval
- Common failure modes: bad chunks, noisy retrieval, missing context, overlong prompts

---

## Phase 5: Fine-Tuning LLMs (Weeks 14–17)

### Courses

| Course | Instructor |
|--------|-----------|
| Fine-Tuning Large Language Models (LLMs) | — |
| Hugging Face: Deploy & Fine-Tune LLMs | — |

### Topics Covered

- Foundations of fine-tuning: classical DL (CNNs), limitations of RNN/LSTM, why transformers scale
- Hugging Face ecosystem vs LangChain (training vs orchestration mindset)
- Full fine-tuning vs parameter-efficient approaches
- **LoRA, QLoRA, PEFT** overview and when to use each
- Dataset preparation: instruction datasets, formatting, cleaning, train/validation splits
- Knowledge distillation and quantization in LLMs
- Frameworks: Hugging Face Transformers, PEFT, Unsloth, Axolotl
- API-based fine-tuning: OpenAI / provider-based workflows and limitations
- Model packaging: Hugging Face checkpoints, Safetensors, GGUF, GGML formats
- **RLHF, DPO, ORPO, GRPO** (conceptual positioning)
- Embedding model fine-tuning
- Vision-language model fine-tuning

---

## Phase 6: Agents & Multi-Agent Systems (Weeks 18–22)

### Courses

| Course | Instructor |
|--------|-----------|
| LangGraph — Build Multi-Agent AI Apps | Eden Marco |
| CrewAI — Build Multi-Agent AI Systems | — |

### Topics Covered

- Agentic AI fundamentals: agents vs simple LLM pipelines
- Single-agent architectures: planning, reasoning, acting loops
- Multi-agent system designs: supervisor, hierarchical, network-based
- Deep agent systems: long-horizon agents with planning, reflection, iterative execution
- LLMs as the reasoning & decision core
- Tools as agent interfaces: APIs, functions, search, RAG, code execution
- Agent orchestration layers: LangGraph, CrewAI
- Memory & state management: short-term, long-term, shared state
- Prompting strategies: role-based, planner, executor prompts
- Human-in-the-loop: approval gates, feedback loops, interrupt & resume
- Safety controls & loop prevention: max steps, termination conditions, error handling
- Cost & execution management: token budgeting, execution limits
- Agentic RAG architectures
- Inter-agent collaboration: task delegation, result aggregation, conflict resolution

---

## Phase 7: Guardrails, Evaluation & MCP (Weeks 23–25)

### 7.1 Guardrails & Evaluation

| Course | Instructor |
|--------|-----------|
| LLMOps: Deploy LLMs to Production | — |

**Guardrails Topics:**

- What guardrails are and why GenAI systems need them
- Guardrails in traditional software vs GenAI systems
- Core objectives: safety, reliability, compliance, trust
- Input validation: prompt sanitization, length limits, content filtering
- Output validation: response checks, format enforcement, refusal logic
- Schema-based guardrails: Pydantic-based schemas for structured outputs
- Prompt injection attacks: types and defense strategies
- Tools: Guardrails.ai, OpenAI Guardrails, custom rule-based approaches

**Evaluation Topics:**

- Observability & debugging: logging, monitoring, tracing
- Why classical evaluation breaks for GenAI
- Model-level vs system-level evaluation
- LLM-as-a-judge, human-in-the-loop, offline vs online evaluation
- RAG & agentic system evaluation: grounding, relevance, faithfulness, hallucination detection
- System-level metrics: cost, latency, UX, quality–speed–cost trade-offs
- Classical metrics: perplexity, loss, token-level metrics
- Task-specific metrics: accuracy, BLEU, ROUGE, exact match vs semantic match
- Common anti-patterns: single-metric obsession, ignoring cost/latency

### 7.2 MCP (Model Context Protocol)

> **Self-study** — No dedicated Udemy course available yet.
> Resources: [Anthropic MCP Documentation](https://modelcontextprotocol.io) + YouTube tutorials

**Topics Covered:**

- What MCP is and why it was introduced
- MCP vs plugins vs function calling
- MCP with RAG, agents, and complex workflows
- Architecture: Client ↔ Server ↔ LLM interaction model
- Core components: MCP Host, MCP Client, MCP Server
- Transports: STDIO, SSE, Streamable HTTP, stateful vs stateless servers
- Python SDK: FastMCP vs low-level servers, CLI tools
- Building MCP servers: project structure, lifecycle
- Capabilities: tools, structured outputs, reusable prompts, context objects
- Advanced: authentication, OAuth, pagination, large data handling
- MCP for agentic AI systems

---

## Phase 8: AWS AI/ML Services (Weeks 26–30)

> You likely already know S3, IAM, Lambda, ECS, VPC — skip AWS basics entirely.

### 8.1 AWS ML & SageMaker

| Course | Instructor |
|--------|-----------|
| AWS Certified Machine Learning Specialty | Stephane Maarek / Frank Kane |
| Amazon SageMaker: Build ML Models & Deploy | — |

**Topics Covered:**

- SageMaker: model training, fine-tuning, deployment, MLOps workflows
- Fine-tuning a base model on SageMaker (LoRA-based)
- Deploying LLMs as SageMaker endpoints: real-time inference & scaling
- API exposure: API Gateway or Application Load Balancer (ALB)
- AWS Lambda for lightweight or burst inference
- ECS Fargate for container-based scalable inference
- Client integration: calling deployed LLM API from frontend/backend

### 8.2 AWS GenAI Services

| Course | Instructor |
|--------|-----------|
| AWS Bedrock — Generative AI on AWS | — |
| AWS Certified AI Practitioner AIF-C01 | Stephane Maarek |

**Topics Covered:**

- Amazon Bedrock: managed foundation models and GenAI inference
- Amazon OpenSearch Service: vector search and RAG-enabled search
- Amazon Textract: OCR/document intelligence
- Amazon Comprehend: NLP
- Amazon Rekognition: vision
- Amazon Transcribe: speech-to-text
- Agent Core (AWS)
- Cloud-native deployment: ECS/Fargate, S3, RDS, CI/CD pipelines, observability

---

## Phase 9: No-Code Agents — n8n (Week 31)

### Course

| Course | Instructor |
|--------|-----------|
| n8n Masterclass: AI Automation | — |

### Topics Covered

- What n8n is, where it fits in GenAI automation
- Setup, interface, nodes, workflows, JSON handling
- Calling APIs, using LLMs inside workflows
- Agent patterns: chain, parallel, controller, hierarchical
- RAG with Supabase / Pinecone integration
- MCP basics, n8n cloud vs self-hosted
- Real automation: social media, GitHub PR, WhatsApp / Assistant workflows

---

## Phase 10: End-to-End Projects (Weeks 32–36)

### Supplementary Course

| Course | Instructor |
|--------|-----------|
| Build LLM Apps: End-to-End Projects | — |

### Project 1: Document Portal System

**Tech Stack:** FastAPI + LangChain + Vector DB + Redis + AWS ECS/Fargate + S3

| Module | Description |
|--------|-------------|
| Document Ingestion Pipeline | Upload → parse → chunk → embed → index with async, scalable processing |
| Advanced RAG Architecture | Query rewriting, MMR, re-ranking, citation-aware answer generation |
| Single & Multi-Document Chat | Conversational memory, context condensation, source-grounded responses |
| Document Comparison Engine | Semantic comparison and question-driven side-by-side analysis |
| LLM Orchestration Layer | Model routing (Groq / OpenAI / local), prompt & context policies |
| Caching & Performance | Redis caching, Cache-Augmented Generation (CAG), embedding reuse |
| Scalability & Reliability | Stateless APIs, autoscaling, queues, retries, and fallbacks |
| Evaluation & Guardrails | Faithfulness, relevance, safety checks, refusal on insufficient context |
| Cloud-Native Deployment | AWS ECS/Fargate, S3, RDS, Vector DB, CI/CD pipelines, observability |

### Project 2: Autonomous Report Generation System

**Tech Stack:** LangGraph + OpenAI/Groq + FastAPI + Vector DB + AWS

| Module | Description |
|--------|-------------|
| Agentic AI Foundations | Single-agent vs multi-agent systems, roles, async orchestration |
| LLM & Tooling Setup | Base LLM (OpenAI / Groq), tool calling, function schemas |
| Agent Role Design | Search, Reader, Analyst, Generator, Coordinator with clear responsibilities |
| Agent Orchestration | LangGraph / CrewAI / AutoGen workflows and state graphs |
| Memory & Communication | Shared state, short-term vs long-term memory, context control |
| Research Toolkits | Web search APIs, Arxiv/PDF parsers, document loaders |
| RAG Integration | Vector DB, external knowledge grounding, citation-aware outputs |
| Human-in-the-Loop | Feedback checkpoints, approvals, interrupt & resume flows |
| UI & Backend | FastAPI task dispatcher, report previews, agent logs & traces |

---

## Complete Course List

| # | Course | Phase | Weeks |
|---|--------|-------|-------|
| 1 | Deep Learning (PyTorch or DL A-Z) | 1 | 1–3 |
| 2 | Hugging Face Transformers | 2 | 4–5 |
| 3 | Generative AI Introduction | 2 | 5–6 |
| 4 | LangChain — Build LLM Apps | 3+4 | 7–13 |
| 5 | RAG Systems (dedicated course) | 4 | 10–13 |
| 6 | Fine-Tuning LLMs | 5 | 14–16 |
| 7 | Hugging Face: Deploy & Fine-Tune | 5 | 16–17 |
| 8 | LangGraph — Multi-Agent AI | 6 | 18–20 |
| 9 | CrewAI — Multi-Agent Systems | 6 | 20–22 |
| 10 | LLMOps: Deploy LLMs to Production | 7 | 23–25 |
| 11 | AWS ML Specialty / SageMaker | 8 | 26–28 |
| 12 | AWS Bedrock & GenAI on AWS | 8 | 28–30 |
| 13 | AWS Certified AI Practitioner | 8 | 28–30 |
| 14 | n8n AI Automation | 9 | 31 |

**Self-study:** MCP (Model Context Protocol) — Anthropic docs + YouTube

---

## Target Certifications

| Certification | When to Attempt |
|---------------|-----------------|
| AWS Certified AI Practitioner (AIF-C01) | After Phase 8 |
| AWS Certified Machine Learning Specialty | After Phase 8 |

---

## Timeline Summary

| Phase | Topic | Weeks |
|-------|-------|-------|
| 1 | Deep Learning Foundations | 1–3 |
| 2 | Foundations of Modern GenAI | 4–6 |
| 3 | LLM APIs & Prompt Engineering | 7–9 |
| 4 | RAG Systems | 10–13 |
| 5 | Fine-Tuning LLMs | 14–17 |
| 6 | Agents & Multi-Agent Systems | 18–22 |
| 7 | Guardrails, Evaluation & MCP | 23–25 |
| 8 | AWS AI/ML Services | 26–30 |
| 9 | No-Code Agents (n8n) | 31 |
| 10 | End-to-End Projects | 32–36 |

**Total: ~36 weeks (8–9 months) at 10–15 hrs/week | ~5 months at 20+ hrs/week**
