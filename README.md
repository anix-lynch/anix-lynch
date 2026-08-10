# Anix Lynch - AI/Data Engineer · Los Angeles

**Applied AI engineer building RAG, agent, and data-platform systems that can be evaluated, deployed, and handed to humans safely.**

I build the trust-to-action stack:

`Trusted Data -> Retrieval -> Signals -> Agent Actions -> Evals/Telemetry -> Human Adoption`

Live, evaluated systems on Cloud Run + Vertex AI, with the data backbone,
quality gates, retrieval layer, eval harness, observability, and adoption loop
around the model.

Los Angeles, CA · Python · SQL · GCP · AWS · Azure · dbt · Vertex AI · RAG · Agents

[Portfolio](https://gozeroshot.dev) · [LinkedIn](https://linkedin.com/in/anixlynch) · [Bluesky](https://bsky.app/profile/anixlynch.bsky.social) · [YouTube](https://youtube.com/@anix_lynch) · [Medium](https://medium.com/@anixlynch)

---

## What I Build

- **RAG systems:** hybrid retrieval, citations, grounding checks, vector search, and eval gates.
- **AI agents:** LangGraph-style workflows, tool calling, bounded actions, safety brakes, and human review.
- **AI data platforms:** dbt/BigQuery/Fabric data layers, quality gates, contracts, semantic layers, and agent-readable APIs.
- **Evaluation + telemetry:** Ragas-style evals, regression gates, Langfuse, Weights & Biases, OpenTelemetry, logs, and cost tracking.
- **Cloud deployment:** FastAPI services on Cloud Run/Vercel/AWS patterns with Docker, GitHub Actions, and scale-to-zero cost discipline.

## Architecture Proof (L1 -> L3)

| Layer | Question | Live project | Proof |
|-------|----------|--------------|-------|
| **L1 Truth** | Can we trust the data? | [healthcare-ai-data-engineer](https://github.com/anix-lynch/healthcare-ai-data-engineer) | dbt medallion on BigQuery · **55 tests green** · quality gate · PII masking |
| **L1.25 Context** | How should AI agents see it? | same repo, **Feast** feature store | point-in-time-correct patient features |
| **L1.5 Signals** | What might happen? | [healthcare-signal-platform](https://github.com/anix-lynch/healthcare-signal-platform) | 5 evaluated signals -> agent · anomaly **F1 0.85** · classify +/-1-tier **100%** |
| **L2 Action** | What should the agent do? | [healthcare-genai-engineer](https://github.com/anix-lynch/healthcare-genai-engineer) | RAG · BM25+dense+RRF · PII guardrails · **CI eval gate** |
| **L3 Adoption** | Will humans use it? | [healthcare-forward-deployed-engineer](https://github.com/anix-lynch/healthcare-forward-deployed-engineer) | LangGraph/FastAPI handoff · runbook · OpenTelemetry · Approve/Override |

The flagship [Signal Console](https://signal-console-819957310168.us-west1.run.app) runs an ablation: the same Gemini agent decides with signals vs. without signals. On the ops-capacity case, the call visibly flips **WATCH -> ACT NOW**. Evals are tracked in [Weights & Biases](https://wandb.ai/alynch-zeroshot/healthcare-l15-signals), and agent calls are traced in Langfuse.

## Production Proof

- **0.97 Ragas faithfulness** on a RAG pipeline evaluation.
- **0.85 anomaly F1** on a signal platform that routes cases before the LLM spends tokens.
- **21 acceptance tests** for a healthcare forward-deployed AI handoff layer.
- **100% action-safety floors** across 50 Baymax ER agent scenarios.
- **55/55 dbt tests green** on a healthcare AI data-engineering stack.
- **$1-2/month serverless runtime** pattern for low-traffic production AI demos.

## Other Public Proof

- [AI Agent Job Intelligence](https://github.com/anix-lynch/ai-agent-job-intelligence-phase-2) - resume-aware multi-agent system with semantic search, ATS scoring, and 14 MCP tools.
- [Healthcare Analytics on Microsoft Fabric](https://github.com/anix-lynch/healthcare-da) - code-reviewed Power BI semantic model, Fabric REST deployment, and openFDA counts reconciled against the cloud data layer.
- [Realtime Fraud Detection](https://github.com/anix-lynch/realtime-fraud-detection) - streaming risk-scoring surface with feature freshness checks, sub-ms scoring path, and data quality gates.

## Stack

- **Languages:** Python, SQL, TypeScript, Bash
- **AI + Agents:** RAG, LangGraph, LangChain, MCP, tool calling, guardrails, eval harnesses
- **Retrieval:** BM25, hybrid retrieval, semantic search, pgvector, ChromaDB, Pinecone, Qdrant
- **Data:** dbt, BigQuery, Microsoft Fabric/OneLake, DuckDB, Snowflake, Feast, Great Expectations
- **Eval + Telemetry:** Ragas-style evals, Langfuse, Weights & Biases, OpenTelemetry, MLflow, CI regression gates
- **Cloud + App:** GCP Cloud Run/Vertex AI/Gemini, AWS Bedrock, Azure/Fabric, FastAPI, Docker, GitHub Actions
- **BI + Analytics:** Power BI, DAX, Direct Lake, TMDL, semantic models, governed dashboards

## Background

Ex-VC/GP and operator turned applied AI engineer. I have screened 700+ startups,
worked across investment and operating teams, and now build the AI/data systems I
used to wish existed during diligence, portfolio support, and enterprise adoption.

MBA, University of Chicago Booth · JLPT N1 · Authorized to work in the US
