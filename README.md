## Hi, I'm Fabio 👋

Software Engineer at UBS, Zurich (Python, TypeScript/Node.js, Swift) · AI Platforms & MLOps · Distributed Systems

---

## 🚀 Currently

Part of the **Graduate Talent Program at UBS**, Zurich (three rotations):

- **Now — Software Engineer, MLOps / AI-as-a-Service Platform** (Aug 2026–present). Building Python model-routing microservices that give internal teams one API to 6 open-weight LLMs (Qwen, Gemma; weights from Hugging Face) served on multi-GPU **vLLM** and to **Azure AI Foundry**, running on **Kubernetes** with the supporting Azure infrastructure as code in **Terraform** and Grafana observability (platform: 35,000 users, billions of tokens per day). Built a benchmarking pipeline that runs on every merge request to measure model latency on H100/H200 GPUs (results in Databricks, TypeScript/Python dashboard), replacing ad-hoc individual benchmarks with one shared standard. Sped up JSON serialization by up to 10x in LLM inference pipelines by adopting orjson.
- **Previously — Software Engineer, Mobile Payments / AI-Augmented Engineering** (Feb–Aug 2026). Shipped Swift/SwiftUI payment features against REST APIs in the UBS Mobile Banking app, and wrote multithreaded XCTest suites wired into the GitLab CI/CD release gates, catching concurrency regressions before production. Integrated MCP tool definitions into agent harnesses (Claude Code, opencode) so LLM agents could assist with code analysis and review.
- **Previously — Software Engineer, Full-Stack Risk & Data Platform** (Sept 2025–Jan 2026). Cut manual triage by 35% for risk and platform stakeholders with a full-stack web app — TypeScript frontend, SQL dashboards and Python ETL pipelines correlating data from 300+ EMEA production applications — with RBAC and audit logging, shipped through CI-gated pipelines.

**Also:** Skills Building Stream Lead, UBS GTPNet (2026) — led a team of 3 that ran 10 online and in-person events with KPMG and UBS senior-management speakers, reaching 300 participants with 94% positive feedback on a USD 8,000 budget.

---

## 🛠 Selected Work

*(private repos — code not public, described here for context)*

**SkiWay** — 3D Ski Navigation App · Co-Founder & Software Engineer (Jan 2026–present)
Co-founded with one partner: native iOS, Apple Watch, Garmin and Android apps on one Supabase backend, with offline 3D ski maps built from OpenStreetMap and elevation data. My parts:
- **AI-assisted live status matching** (Python, AWS EC2): links lift and piste status from resort websites to map features. Deterministic rules run first; a Cloudflare Workers AI model handles only ambiguous names, choosing from a closed shortlist and returning validated JSON, with caching, quotas and a circuit breaker, and every suggestion is confirmed by a person. 47 of 53 official entries matched in the Pila pilot; 28-case offline test suite; CI on GitHub Actions.
- **Android app, end to end** (Kotlin, Jetpack Compose), including a custom difficulty-aware Dijkstra router for fastest or easiest routes over the slope graph, covered by graph-invariant tests.
- **Admin console** (Next.js/React, TypeScript): users, moderation, map corrections, audit log and analytics on Supabase/PostgreSQL with row-level security.
- Contributions to the SwiftUI iOS app and to the 3D map's GPS slope and lift recognition.

`Kotlin · Jetpack Compose · Swift/SwiftUI · TypeScript · Next.js · Python · PostgreSQL/Supabase · Cloudflare Workers AI · AWS`

**Polycopy** — Real-Time Event-Driven Trade Replication Engine
Worker consuming a live **WebSocket** activity stream, reconciled against a REST Data API, routing FAK orders through the Polymarket CLOB v2 SDK. Risk layer with slippage caps and position/daily limits, a persisted crash-safe execution state machine, and idempotent ingestion enforced by **database unique constraints** rather than application checks. Paper-trading Test Lab simulating market impact, latency and partial fills. 97 tests across 18 suites; releases gated on lint/tests/type-check/build and deployed to AWS EC2 over SSH with a pinned host key, into non-root multi-stage containers verified by a post-deploy health check.
`TypeScript · Next.js · viem/ethers (EVM) · Prisma · Docker · AWS · GitHub Actions`

**Swiss Tech Job Radar** — Job-Market Intelligence Platform
**React 19/Vite** front end on an **Express/TypeScript** backend ingesting 7 ATS APIs and structured career-page sources (Greenhouse, Lever, Workday, Ashby, Oracle, Pinpoint) across 24 Swiss companies, with explainable CV–job fit scoring by a **locally-run LLM** and structured-output parsing. Vitest-tested. Built through an AI-directed workflow with Claude Code, owning the architecture and validation decisions myself.
`TypeScript · React 19 · Node.js · Express · SQLite · Vitest · local LLM`

**Summa** — Personal Finance Tracker
Local-first web app for expenses, income, savings and investments. **React/Vite/TypeScript** front end on an **Express** backend over **SQLite** (better-sqlite3), with Recharts visualisations, a d3-geo/TopoJSON world map, statement import from PDF and Excel, and optional LLM-assisted categorisation via pluggable AI providers.
`TypeScript · React · Vite · Express · SQLite · Recharts · d3-geo · LLM integration`

**Casa Rova Dashboard** — Short-Let Bookings & Settlement
Replaces a spreadsheet for managing Airbnb/Booking reservations, expenses and profit-sharing between two owners. **React/Vite/TypeScript** front end with a small Node backend, syncing state across devices in real time over **Server-Sent Events**, with CSV import of Airbnb transaction reports and an emergency local cache.
`TypeScript · React · Vite · Node.js · SSE`

---

## 📦 Public Repos

### 🧠 MLSys 2026 — Operator-Graph Scheduling
Competition solver for scheduling ML operator graphs onto accelerators with limited fast memory. C++ **adaptive large-neighbourhood search**, shipped as a statically linked binary that must leave a valid schedule on disk before a hard 2–60s deadline arrives with no warning — an *anytime* design. Produced by an **agent-driven development loop I designed and ran** (checkpoint/resume, retry-with-backoff, quota-aware scheduling, alerting); I owned the architecture, the evaluation contract and the submission review. Every run graded by an **independent evaluator** rather than the solver's self-reported metrics.
`C++ · Python · Linux` · [Repository](https://github.com/theblackoreo/ML_Sys_Sol)

### 🤖 SAHARA — Secure Ad-Hoc Advanced Resilient Architecture
Master's thesis @ Politecnico di Milano / NECSTLab, visiting research at the **iSENSE Lab, Florida Atlantic University**. A reputation-based, Byzantine-resilient data-dissemination protocol for infrastructure-less ad-hoc networks (drone-swarm scenarios, simulated network nodes) — reputation consensus, SHA-256 block-chaining integrity, Bloom-filter set reconciliation. Automated 500+ NS-3 simulation configurations across 25–196-node topologies; in adversarial simulations, **37x lower data overhead than flooding and 36% lower packet loss than DSDV**.
`C++ · NS-3 · Python` · [Repository](https://github.com/theblackoreo/smesh)

### 🧩 Parallel Maze Solver (ACA-Project)
Perfect-maze extraction from binary/grayscale images (OpenCV) with two implementations — serial and parallel (Open MPI) — domain-decomposed with halo-row exchange, reaching **8x speedup (~50% parallel efficiency)** on a 16-node GCP cluster with strong/weak-scaling benchmarks. Built with a fellow student.
`C++ · OpenCV · Open MPI · Google Cloud` · [Repository](https://github.com/theblackoreo/ACA-Project)

### 🖼️ Image Quality Assessment (IQA)
Subjective, crowdsourced image-quality-evaluation platform — full-stack web app for rating collection and visualization. Basis for a contributor credit on *"Collaborative CNN-based Image Quality Assessment"* (IARIA, 7th Int'l Conf. on Visual Paradigms, Venice, 2022).
`Python · Flask · Jupyter · JavaScript` · [Repository](https://github.com/theblackoreo/image_quality_assessment)

### 🎮 On-Chain Battleship (Solana)
Fully on-chain battleship game — every move is a Solana transaction, no centralized server. Smart contract in **Rust/Anchor**, React frontend, token-based rewards.
`Rust · Anchor · Solana · React` · [Repository](https://github.com/theblackoreo/deep-battle-ship)

### 📱 Whooliday — Travel Booking App
iOS app for accommodation search and booking: price-trend charts, real-time price tracking/alerts, destination suggestions with historical climate data, 6-language support.
`Swift · SwiftUI · MVVM + Combine · Firebase · Google Maps API · Open Meteo API` · [Repository](https://github.com/theblackoreo/Whooliday)

### 🚗 PlateHunt — Italian Vehicle Registration Tracker *(in development)*
Tracks and analyzes newly issued Italian license plates, with statistical insights and forecasting. Includes a Python ingestion pipeline that parses published registration reports out of vendor PDFs — 6 format-specific parsers behind a common interface — loading idempotently into Postgres with per-run tracking, plus a Next.js admin dashboard.
`Swift · Python · Next.js · PostgreSQL · Firebase`

---
