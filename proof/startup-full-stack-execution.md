# Startup Full-Stack Execution

## The hiring case

I am strongest when a small team has an important workflow but the product, system boundaries, and failure behavior are still being discovered.

At Roitech, I was employee #1 and the only full-time engineer. Starting from a minimal React/FastAPI scaffold and a company-supplied concept, I implemented the first working vertical slice in about five weeks: authentication, protected routes, users, clients, sessions, PostgreSQL state, multi-file uploads, assessment capture, AI follow-up, grounded retrieval, editable output, and assignment state.

I continued developing substantial parts of the company-owned product through later workflow generations, deployment, and operations.

## Breadth with a product reason

- **React and TypeScript:** conversational and table-based review flows, evidence previews, hydration, recovery, billing, progress, conflicts, and readiness.
- **Python and FastAPI:** authentication, uploads, parsing, voice, sketches, AI workflows, billing, and third-party integration APIs.
- **PostgreSQL and S3:** durable workflow state, artifacts, provenance, revisions, migrations, cleanup, and recovery.
- **Queues and workers:** SQS/Lambda and Redis/database-backed jobs for long-running work, retries, progress, leases, and restart recovery.
- **AWS operations:** Docker, ECR, ECS/Fargate, ALB, RDS, S3/CloudFront, Route 53/ACM, ElastiCache, CloudWatch, SNS, IAM, CloudTrail, and GuardDuty.
- **Commercial and vendor boundaries:** Stripe subscriptions and entitlements plus authenticated, stateful external delivery.

## Operational problems I worked through

- ALB listener, target-health, security-group, and service-port failures
- RDS access and migration-startup problems
- stale ECS task revisions and missing environment injection
- frontend builds containing localhost and stale CDN or service-worker assets
- DNS, TLS, dependency, and Lambda packaging constraints
- database and object-storage cleanup failures

## Important boundary

The approximately five-week milestone was the first working vertical slice, not a completed commercial product. The evidence demonstrates broad early-stage execution, not sole authorship, product ownership, verified adoption, or measured scale.

## Public proof

- [Professional case study](https://varsha-ai.notion.site/From-Messy-Evidence-to-Controlled-Action-Applied-AI-Engineering-Case-Study-3d006085ac208097a192dd7b776dd685)
- [Commerce Action Reliability Lab](https://github.com/VarshaThondalapally/commerce-action-reliability-lab)
- [Live reviewer demo](https://varshathondalapally.github.io/commerce-action-reliability-lab/)

[Back to profile](../README.md)
