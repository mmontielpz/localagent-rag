# localagent-rag

An open-source, local-first agentic RAG system built with modular architecture, multi-step planning, tool execution, evaluation, and production-ready practices.

## Overview

localagent-rag is a modular AI engineering project designed to demonstrate how to build a fully local, cost-free, agentic LLM system capable of:

- Multi-step planning
- Tool usage
- Retrieval-Augmented Generation (RAG)
- Structured reasoning
- Automatic evaluation
- Observability and logging
- Containerized deployment

This project avoids paid APIs and runs entirely on open-source components.

---

## Architecture

High-level flow:

User  
↓  
FastAPI  
↓  
LangGraph Orchestrator  
↓  
Planner → Executor → Critic → Reporter  
↓  
Tools (Retriever, Calculator, etc.)  
↓  
Evaluation Layer  
↓  
Logs / MLflow  

---

## Tech Stack

- Python 3.11
- Poetry (dependency management)
- LangGraph (agent orchestration)
- ChromaDB (vector database)
- Sentence Transformers (embeddings)
- FastAPI (API layer)
- MLflow (experiment tracking)
- Docker (containerization)
- GitHub Actions (CI)

All components are open-source.

---

## Project Structure

```

localagent-rag/
├── agents/
├── tools/
├── rag/
├── evaluation/
├── api/
├── tests/
├── docs/
├── pyproject.toml
└── README.md

````

---

## Installation

### 1. Clone

```bash
git clone https://github.com/YOUR_USERNAME/localagent-rag.git
cd localagent-rag
````

### 2. Install dependencies

```bash
poetry install
```

### 3. Activate environment

```bash
poetry shell
```

---

## Running Tests

```bash
poetry run pytest
```

---

## Development Workflow

* main → stable branch
* dev → integration branch
* feature/* → isolated feature development

All commits follow Conventional Commits format.

---

## Roadmap

* [ ] Core agent graph
* [ ] RAG ingestion pipeline
* [ ] Tool execution system
* [ ] Evaluation framework
* [ ] API layer
* [ ] Observability
* [ ] Docker deployment
* [ ] Benchmark dataset

---

## License

MIT