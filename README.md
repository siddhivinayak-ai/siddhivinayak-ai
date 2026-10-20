# Siddhivinayak Waghmode

**I build AI systems for manufacturing and industrial operations.**

I'm a manufacturing engineer (BTech, Manufacturing Science & Technology, COEP Technological University, Pune) working on agentic AI, retrieval and digital twins. I understand the shop floor and the paperwork around it: tool wear, OEE, tenders, cargo compliance and procurement. I build software that handles that work.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Siddhivinayak_Waghmode-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/siddhivinayak-waghmode-641b6b241/)
[![Email](https://img.shields.io/badge/Email-siddhivinayakwaghmode2004%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:siddhivinayakwaghmode2004@gmail.com)

**Open to:** co-founding in industrial AI or B2B automation, and AI/ML engineering roles (agentic systems, RAG, applied ML).

---

## Selected work

### [Manufacturing Copilot](https://github.com/siddhivinayak-ai/mfg-copilotv0.1)
A reasoning engine for factories. It answers maintenance, quality, energy, safety and supply-chain questions using sensor datasets, OEM manuals and regulations.
- GraphRAG over a 7-domain knowledge graph (~10,000 nodes, ~21,000 edges) built from NASA C-MAPSS, CWRU bearings, SECOM and others, plus ABB, KUKA, Siemens and UR robot manuals
- An orchestrator sends each question to one of 6 specialist agents
- Connects facts across domains: a vibration spike → the related OSHA hazard → the matching KUKA error code

`Python` `GraphRAG` `Multi-agent orchestration`

### [SV Digital Twin Labs](https://github.com/siddhivinayak-ai/SV-DigitalTwinLabs) · *in active development*
An open-source digital twin of a manufacturing production line.
- A C# simulation server streams live machine state over WebSocket to a web console and a Unity 3D client
- V1 covers one line: 11 assets, synthetic sensors, fault injection, OEE analytics and what-if scenarios
- One shared wire contract defines the data format for the server and every client

`C#` `.NET 10` `TypeScript` `Three.js` `Unity 6`

### [PLACI: Cargo Risk Intelligence](https://github.com/siddhivinayak-ai/placi-version-0.2)
Screens air cargo before loading, following ICAO Annex 17, the WCO SAFE Framework and PLACI (Pre-Loading Advance Cargo Information) rules.
- 6 agents in a LangGraph workflow: sanctions matching, cargo-description analysis, anomaly detection (Isolation Forest), historical pattern search, risk aggregation, and an explanation a regulator can read
- Each shipment gets a risk score and a decision (clear, request information, extra screening, or do not load), with the evidence behind it
- Tested against 10,000 synthetic historical shipments

`Python` `FastAPI` `LangGraph` `Claude` `MongoDB` `React`

### [BidOps: from RFP to proposal](https://github.com/siddhivinayak-ai/BidOpsv0.1)
Turns a tender PDF into a technical proposal (.docx) and a pricing model (.xlsx).
- Five agents: triage, solution design, commercial pricing, writer and auditor
- The auditor sends drafts back to the writer until the proposal reaches an 85% compliance score against the RFP's requirements
- Searches past proposals using local embeddings, so company data stays on the machine

`Python` `LangGraph` `ChromaDB` `Gemini`

### [hiresprint: Agentic Hiring Intelligence](https://github.com/siddhivinayak-ai/hiresprint)
Tests whether engineers can build *with* AI, not just code without it.
- Candidates solve a realistic task in a sandboxed IDE that includes an AI assistant, a terminal and a test runner
- Scores five weighted dimensions, including prompt quality and error recovery
- Records a full session replay, plus integrity signals: tab switches, focus loss and pastes

`React` `Node.js` `PostgreSQL` `LangChain` `Gemini`

### Self-Maintaining APIs · *private repo, demo on request*
An agent that stops third-party API integrations from breaking when vendors retire versions.
- Monitors vendor deprecation notices and scans the codebase for affected calls
- Prepares a fix for each call and runs the tests in an offline Docker sandbox before and after the patch
- Opens a pull request for human approval and never merges on its own

Demo targets: [support-desk-ai](https://github.com/siddhivinayak-ai/support-desk-ai) · [stripe-legacy-checkout](https://github.com/siddhivinayak-ai/stripe-legacy-checkout)

---

## Also built

- **[SmartScan](https://github.com/siddhivinayak-ai/sih-DevNexus2026)** (Smart India Hackathon 2026): a reinforcement-learning (PPO) scheduler that decides which RF band a receiver scans next. Evaluated against three baselines on unseen test scenarios.
- **[Siddhivinayak](https://github.com/siddhivinayak-ai/siddhivinayak)**: a talking 3D engineering assistant. Hybrid search over your notes with page citations, plus ISO fastener and welding calculators.
- **[BhashaBill](https://github.com/siddhivinayak-ai/BhashaBill)**: turns voice notes and bills in Hindi, Tamil or Gujarati into standard government Bills of Materials, for small businesses (MSMEs) bidding on tenders.
- **[mill](https://github.com/siddhivinayak-ai/mill)**: tool-wear prediction on the UC Berkeley milling dataset. An LSTM beat Random Forest and XGBoost.
- **[EcoTwin](https://github.com/siddhivinayak-ai/EcoTwin)**: an energy digital twin (solar, battery, grid, HVAC) with a live 3D view.
- **[code-writer](https://github.com/siddhivinayak-ai/code-writer-v0.1)**: a terminal coding agent built to run within Gemini's free-tier limits.
- **[sv-iot-telemetry-sim](https://github.com/siddhivinayak-ai/sv-iot-telemetry-sim)**: a pip package that simulates industrial sensors, with anomaly injection and MQTT streaming.

---

## Stack

| | |
|---|---|
| **AI / ML** | LangGraph, LangChain, RAG and GraphRAG, ChromaDB, FAISS, scikit-learn, TensorFlow, PyTorch, Stable-Baselines3 |
| **LLMs** | Claude, Gemini, Groq, local models via Ollama |
| **Backend** | Python, FastAPI, Flask, Node.js, C# / .NET, MongoDB, PostgreSQL, SQLite, WebSockets, MQTT |
| **Frontend & 3D** | React, TypeScript, Vite, Three.js / React Three Fiber, Unity, Streamlit |

## How I work

- **Problem first.** I start from the domain problem, then choose the model.
- **Ship v0.1, then iterate.** PLACI went through three versions in public.
- **Local and low-cost by default.** Local embeddings, swappable LLM providers, and designs that fit within free-tier limits.

<sub>Pune, India</sub>
