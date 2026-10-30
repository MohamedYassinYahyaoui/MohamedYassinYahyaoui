# Hi, I'm Mohamed Yassin Yahyaoui

**Software Engineering Student @ ISSAT Sousse (Tunisia)**  
*Focused on Distributed Systems, High-Throughput Event Streaming & Resilient Anti-Bot Pipelines*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Yassin_Yahyaoui-0077b5?style=flat-square&logo=linkedin)](https://linkedin.com/in/yassin-yahyaoui-331939389/)
[![GitHub](https://img.shields.io/badge/GitHub-MohamedYassinYahyaoui-181717?style=flat-square&logo=github)](https://github.com/MohamedYassinYahyaoui)
[![Email](https://img.shields.io/badge/Email-yassinyahyaoui0000%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:yassinyahyaoui0000@gmail.com)

---

### Flagship Systems & Live Benchmarks

#### 1. [StreamPulse](https://github.com/MohamedYassinYahyaoui/Stream_pulse) — Distributed Telemetry & Ingestion Engine
- **Throughput:** **10,635.49 req/sec** (50,000 / 50,000 HTTP 202, 0% drop rate) across 100 concurrent sockets.
- **Tech Stack:** FastAPI, PostgreSQL 16 (Async SQLAlchemy 2.0), Redis 7, Redpanda (Kafka), AIOKafka, ClickHouse OLAP, Grafana.
- **Architecture Highlights:** Multi-tenant auth plane (SHA-256 keys, HS256 JWTs), Redis L1/L2 read-through cache, atomic pipeline rate-limiting (`INCRBY`/`EXPIRE`), ClickHouse micro-batching worker (10k-event window) eliminating write-stalls, and 14 Pytest integration tests.
- 📹 **[Watch 90s Architecture Walkthrough](https://www.loom.com/share/1cc9c2674e0b4a73b64ff7489858df0d)**

#### 2. [Automated Competitor Intelligence Engine](https://github.com/MohamedYassinYahyaoui/Automated-Competitor-Intelligence-Engine) — Async Anti-Bot ETL & Columnar OLAP
- **Performance:** **0.36s** concurrent multi-brand ingestion across Shopify JSON & HTML microdata.
- **Token Pruning:** **92.6% token reduction** (183,972 chars → 13,636 chars) prior to Gemini 2.5 Flash synthesis.
- **Tech Stack:** Python (`asyncio.gather`), `curl_cffi` (Chrome 120 TLS/JA3 impersonation), Headless Playwright Chromium, DuckDB, Pydantic v2.
- **Architecture Highlights:** Two-tier ingestion auto-escalating to Playwright on HTTP 403 Cloudflare challenges, strict Pydantic v2 validation, Dead-Letter Queue quarantine with CLI replay (`scripts/replay_dlq.py`), and 7 Pytest integration tests.
   **[Watch 90s Architecture Walkthrough](https://www.loom.com/share/bb6d64ce11834316989040e831c22e84)**

---

### Technical Stack
- **Languages:** Python (Asyncio, Typing), SQL, C, TypeScript, Bash
- **Streaming & Messaging:** Apache Kafka / Redpanda, AIOKafka, Event-Driven Architecture, Micro-Batching, Dead-Letter Queues (DLQ)
- **Databases & OLAP:** PostgreSQL (Async SQLAlchemy 2.0), Redis, ClickHouse, DuckDB, SQLite
- **Backend & Cloud:** FastAPI, Pydantic v2, `curl_cffi`, Playwright, Docker, Docker Compose, GitHub Actions CI/CD, Linux, Grafana
