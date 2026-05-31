# Anix Lynch — AI Platform / GenAI Engineer

**I build the trust-to-action stack: trusted data → features → evaluated signals → agent actions → accountable human decisions.**
Live, evaluated systems on Cloud Run + Vertex AI — not demos. Ex-VC / family-office operator, so I also own the layer most engineers skip: getting executives to actually *adopt* the AI.

🌐 [gozeroshot.dev](https://gozeroshot.dev) · 💼 [linkedin.com/in/anixlynch](https://linkedin.com/in/anixlynch)

---

## The architecture I build across (L1 → L3)

| Layer | Question | Live project | Proof |
|-------|----------|--------------|-------|
| **L1 Truth** | *Can we trust the data?* | [healthcare-ai-data-engineer](https://github.com/anix-lynch/healthcare-ai-data-engineer) | dbt medallion on BigQuery · **55 tests green** · quality gate · PII masking |
| **L1.25 Context** | *How should AI agents see it?* | ↳ same repo (**Feast** feature store) | point-in-time-correct patient features |
| **L1.5 Signals** ★ | *What might happen?* | [healthcare-signal-platform](https://github.com/anix-lynch/healthcare-signal-platform) | 5 evaluated signals → agent · anomaly **F1 0.85** · cluster silhouette 0.41 (535/40K) · classify ±1-tier **100%** |
| **L2 Action** | *What should the agent do?* | [healthcare-genai-engineer](https://github.com/anix-lynch/healthcare-genai-engineer) | RAG · BM25+dense+RRF · PII guardrails · **CI eval gate** |
| **L3 Influence** | *Will humans adopt it?* | [healthcare-forward-deployed-engineer](https://github.com/anix-lynch/healthcare-forward-deployed-engineer) | VPC deploy · runbook · postmortems · human Approve/Override |

**★ The flagship proves it:** the [live Signal Console](https://signal-console-819957310168.us-west1.run.app) runs an **ablation** — the same Gemini agent decides *with* the signals vs *without*. On the ops-capacity case the call visibly flips **WATCH → ACT NOW**. Signals change the decision; they don't just decorate it. Evals tracked in [Weights & Biases](https://wandb.ai/alynch-zeroshot/healthcare-l15-signals), agent calls traced in Langfuse.

---

## Why the whole chain (not one layer)

Most engineers stop at L2. Most executives start at L3. **Few people understand the entire chain** — Truth → Context → Signals → Actions → Human adoption. That's the rare part, and it's where 10 years of VC / family-office / CEO-office translation (tech ↔ business ↔ stakeholder) becomes a moat.

---

## Stack
**AI/Platform:** Vertex AI · Gemini · Signal Intelligence · Decision Intelligence · Feature Stores (Feast) · anomaly/cluster/classify/rank
**GenAI:** RAG · hybrid retrieval (BM25/dense/RRF) · agents · tool calling · guardrails · LLM eval · vector search (Chroma/Pinecone/Qdrant)
**Data:** dbt · BigQuery · analytics engineering · medallion · data contracts · governance · Snowflake · DuckDB · Microsoft Fabric · Power BI
**Cloud/Infra:** GCP · Cloud Run · AWS Bedrock · Azure · Docker · FastAPI · GitHub Actions
**Eval/Obs:** Weights & Biases · Langfuse · Ragas-style eval · CI regression gates
**Languages:** Python · SQL

*MBA, University of Chicago Booth · JLPT N1 · Authorized to work in the US (Green Card)*
