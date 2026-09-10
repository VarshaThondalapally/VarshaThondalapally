# Multimodal and Document AI

## The hiring case

I have built AI workflows where the input was not one clean text prompt. Evidence arrived as photographs, image crops, multi-page PDFs, existing estimate packages, DOCX, text, Markdown, CSV, sketches, measurements, room notes, structured intake, and audio.

The core engineering problem was preserving identity and provenance while routing each modality through the appropriate extraction or reasoning path.

## Technical decisions I implemented

- Rendered and processed multi-page documents while retaining source, filename, page, room, and upload identity.
- Added image, crop, sketch, OCR-fallback, document-parser, and Whisper transcription paths instead of flattening every input into one prompt.
- Routed lighter extraction and heavier document reasoning through different OpenAI and Gemini paths with structured outputs.
- Bound extracted and generated proposals to the source evidence that produced them.
- Isolated named sections, rooms, and shared tables and handled duplicate or conflicting extraction through review instead of silent overwrite.
- Preserved accepted measurements and state when a later extraction failed.
- Stored binary artifacts in S3 and operational relationships in PostgreSQL, with presigned access and exact-key cleanup.

## What this demonstrates

- Multimodal foundation-model orchestration
- Document intelligence and page-aware provenance
- OCR and speech-to-text integration
- Schema-constrained extraction
- Source-aware review and failure handling
- Storage and lifecycle design for large artifacts

## Important boundary

This work used foundation-model and document-processing capabilities. It does not support a claim that I trained a proprietary vision classifier or measured production extraction accuracy.

## Public proof

- [Recipe Review Evidence Pipeline](https://github.com/VarshaThondalapally/recipe-review-evidence-pipeline): attributed evidence, strict extraction contracts, and measured review-level evaluation
- [Professional case study](https://varsha-ai.notion.site/From-Messy-Evidence-to-Controlled-Action-Applied-AI-Engineering-Case-Study-3d006085ac208097a192dd7b776dd685)

[Back to profile](../README.md)
