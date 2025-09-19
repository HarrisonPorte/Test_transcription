# Tree Map: Test_transcription Workstreams

## 1. Repository Structure Overview
```
Test_transcription/
├── docs/
│   ├── README.md
│   ├── SOP.md
│   ├── delivery-roadmap.md
│   └── tree-map.md
├── (planned) backend/
│   ├── app/
│   │   ├── __init__.py
│   │   ├── main.py
│   │   ├── routes/
│   │   │   ├── transcription.py
│   │   │   ├── summaries.py
│   │   │   ├── webhooks.py
│   │   │   └── exports.py
│   │   ├── models.py
│   │   └── services/
│   │       ├── job_manager.py
│   │       └── storage_adapter.py
│   └── tests/
│       ├── __init__.py
│       ├── test_transcription_flow.py
│       └── test_summary_generation.py
├── (planned) services/
│   ├── transcription/
│   │   ├── __init__.py
│   │   ├── ingestor.py
│   │   ├── provider_client.py
│   │   └── workers.py
│   └── summarization/
│       ├── __init__.py
│       ├── generator.py
│       ├── templates/
│       │   ├── executive.md
│       │   ├── bullets.md
│       │   └── action-items.md
│       └── evaluators.py
├── (planned) infra/
│   ├── terraform/
│   │   ├── main.tf
│   │   ├── storage.tf
│   │   ├── queue.tf
│   │   ├── worker.tf
│   │   ├── api-gateway.tf
│   │   ├── secrets.tf
│   │   ├── logging.tf
│   │   └── iam.tf
│   └── cdn/
│       └── config.yaml
├── (planned) monitoring/
│   ├── prometheus.yml
│   └── alerts/
│       ├── queue_backlog.yaml
│       ├── cost_anomalies.yaml
│       └── sla_breach.yaml
├── (planned) ci/
│   └── github-actions/
│       ├── api-contract.yml
│       └── ops.yml
├── (planned) data/
│   ├── transcripts/
│   │   ├── README.md
│   │   └── {request-id}.json
│   └── summaries/
│       ├── {request-id}/
│       │   ├── executive.md
│       │   ├── bullets.md
│       │   └── metadata.json
├── (planned) scripts/
│   ├── evaluate_summaries.py
│   └── cost_reports.py
├── (planned) integration-tests/
│   └── test_end_to_end.py
└── (planned) frontend/
    ├── package.json
    ├── src/
    │   ├── App.tsx
    │   ├── components/
    │   └── pages/
    └── public/
```

## 2. Document Tree by Workstream
```
docs/
├── ADRs & Decisions
│   ├── adr/
│   │   └── 0001-tech-stack.md (pending)
├── Product & Design
│   ├── product-brief.md (pending)
│   ├── domain-model.md (pending)
│   ├── architecture-overview.md (pending)
│   ├── api/
│   │   └── openapi.yaml (pending)
│   └── ui/
│       └── wireframes.md (pending)
├── Operations
│   ├── SOP.md
│   ├── operations/
│   │   └── runbooks/
│   │       └── incident-response.md (pending)
│   ├── transcription/
│   │   ├── runbook.md (pending)
│   │   └── provider-comparison.md (pending)
│   ├── summarization/
│   │   ├── prompt-catalog.md (pending)
│   │   └── quality-checklist.md (pending)
│   ├── evaluation/
│   │   └── summary-benchmarking.md (pending)
│   └── delivery-roadmap.md
├── Security & Governance
│   ├── security/
│   │   └── threat-model.md (pending)
│   ├── compliance/
│   │   └── data-retention-policy.md (pending)
│   ├── data-classification.md (pending)
│   └── pii-handling.md (pending)
└── Contributor Guides
    ├── README.md
    ├── glossary.md (pending)
    ├── contributing.md (pending)
    └── code_of_conduct.md (pending)
```

## 3. Execution Checkpoints
- Use this tree map with `docs/delivery-roadmap.md` to track which assets exist and which remain placeholders.
- Update tree entries with actual filenames as components are implemented (e.g., replace `{request-id}` with real examples).
- For each new directory introduced, add a minimal `README.md` explaining its purpose to help onboard contributors.
