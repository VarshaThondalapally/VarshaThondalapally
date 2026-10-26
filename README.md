# Varsha Thondalapally

**Applied AI Engineer** building the software that makes model output usable: retrieval, structured outputs, deterministic validation, durable state, human review, external integrations, and AWS operations.

At an early-stage company building insurance-restoration software, I was employee #1 and the only full-time engineer. I developed substantial parts of a company-owned vertical-AI workflow from an early React/FastAPI scaffold to its first working vertical slice in about five weeks, then continued through deployment and operations.

## Choose the proof path that matches what you are hiring for

| Hiring need | Relevant evidence |
| --- | --- |
| Applied AI and LLM systems | [Retrieval, model routing, structured outputs, guardrails, and human review](proof/applied-ai-llm-systems.md) |
| Backend and workflow systems | [PostgreSQL state, queues, recovery, concurrency, billing, and integrations](proof/backend-workflow-systems.md) |
| Multimodal and document AI | [PDF, image, sketch, audio, page, room, and source-aware processing](proof/multimodal-document-ai.md) |
| AI evaluation and reliability | [Behavioral regression, deterministic graders, telemetry, and independent eval proof](proof/ai-evaluation-reliability.md) |
| Startup full-stack execution | [Zero-to-one React/FastAPI delivery through AWS operation](proof/startup-full-stack-execution.md) |

## Fifteen-second technical evidence

- Replaced permissive AI selection with hybrid retrieval, constrained candidates, typed outputs, and exact resolution against an authoritative 14,211-record catalog.
- Made human approval revision-aware so an earlier decision could not silently authorize changed work.
- Persisted long-running workflows across refreshes and restarts using PostgreSQL-backed state, Redis or SQS/Lambda job paths, retries, leases, and recovery.
- Treated Stripe and third-party delivery as stateful, retryable workflows with entitlement, identity, reconciliation, and failure boundaries.
- Containerized, deployed, and troubleshot the application across ECS/Fargate, ALB, RDS, S3/CloudFront, Route 53/ACM, ElastiCache, CloudWatch, IAM, CloudTrail, and GuardDuty.

## Public, candidate-owned proof

### [Commerce Action Reliability Lab](https://github.com/VarshaThondalapally/commerce-action-reliability-lab)

A React/TypeScript, FastAPI, and PostgreSQL reference system showing how model proposals become bounded, reviewable actions.

- 20 versioned synthetic cases
- structured provider contracts and authoritative entity resolution
- deterministic policy gates and revision-bound approval
- PostgreSQL transactional outbox and idempotent execution
- timeout-after-success reconciliation and compensating revisions
- 62 verified deterministic and PostgreSQL integration tests, plus 10 retry-explainer tests
- [Live reviewer demo](https://varshathondalapally.github.io/commerce-action-reliability-lab/)
- [See it in 60 seconds: interactive retry explainer](https://varshathondalapally.github.io/commerce-action-reliability-lab/explainer/index.html)

### [Recipe Review Evidence Pipeline](https://github.com/VarshaThondalapally/recipe-review-evidence-pipeline)

A measured LLM extraction-and-action pipeline using strict Pydantic contracts, quote grounding, transactional edit bundles, and a hand-labeled 12-review evaluation.

### [Udyogam Job Intelligence](https://github.com/VarshaThondalapally/udyogam-job-intelligence)

Evidence-grounded pipeline from live careers pages to LLM-ready job documents and cited company research.

### Restoration intake workflow

[Restoration AI Operations Reliability Lab](https://github.com/VarshaThondalapally/restoration-ai-operations-reliability-lab) shows synthetic intake, clarification, safety escalation, and human handoff. It is a frontend prototype with 18 regression scenarios; it does not reproduce the professional product or connect to a real dispatch system.

### Additional demonstration

[ShiftMemory](https://github.com/VarshaThondalapally/shiftmemory-cognee-hackathon) is a synthetic hackathon demonstration of source-grounded team memory and role boundaries.

## Professional engineering case

The [sanitized professional case study](https://varsha-ai.notion.site/From-Messy-Evidence-to-Controlled-Action-Applied-AI-Engineering-Case-Study-3d006085ac208097a192dd7b776dd685) contains the longer idea-to-operated-product history. The role-specific pages above are the faster entry points for hiring teams.

The employer owns the professional product, source code, designs, data, and intellectual property. The public repositories use independent synthetic data and do not reproduce employer materials.

[LinkedIn](https://www.linkedin.com/in/varshase/) | [Email](mailto:varshareddy1601@gmail.com) | [Request a current resume](mailto:varshareddy1601@gmail.com?subject=Current%20resume%20request)
