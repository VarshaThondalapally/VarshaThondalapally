# Backend and Workflow Systems

## The hiring case

I turn long-running, failure-prone AI and business processes into explicit state machines that can survive refreshes, retries, concurrent edits, restarts, payment events, and third-party failures.

The professional system I worked on used FastAPI, Pydantic, async SQLAlchemy, PostgreSQL, S3, Redis, SQS/Lambda, Stripe, and a third-party estimating platform. PostgreSQL held operational truth while S3 held source and generated artifacts.

## Technical decisions I implemented

- Modeled users, clients, sessions, rooms, sources, pages, line items, suggestions, audits, conversations, jobs, revisions, payments, usage, and delivery state.
- Evolved the schema through 91 Alembic migrations with indexes, constraints, repair paths, and backfills.
- Added base revisions, structured stale-write conflicts, before-and-after history, and approval invalidation after mutation.
- Implemented Redis-backed and database-backed jobs with queued, running, terminal, progress, error, retry, lease, and startup-recovery state.
- Built an earlier S3-to-SQS-to-Lambda processing path with SNS status and poison-job handling.
- Preserved database and object-storage consistency through exact object identity, rollback cleanup, and dependency-aware deletion.
- Implemented Stripe subscription, trial, usage, overage, webhook, entitlement, reconciliation, deduplication, and repair workflows.
- Treated third-party delivery as an authenticated, diagnosable process with project and transaction identity, XML/file/API exchange, retry classification, readiness checks, and saved history.

## Concrete failure converted into an invariant

Durable interaction records introduced a foreign-key deletion failure. I traced the dependency order, changed cleanup to delete children before parents, restricted S3 removal to exact owned keys, and added regression coverage. The lesson was broader than one bug: distributed cleanup must respect both relational dependency order and storage ownership boundaries.

## Important boundary

The evidence supports production-shaped backend and distributed-workflow engineering. It does not support claims of pristine microservices, universal queue-first architecture, measured high availability, or millions of production transactions.

## Public proof

- [Commerce Action Reliability Lab](https://github.com/VarshaThondalapally/commerce-action-reliability-lab): PostgreSQL transactional outbox, idempotency, reconciliation, compensating revisions
- [Live reviewer demo](https://varshathondalapally.github.io/commerce-action-reliability-lab/)

[Back to profile](../README.md)
