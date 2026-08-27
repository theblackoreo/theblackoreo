## Hi, I'm Fabio 👋

Software Engineer (Swift, Python, TypeScript/Node.js) · AI-Assisted Development · Distributed Systems

---

## 🚀 Currently

Part of the **Graduate Talent Program at UBS**, Zurich (two rotations):

- **Now — iOS Software Engineer, AI-Augmented Engineering / Mobile Payments** (Feb 2026–present). Configure agent harnesses (Claude Code, opencode) with MCP tool integrations to orchestrate LLM agents for code analysis, generation, and review across a 1M+ LOC banking codebase. Caught concurrency regressions pre-production in UBS Mobile Banking (3M+ users) via multithreaded XCTest suites as release gates.
- **Previously — Software Engineer, Full-Stack Risk & Data Platform** (Sept 2025–Jan 2026). Built Python ETL pipelines ingesting and correlating 2M+ rows across 300+ production apps (EMEA), feeding real-time TypeScript dashboards, CI-gated with RBAC + audit logging.

---

## 🛠 Selected Work

*(private repos — code not public, described here for context)*

**SkiWay** — Full-Stack Geospatial Platform (80K+ LOC) · Co-Founder & Developer, in development
Node.js REST APIs over PostgreSQL, containerized Python/GDAL pipeline processing 200+ MB geospatial datasets, CI-gated on AWS at sub-100ms p99 tile latency, offline coverage for 500+ ski resorts, native Swift/CoreML client.
`Node.js · Python · PostgreSQL · GDAL · AWS · Swift/CoreML`

**Swiss Tech Job Radar** — AI-Directed Full-Stack Job-Intelligence Platform (2026)
Built and tested through an AI-directed workflow with Claude Code, owning architecture and validation decisions myself. Node.js/Express backend + React/TypeScript frontend ingesting and correlating postings from 7 ATS APIs and structured career-page sources (Greenhouse, Lever, Workday, Ashby, Oracle, Pinpoint) across 24 Swiss companies, with explainable CV–job fit scoring and optional local-LLM semantic matching. ~3.7K LOC.
`TypeScript · Node.js · React · Express · SQLite · Vitest · LLM integration`

**Polycopy** — On-Chain Copy-Trading Engine for Polymarket (Polygon/EVM), ~4.5K LOC
WebSocket real-time activity stream + Data API reconciliation → FAK order routing via the Polymarket CLOB v2 SDK. Risk layer (worst-price slippage caps, position/daily limits, crash-safe execution state), paper-trading Test Lab for market-impact and latency simulation, multi-scheme wallet signing (EOA, Proxy, Gnosis Safe), AES-256-GCM credential encryption. Deployed on AWS EC2 (Docker Compose, GitHub Actions CI/CD, Caddy).
`TypeScript · Solidity/EVM · Rust (tooling) · Docker · AWS · GitHub Actions`

---

## 📦 Public Repos

### 🤖 SAHARA — Secure Ad-Hoc Advanced Resilient Architecture
Master's thesis @ Politecnico di Milano / NECSTLab, visiting research at the **iSENSE Lab, Florida Atlantic University**. A reputation-based, Byzantine-resilient data-dissemination protocol for infrastructure-less ad-hoc networks (drone-swarm scenarios, simulated network nodes) — reputation consensus, SHA-256 block-chaining integrity, Bloom-filter set reconciliation. Automated 500+ NS-3 simulation configurations across 25–196-node topologies: **37x lower data overhead, 36% lower packet loss vs. DSDV, O(n^1.47) empirical scaling**.
`C++ · NS-3 · Python` · [Repository](https://github.com/theblackoreo/smesh)

### 🧩 Parallel Maze Solver (CA-Project)
Perfect-maze extraction from binary/grayscale images (OpenCV) with two implementations — serial and parallel (OpenMPI) — domain-decomposed across images up to **64M pixels**, near-8x speedup on a 16-node GCP cluster with strong/weak-scaling benchmarks.
`C++ · OpenCV · OpenMPI · Google Cloud` · [Repository](https://github.com/theblackoreo/ACA-Project)

### 🖼️ Image Quality Assessment (IQA)
Subjective, crowdsourced image-quality-evaluation platform — full-stack web app for rating collection and visualization. Basis for a contributor credit on *"Collaborative CNN-based Image Quality Assessment"* (IARIA, 7th Int'l Conf. on Visual Paradigms, Venice, 2022).
`Python · Flask · Jupyter · JavaScript` · [Repository](https://github.com/theblackoreo/image_quality_assessment)

### 🎮 On-Chain Battleship (Solana)
Fully on-chain battleship game — every move is a Solana transaction, no centralized server. Smart contracts in Rust/Anchor, React frontend, token-based rewards.
`Rust · Anchor · Solana · React` · [Client](https://github.com/theblackoreo/deep-battle-ship) · [Server](https://github.com/theblackoreo/HyperShipBattle_Server)

### 📱 Whooliday — Travel Booking App
iOS app for accommodation search and booking: price-trend charts, real-time price tracking/alerts, destination suggestions with historical climate data, 6-language support.
`Swift · SwiftUI · MVVM + Combine · Firebase · Google Maps API · Open Meteo API` · [Repository](https://github.com/theblackoreo/Whooliday)

### 🚗 PlateHunt — Italian Vehicle Registration Tracker *(in development)*
Tracks and analyzes newly issued Italian license plates, with statistical insights and forecasting.
`Swift · Core ML · Create ML · MLX · Firebase · Python`

---

📫 fabio.tagliani99@icloud.com · [LinkedIn](https://linkedin.com/in/fabio-tagliani)
