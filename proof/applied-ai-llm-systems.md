# Applied AI and LLM Systems

## The hiring case

I build the product and control layers around foundation models. My strongest work is not a single prompt or SDK call; it is deciding what a model may interpret, what must be grounded in evidence, and what application code or a person must authorize.

At Roitech, I developed substantial parts of a company-owned vertical-AI workflow as employee #1 and the only full-time engineer. The system processed multimodal evidence, retrieved domain knowledge and catalog candidates, produced typed proposals, preserved provenance, and required review before downstream action.

## Technical decisions I implemented

- Replaced simulated and overly broad retrieval with OpenAI embeddings, FAISS, four evidence views, cosine scoring, domain-aware reranking, thresholds, review-history signals, and exact catalog resolution.
- Restricted model selection to admissible candidates and converted OpenAI and Gemini responses into JSON-schema and Pydantic-validated operations.
- Routed OpenAI, Gemini Flash/Pro, vision-capable paths, embeddings, and Whisper by modality, context, response shape, latency, and cost constraints.
- Added provider-specific timeout and transient-error handling, exponential backoff with jitter, batching, input deduplication, prompt and embedding caches, provider cached content, and fallback behavior.
- Preserved source, page, room, and measurement lineage so reviewers could inspect why a proposal existed.
- Kept external execution behind deterministic validation, current-state checks, entitlement, and revision-bound human approval.

## What this demonstrates

- Production LLM application engineering
- Hybrid retrieval and domain-aware reranking
- Structured generation and model-to-application contracts
- Multimodal orchestration and evidence grounding
- Human-in-the-loop guardrails
- Model latency, token, cache, status, and error instrumentation

## Important boundary

This is foundation-model integration and control, not proprietary model training, fine-tuning, classical ML research, or GPU inference engineering. The implementation did not produce a controlled benchmark proving one provider was universally best.

## Public proof

- [Commerce Action Reliability Lab](https://github.com/VarshaThondalapally/commerce-action-reliability-lab)
- [Live reviewer demo](https://varshathondalapally.github.io/commerce-action-reliability-lab/)
- [Professional case study](https://varsha-ai.notion.site/From-Messy-Evidence-to-Controlled-Action-Applied-AI-Engineering-Case-Study-3d006085ac208097a192dd7b776dd685)

[Back to profile](../README.md)
