# Hi, I'm Nitesh

CSE undergrad at VIT Vellore (Bioinformatics specialisation, graduating 2028).
I work on backend systems and applied LLM infrastructure — retrieval pipelines,
agent orchestration, and the unglamorous plumbing that makes them reliable.

## What I'm building

**[SureShot](https://github.com/Nitesh050/SureShot)** — security scanning where the
hard problem is triage, not detection.

Semgrep and Trivy already find plenty. The trouble is what comes back: hundreds of
findings, most of them noise, and no good way to tell which ones matter. SureShot
runs those scanners and puts an LLM triage layer in front of the results, so what
reaches you is the subset worth acting on.

Built as a real system rather than a portfolio piece:

- Python 3.12, `uv` workspace monorepo, Pydantic v2 domain models
- Multi-tenant from the schema up, not bolted on later
- Control plane / data plane separation — API, worker, and scheduler as distinct services
- Transactional outbox for reliable event delivery
- Prompt injection defense and secret redaction at adapter boundaries
- Degraded-not-failed semantics: a partial scan returns partial results instead of nothing

In active development — domain and engine packages are in place, services are next.

## Other projects

**[RAG-Based PDF Analyzer](https://github.com/Nitesh050/rag-pdf-analyzer)** —
natural-language querying over uploaded PDFs. LangChain ingestion pipeline
(loading, chunking, embeddings) indexed into ChromaDB, with retrieval quality
pushed up via metadata filtering, BM25, hybrid search, and reranking. Locally
hosted LLMs through Ollama behind FastAPI endpoints, fully containerised for
one-command setup.

**[Full-Stack E-Commerce Platform](https://github.com/Nitesh050/ecommerce-platform)** —
React and Node/Express over a normalised PostgreSQL schema, with indexed catalog
and order-history queries, hashed-password auth with protected routes, and a
payment gateway integration handling transaction verification and failure paths.

## Experience

**AI Intern, Qualitia Software** (May–June 2026) — Built RAG pipelines for
large-scale document processing and the FastAPI microservices serving them
asynchronously. Wrote a Java multithreaded AI Job Manager on the Executor
Framework and CompletableFuture, with job tracking, snapshots, and selective
cancellation that cut redundant LLM token spend on superseded work.

## Working with

**Languages** Python · Java · C/C++ · TypeScript · SQL
**AI** LLMs · RAG · LangChain · LangGraph · embeddings · hybrid search
**Backend** FastAPI · Node.js · Docker · PostgreSQL · ChromaDB
**Other** React · AWS (EC2, S3, Lambda) · Linux · Git

## Reach me

- mniteshpandey.005@gmail.com
- [linkedin.com/in/niteshpandey05](https://linkedin.com/in/niteshpandey05)
