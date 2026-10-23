# Anix Lynch — Applied AI Builder

### I build AI systems that survive contact with real operations.

Most AI demos stop when the model produces an answer. I build the layers that
make the answer useful: trusted data, evidence retrieval, attention routing,
safety gates, durable actions, evaluation, and human handoff.

```text
Truth → Context → Signals → Decisions → Actions → Adoption
```

My work sits where **AI engineering, data platforms, and business operations**
meet. I turn ambiguous workflows into systems that can be tested, deployed,
observed, and handed to the people who must trust them.

**Los Angeles, CA** · Python · SQL · GCP · AWS · Azure · RAG · Agents · Data Platforms

[Portfolio](https://gozeroshot.dev) · [Proof of Work](https://gozeroshot.dev/projects) · [LinkedIn](https://linkedin.com/in/anixlynch) · [Medium](https://medium.com/@anixlynch)

---

## Start Here

### 1. [Signal-First AI Platform](https://github.com/anix-lynch/healthcare-signal-platform)

**The problem:** Sending every record to an LLM is expensive, noisy, and impossible to prioritize.

**What I built:** A signal layer that scores openFDA reports before the model spends a token. Anomaly detection, clustering, classification, ranking, and lookalike retrieval decide what deserves attention first.

**Proof:** Evaluated on **5,000 real openFDA reports**. The router cuts **30% of LLM calls while preserving 95.4% serious-case recall**.

### 2. [Healthcare AI Data Platform](https://github.com/anix-lynch/healthcare-ai-data-engineer)

**The problem:** AI cannot be trustworthy when bad rows, stale timestamps, duplicate identities, and unreconciled metrics reach the model first.

**What I built:** A trust layer spanning ingestion, quarantine, entity resolution, dbt/BigQuery models, semantic profiles, retrieval, fault injection, and AI-spend governance.

**Proof:** **55.5K records** through a layered data platform, with quality controls that stop invalid data before it reaches AI-facing endpoints.

### 3. [Baymax ER Nurse Assistant](https://github.com/anix-lynch/healthcare-genai-engineer)

**The problem:** A recommendation is not an outcome. Someone must own the task, unsafe uncertainty must stop, duplicate actions must be prevented, and downstream state must be verified.

**What I built:** A trace-backed healthcare agent simulation that moves from intake to evidence, disposition, human review or bounded tool action, and an outcome receipt.

**Proof:** **50/50 labelled agent scenarios**, **100% action-safety floors**, and **5/5 rollout gates** in the current public showcase.

### 4. [Healthcare Forward Deployed Engineer](https://github.com/anix-lynch/healthcare-forward-deployed-engineer)

**The problem:** Working code is not a deployable solution if the customer cannot integrate, operate, evaluate, and own it.

**What I built:** The handoff layer around an AI workflow: discovery, contracts, acceptance gates, human review, observability, runbooks, and deployment ownership.

**Proof:** **21 acceptance tests** covering the customer-facing delivery contract.

---

## The System I Keep Building

```text
Raw sources
    ↓
Trusted data contracts
    ↓
Agent-readable context
    ↓
Signals that allocate attention
    ↓
Grounded AI decisions
    ↓
Human approval or bounded action
    ↓
Verified outcome + audit receipt
```

I care about the seams between these layers:

- Can the source be traced and reconciled?
- Does new evidence actually change the decision?
- What is probabilistic, and what must remain deterministic?
- Who owns the task when the model stops?
- Can the system detect false success instead of trusting a green message?
- Can another engineer or business team operate it after handoff?

That is the difference between an AI feature and an AI operating system.

---

## Selected Builds

| Build | What it proves |
|---|---|
| [Healthcare Analytics on Microsoft Fabric](https://github.com/anix-lynch/healthcare-da) | Code-first Fabric, OneLake, Power BI, DAX, and reconciliation against the cloud data layer |
| [Multicloud Portability](https://gozeroshot.dev/projects/healthcare-multicloud-portability) | One data contract across GCP, Microsoft Fabric, and AWS without changing the underlying truth |
| [Pied Piper Legal Simulator](https://gozeroshot.dev/projects/pied-piper-legal) | Grounded GenAI applied to term sheets, clause-level citations, and venture/startup analysis |
| [Realtime Fraud Detection](https://github.com/anix-lynch/realtime-fraud-detection) | Streaming features, freshness checks, leakage control, and low-latency risk scoring |
| [MocktailVerse Bedrock](https://gozeroshot.dev/projects/mocktailverse-bedrock) | AWS Bedrock RAG with Claude, Titan embeddings, and pgvector retrieval |

---

## My Domain Edge

Before becoming a hands-on AI builder, I worked as a **VC/GP, investment
professional, and operator**. I screened more than **700 startups** and worked
across diligence, portfolio support, corporate innovation, and operating teams.

That background changes how I build:

- I begin with the decision and workflow, not the model demo.
- I translate between executives, domain experts, data teams, and engineers.
- I treat evidence, ownership, failure modes, and adoption as product requirements.
- I know that a technically correct system can still fail if nobody trusts or owns it.

[Pied Piper Legal Simulator](https://gozeroshot.dev/projects/pied-piper-legal)
is one example: grounded GenAI meets term-sheet analysis and venture-domain
judgment. The value is not merely extracting a clause. It is helping a human
understand what the clause changes, who it favors, and what deserves scrutiny.

---

## How I Build

- **Evidence before confidence** — citations, data lineage, reconciliation, and evaluation.
- **Signals before expensive reasoning** — spend model attention where it changes the outcome.
- **Brakes before autonomy** — human review, bounded retries, idempotency, and escalation.
- **Receipts before celebration** — verify durable state instead of trusting “success.”
- **Handoff before heroics** — runbooks, contracts, observability, and clear ownership.

Core tools include **Python, SQL, FastAPI, BigQuery, dbt, Microsoft Fabric,
Power BI, Vertex AI, Gemini, AWS Bedrock, Docker, GitHub Actions, retrieval and
evaluation frameworks**. The complete proof-backed inventory lives in
[tech-stack.md](./tech-stack.md); this page is about the systems, not the keyword pile.

---

## What I Am Looking For

I am most useful on teams turning AI ambition into operational systems:

- applied AI and agent workflows
- AI/data platform engineering
- enterprise AI enablement and citizen-development guardrails
- forward-deployed and solutions engineering
- investment, financial-services, healthcare, and other evidence-sensitive domains

I like collaborating on challenges that require moving comfortably between
business context and system behavior—inspecting data, designing control planes,
building services, evaluating outcomes, and making tradeoffs legible to everyone
involved.

**MBA, University of Chicago Booth** · **JLPT N1** · **Authorized to work in the US**
