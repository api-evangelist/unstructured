# Unstructured (unstructured)

Unstructured is a document parsing and pre-processing platform that provides a REST API for ingesting PDFs, HTML, DOCX, images, and more than 50 other file formats, transforming them into clean structured JSON chunks ready for RAG pipelines and LLM applications. The platform offers partitioning, enrichment, chunking, and embedding capabilities via a SaaS serverless API, dedicated instances, and in-VPC deployments. It ships Python and JavaScript SDKs, an MCP server for AI agent workflows, and 40+ connectors for source and destination data systems.

APIs.json: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/apis.yml

Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=unstructured-api-evangelist&utm_content=repo

## Tags

- document-processing
- ETL
- RAG
- LLM
- PDF
- OCR
- data-ingestion
- chunking
- embeddings
- AI

## APIs

### Unstructured Platform API

The Unstructured Platform API provides programmatic access to workflow operations including source connectors, destination connectors, workflows, and jobs. It enables headless, push-style data transformation pipelines that partition, enrich, chunk, and embed documents from 50+ file formats into AI-ready JSON.

- Human URL: https://docs.unstructured.io/api-reference/overview
- Base URL: https://platform.unstructuredapp.io/api/v1

### Unstructured Partition Endpoint

The Unstructured Partition Endpoint is the legacy serverless API for processing individual files on demand. It supports PDFs, images, DOCX, HTML, and dozens of other formats, returning structured element JSON with configurable processing strategies (fast, hi_res, ocr_only, auto).

- Human URL: https://docs.unstructured.io/api-reference/api-services/saas-api-development-guide
- Base URL: https://api.unstructured.io/general/v0/general

## Plans / Rate Limits / FinOps

- Plans: [plans/unstructured-plans-pricing.yml](plans/unstructured-plans-pricing.yml)
- Rate Limits: [rate-limits/unstructured-rate-limits.yml](rate-limits/unstructured-rate-limits.yml)
- FinOps: [finops/unstructured-finops.yml](finops/unstructured-finops.yml)

### Pricing Summary

| Plan | Price | Pages |
|------|-------|-------|
| Let's Go (Free) | $0 | 15,000 lifetime |
| Pay-As-You-Go | $0.03/page | Unlimited |
| Business | Custom | Custom |

### Rate Limits

Unstructured does not publish explicit rate limit values in public documentation. The SDK uses exponential backoff retry logic (initial 500ms, max 1 minute, max 1 hour elapsed). The `split_pdf_concurrency_level` parameter is capped at 15 per request. Contact support@unstructured.io for plan-specific limits.

## Timestamps

- Created: 2026-06-12
- Modified: 2026-06-12

## Common Properties

| Type | URL |
|------|-----|
| Website | https://unstructured.io |
| Documentation | https://docs.unstructured.io |
| GitHub Organization | https://github.com/Unstructured-IO |
| LinkedIn | https://www.linkedin.com/company/unstructuredio/ |
| X / Twitter | https://twitter.com/UnstructuredIO |
| Blog | https://unstructured.io/blog |
| Pricing | https://unstructured.io/pricing |
| Status Page | https://unstructuredio.trust.pagerduty.com/posts/dashboard |
| Python SDK | https://github.com/Unstructured-IO/unstructured-python-client |
| JavaScript SDK | https://github.com/Unstructured-IO/unstructured-js-client |
| MCP Server | https://github.com/Unstructured-IO/UNS-MCP |

## Maintainers

- Kin Lane / kin@apievangelist.com
