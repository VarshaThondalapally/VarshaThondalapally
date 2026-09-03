# Varsha Thondalapally

Applied AI engineer building evidence-grounded, human-reviewed systems around probabilistic models.

I work across model workflows, backend systems, durable product state, review experiences, cloud operations, billing, and external integrations. My strongest engineering pattern is turning uncertain model output and messy operational evidence into software that can be reviewed, recovered, audited, and safely acted on.

## Technical scope

| Layer | Demonstrated work |
| --- | --- |
| Applied AI | OpenAI and Gemini workflows, multimodal inputs, structured outputs, embeddings, FAISS, hybrid retrieval, reranking, and source grounding |
| Evaluation and controls | Versioned cases, scenario regression, deterministic validation, ambiguity handling, human approval, provenance, and model/workflow telemetry |
| Workflow reliability | Durable state, revision and stale-state controls, idempotency, transactional outbox, retries, reconciliation, and recovery |
| Product engineering | Python, FastAPI, Pydantic, PostgreSQL, SQLAlchemy, Alembic, React, and TypeScript |
| Operations and integrations | Docker, AWS ECS/Fargate, RDS, S3, CloudWatch, Redis, SQS, Lambda, Stripe, and third-party delivery workflows |

## Start here

### 1. [Commerce Action Reliability Lab](https://github.com/VarshaThondalapally/commerce-action-reliability-lab)

An independent synthetic evaluation of free-form versus bounded LLM decision architecture.

- 20 versioned gold cases
- deterministic entity and policy controls
- revision-bound human approval
- PostgreSQL transactional outbox
- idempotency, timeout reconciliation, and compensating revisions
- 61 CI-verified tests, including seven PostgreSQL integration tests
- [Live reviewer demo](https://varshathondalapally.github.io/commerce-action-reliability-lab/)

The live-provider benchmark is pending; no live accuracy, latency, cost, production-use, or real-commerce claim is made.

### 2. [Recipe Review Evidence Pipeline](https://github.com/VarshaThondalapally/recipe-review-evidence-pipeline)

A measured LLM extraction-and-action pipeline that converts attributed review evidence into exact, deterministic edits.

- strict Pydantic extraction contracts
- quote grounding and evidence-state classification
- transactional edit bundles
- hand-labeled evaluation across 12 reviews
- recorded intent, grounding, edit, latency, and token results
- CI across Python 3.11 and 3.13 with coverage, lint, type, and dependency checks

This is a small independent evaluation, not a production or food-safety claim.

### 3. [ShiftMemory](https://github.com/VarshaThondalapally/shiftmemory-cognee-hackathon)

A source-grounded team-memory demonstration using Cognee, Gemini, FastAPI, and React.

- remember, recall, improve, and forget lifecycle
- source verification before generated handoffs
- role-based access and assignment boundaries
- backend-owned provider credentials
- reviewer feedback and auditable traces
- recorded Cognee/Gemini lifecycle verification

## Professional work and ownership boundary

At an early-stage company, I was employee #1 and served as the only full-time engineer, developing and operating substantial parts of a company-owned vertical-AI product from its first working vertical slice through deployed operations.

That work included multimodal evidence processing, retrieval and authoritative-data resolution, structured model outputs, human review, durable workflow state, AWS operations, billing, and third-party integrations.

The employer owns that product, its source code, designs, data, and intellectual property. The repositories above are independently created synthetic projects that demonstrate transferable engineering patterns without copying employer materials.

## Role focus

Applied AI Engineer · AI Product Engineer · Product-oriented Forward Deployed Engineer

[LinkedIn](https://www.linkedin.com/in/varshase/)
