<div align="center">

# 🎓 EduMorph

### Self-Improving Learning Intelligence Platform

> Every student who learns makes the next student's experience better — automatically.

![Next.js](https://img.shields.io/badge/Next.js-14-black?style=flat-square&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=flat-square&logo=typescript)
![Azure](https://img.shields.io/badge/Azure-5%20Services-0078D4?style=flat-square&logo=microsoft-azure)
![Power BI](https://img.shields.io/badge/Power%20BI-Analytics-F2C811?style=flat-square&logo=powerbi)
![Groq](https://img.shields.io/badge/Groq-Llama%203.3%2070B-orange?style=flat-square)
![Vercel](https://img.shields.io/badge/Deployed-Vercel-black?style=flat-square&logo=vercel)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

<br/>

![Edumorph Cover](edumorph_cover.png)

<br/>

---

### 👤 Built by

**Brijesh Kumar**
📞 623-666-2665 · 📧 [bkumar25@asu.edu](mailto:bkumar25@asu.edu) · 💼 [linkedin.com/in/brijeshkumar03](https://linkedin.com/in/brijeshkumar03) · 🐙 [github.com/Brijesh03032001](https://github.com/Brijesh03032001) · 📍 Tempe, AZ · ✅ Open to CPT / OPT

---

</div>

## 📌 Description

**EduMorph** is a full-stack, cloud-native adaptive learning platform that combines **Generative AI**, **real-time big data pipelines**, and **interactive BI dashboards** to create a self-improving educational experience.

A student pastes any concept or lecture text — EduMorph instantly generates multiple teaching formats (analogies, diagrams, explainer videos, quizzes) tailored to how that concept is best understood. Every interaction is captured as a telemetry event, streamed through an **Azure Event Hubs → Stream Analytics → Data Lake Gen2 → Synapse Analytics** pipeline, and visualized in **Power BI** dashboards. **Azure OpenAI (GPT-4o)** then analyzes the aggregated data to generate targeted adaptation strategies — so the next learner automatically gets a smarter, better-tuned explanation.

**The system learns from learners. Teaching improves automatically. No instructor intervention required.**

Key highlights:
- 🔁 **Closed feedback loop** — student behavior drives content improvement in real time
- 📊 **Power BI dashboards** — concept difficulty, format effectiveness, engagement trends visualized end-to-end
- ☁️ **5 Azure services** — Event Hubs, Stream Analytics, Data Lake Gen2, Synapse Analytics, Azure OpenAI
- ⚡ **Groq / Llama 3.3 70B** — sub-second multi-format content generation
- 🏗️ **Production-grade DevOps** — CI/CD via Vercel, environment-based config, pnpm workspaces, TypeScript strict mode

---

## 🏷️ Topics

`adaptive-learning` `edtech` `generative-ai` `llm` `groq` `llama` `azure` `azure-openai` `azure-event-hubs` `azure-stream-analytics` `azure-data-lake` `azure-synapse-analytics` `power-bi` `big-data` `real-time-analytics` `data-pipeline` `data-visualization` `nextjs` `typescript` `react` `tailwindcss` `zustand` `recharts` `vercel` `ci-cd` `devops` `cloud-native` `infrastructure-as-code` `event-driven-architecture` `telemetry` `student-analytics` `open-to-cpt` `open-to-opt`

---

## ❓ What is EduMorph?

EduMorph is an AI-powered adaptive learning platform. A student pastes any concept or lecture text, and EduMorph instantly generates multiple teaching formats — analogies, step-by-step diagrams, explainer videos, and quizzes — tailored for how that concept is best understood.

What makes EduMorph different from a content generator is the **feedback loop**. Every interaction a student has — a quiz score, a video pause, a "make it simpler" click — is captured as a telemetry event, streamed into an Azure data pipeline, and analyzed to detect where learners consistently struggle. Azure OpenAI then generates targeted adaptation strategies. The next learner gets a better, smarter explanation — without any manual instructor intervention.

**The system learns from learners. Teaching improves automatically.**

---

## 🚨 The Problem

Traditional digital learning platforms are static by design:

| Platform | How it adapts |
|---|---|
| Khan Academy | It doesn't — same video for everyone |
| Duolingo | Rule-based: if wrong, show easier content |
| Coursera | Instructor manually updates content every few months |

There is no system that closes the loop between **what students struggle with** and **how the explanation gets better** — in real time, at scale, without human intervention.

---

## ✅ How EduMorph Solves It

EduMorph is built around a closed feedback loop powered by Azure:

```
Input Concept
     │
     ▼
Content Generation (Groq / Llama 3.3 70B)
     │
     ├── Analogy
     ├── Step-by-Step Diagram
     ├── Explainer Video
     └── Adaptive Quiz
           │
           ▼
     Student Interacts
           │
           ▼
  Telemetry Events Captured
  (quiz score · video drop-off · feedback · regeneration clicks)
           │
           ▼
  Azure Event Hubs  ──▶  Azure Stream Analytics  ──▶  Azure Data Lake Gen2
                                                              │
                                                              ▼
                                                  Azure Synapse Analytics
                                                  (concept difficulty · format effectiveness)
                                                              │
                                                              ▼
                                                    Azure OpenAI (GPT-4o)
                                                  generates adaptation strategy
                                                              │
                                                              ▼
                                               Groq regenerates improved content
                                                              │
                                                              ▼
                                              Next learner gets a better explanation
```

---

## 🏗️ Architecture

### Layers

| Layer | Technology | Responsibility |
|---|---|---|
| Frontend | Next.js 14 App Router, React 18, TypeScript | UI, interaction capture, event batching |
| API | Next.js Route Handlers | Content generation, telemetry ingestion, analytics export |
| Event Streaming | Azure Event Hubs | Ingests 1000+ learning events/sec in real time |
| Processing | Azure Stream Analytics | Enriches and routes events |
| Storage | Azure Data Lake Gen2 | Petabyte-scale telemetry store, partitioned by date and concept |
| Analytics | Azure Synapse Analytics | SQL queries on difficulty, engagement, and format effectiveness |
| BI & Visualization | Power BI | Interactive dashboards connected to Synapse for stakeholder reporting |
| Adaptation | Azure OpenAI (GPT-4o) | Generates teaching improvement strategies from analytics insights |
| Content AI | Groq (Llama 3.3 70B) | Fast multi-format teaching content generation |
| Deployment | Vercel + GitHub CI/CD | Automated build, preview, and production deployments |

### Azure Services Used

- **Azure Event Hubs** — real-time event ingestion at scale
- **Azure Stream Analytics** — stateless event processing and routing
- **Azure Data Lake Gen2** — durable, queryable telemetry storage
- **Azure Synapse Analytics** — SQL-based learning behavior analysis
- **Azure OpenAI** — adaptive teaching recommendations

---

## 📊 Power BI & Big Data

EduMorph is built with enterprise-grade data visualization and big data processing at its core:

- **Power BI Dashboards** — connected directly to Azure Synapse Analytics via DirectQuery, providing live views of concept difficulty scores, format effectiveness rates, student engagement trends, and cohort-level performance comparisons
- **Big Data Pipeline** — telemetry events flow through Event Hubs at 1000+ events/sec, processed by Stream Analytics, and stored in a partitioned Data Lake Gen2 — designed to scale to millions of learners
- **Exportable Datasets** — CSV and JSON exports from `/api/export-data` feed directly into Power BI Desktop or any BI tool
- **Synapse SQL Analytics** — pre-built queries for concept difficulty ranking, format effectiveness scoring, and engagement funnel analysis (see [`docs/synapse-queries.sql`](docs/synapse-queries.sql))
- **Real-time Metrics** — in-app Recharts dashboards mirror the Power BI views for instant feedback without leaving the platform

---

## ⚙️ DevOps & Infrastructure

| Practice | Implementation |
|---|---|
| CI/CD | Vercel Git integration — auto-deploy on every push to `main` |
| Preview Environments | Vercel preview URLs on every pull request |
| Environment Config | `.env.local` with strict separation of dev / prod secrets |
| Package Management | pnpm workspaces for fast, deterministic installs |
| Type Safety | TypeScript strict mode across all layers |
| Schema Validation | Zod for all AI input/output contracts |
| Linting | ESLint + Next.js recommended config |
| Build Optimization | Next.js App Router with server components and edge-ready API routes |
| Monitoring | Azure Monitor + custom telemetry health endpoint (`/api/telemetry`) |

---

## ✨ Key Features

- **Multi-format generation** — one input, four teaching outputs (analogy, diagram, video, quiz)
- **Real-time telemetry** — every interaction streamed to Azure in under 1 second
- **Adaptive content** — AI-generated improvement strategies applied at regeneration time
- **Power BI integration** — live dashboards connected to Synapse for deep learning analytics
- **Learning analytics dashboard** — concept difficulty, format effectiveness, engagement trends
- **Student progress tracking** — per-session performance and historical trends
- **Exportable datasets** — CSV and JSON exports for Power BI and external BI tools
- **Gamification layer** — streaks, badges, and points to sustain engagement
- **Big data ready** — pipeline designed to scale to millions of concurrent learners

---

## 🛠️ Tech Stack

### Frontend
- Next.js 14 (App Router)
- React 18 · TypeScript · Tailwind CSS
- Zustand (state management)
- Recharts (in-app analytics visualisation)

### AI
- Groq API — Llama 3.3 70B — primary content generation
- Azure OpenAI — GPT-4o — adaptive teaching strategies
- Zod — schema validation for all AI I/O

### Cloud & Big Data
- Azure Event Hubs · Azure Stream Analytics
- Azure Data Lake Gen2 · Azure Synapse Analytics
- Azure OpenAI Service

### Visualization & BI
- Power BI (DirectQuery to Synapse)
- Recharts (in-app dashboards)
- CSV / JSON data exports

### DevOps & Infrastructure
- Vercel (CI/CD + deployment)
- GitHub (version control + PR previews)
- pnpm (package management)
- ESLint · TypeScript strict mode
- Azure Monitor (observability)

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- pnpm
- Groq API key ([console.groq.com](https://console.groq.com))
- Azure Event Hubs + Azure OpenAI resource

### 1. Clone and Install

```bash
git clone https://github.com/Brijesh03032001/eduMorph.git
cd eduMorph
pnpm install
```

### 2. Configure Environment

Create `.env.local` in the project root:

```env
# Groq (required for content generation)
GROQ_API_KEY=your_groq_api_key

# Azure Event Hubs (required for telemetry)
AZURE_EVENTHUB_CONNECTION_STRING=your_connection_string
AZURE_EVENTHUB_NAME=edumorph-learning-events

# Azure OpenAI (required for adaptive teaching)
AZURE_OPENAI_ENDPOINT=https://your-resource.openai.azure.com/
AZURE_OPENAI_API_KEY=your_api_key
AZURE_OPENAI_DEPLOYMENT_NAME=gpt-4o
```

### 3. Run

```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000)

Check telemetry: [http://localhost:3000/api/telemetry](http://localhost:3000/api/telemetry)

---

## 📁 Project Structure

```
edumorph/
├── app/
│   ├── page.tsx                      # Landing page
│   ├── studio/page.tsx               # Teaching studio
│   ├── analytics/page.tsx            # Analytics dashboard
│   ├── student-dashboard/page.tsx    # Student view
│   └── api/
│       ├── generate/route.ts         # Content generation (Groq)
│       ├── generate/quiz/route.ts    # Quiz generation
│       ├── telemetry/route.ts        # Event ingestion (Azure)
│       ├── analytics/route.ts        # Analytics API
│       ├── student-analytics/route.ts
│       └── export-data/route.ts      # Dataset exports (Power BI ready)
├── components/
│   ├── InputCard.tsx                 # Lecture input
│   ├── ResultTabs.tsx                # Teaching format tabs
│   ├── ExplainerVideo.tsx            # Video + engagement telemetry
│   ├── QuizBlock.tsx                 # Quiz + score telemetry
│   ├── FeedbackBlock.tsx             # Feedback + telemetry
│   └── analytics/                   # Power BI-style dashboard charts
├── lib/
│   ├── groq.ts                       # Groq API client
│   ├── telemetry.ts                  # Event schema and batcher
│   ├── schema.ts                     # Zod validation schemas
│   └── azure/
│       ├── eventHubs.ts              # Event Hubs client
│       └── adaptiveTeaching.ts       # Azure OpenAI integration
└── docs/
    ├── AZURE_ARCHITECTURE.md         # Full Azure documentation
    ├── QUICK_START.md                # Step-by-step Azure setup
    ├── synapse-queries.sql           # Analytics SQL queries
    └── POWERBI_SETUP.md             # Power BI dashboard setup guide
```

---

## 📡 API Reference

| Route | Method | Purpose |
|---|---|---|
| `/api/generate` | POST | Generate multi-format teaching content |
| `/api/generate/quiz` | POST | Generate adaptive quiz questions |
| `/api/telemetry` | POST / GET | Ingest events / health check |
| `/api/analytics` | GET | Retrieve aggregated learning analytics |
| `/api/student-analytics` | GET | Per-student performance data |
| `/api/export-data` | GET | Export datasets (CSV / JSON) for Power BI |

---

## 📚 Documentation

| Document | Description |
|---|---|
| [Azure Architecture](docs/AZURE_ARCHITECTURE.md) | Complete technical architecture deep dive |
| [Quick Start Guide](docs/QUICK_START.md) | Full Azure resource setup in 30 minutes |
| [Synapse Queries](docs/synapse-queries.sql) | Analytics SQL for concept and engagement insights |
| [Power BI Setup](docs/POWERBI_SETUP.md) | Connect Synapse data to Power BI dashboards |

---

## 📄 License

MIT — see [LICENSE](LICENSE) for details.

---

<div align="center">

Built with Azure · Powered by big data · Visualized with Power BI · Improved by every student.

<br/>

**Brijesh Kumar** · 📞 623-666-2665 · 📧 [bkumar25@asu.edu](mailto:bkumar25@asu.edu) · [LinkedIn](https://linkedin.com/in/brijeshkumar03) · [GitHub](https://github.com/Brijesh03032001) · Tempe, AZ · Open to CPT / OPT

</div>
