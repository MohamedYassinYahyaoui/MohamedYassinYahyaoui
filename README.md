# Mohamed Yassine Yahyaoui

**Backend Engineering & Distributed Systems**  
Sousse, Tunisia • [LinkedIn](https://linkedin.com) • [Email](mailto:yassinyahyaoui0000@gmail.com)

---

### 🚀 What I Build
I specialize in high-throughput backend architecture, event-driven streaming pipelines, and analytical data storage. My core stack focuses on asynchronous concurrency (**FastAPI**, **Asyncio**), distributed message brokers (**Redpanda / Kafka**), and columnar OLAP engines (**ClickHouse**, **DuckDB**).

---

### 🛠️ Featured Systems & Flagship Repositories

#### ⚡ [StreamPulse — Distributed Real-Time Log & Event Analytics Engine](https://github.com/MohamedYassinYahyaoui/Stream_pulse)
* **Stack:** FastAPI, AIOKafka, Redpanda, ClickHouse (MergeTree), Grafana, Docker Compose
* **Architecture:** Ingestion gateway processing 50k events with non-blocking AIOKafka publishing; dual-threshold micro-batching (`1,000 records` / `1.0s timeout`) flushed to ClickHouse via thread pools (`asyncio.to_thread`).
* **Fault Tolerance:** Schema validation at ingress (HTTP 422) + Dead-Letter Queue (DLQ) for poisoned payloads and database insert failures.
* **Telemetry:** Pre-provisioned Grafana dashboards tracking throughput, volume, and P95/P99 latency percentiles.

#### 📊 [Automated Competitor Intelligence Engine](https://github.com/MohamedYassinYahyaoui/Automated-Competitor-Intelligence-Engine)
* **Stack:** Python, DuckDB, HTTPX, `curl_cffi`, Playwright Stealth, Gemini API, Docker, GitHub Actions
* **Architecture:** Multi-tier asynchronous ETL pipeline crawling e-commerce catalogs with adaptive failover to stealth browser sessions for Cloudflare/anti-bot protected targets.
* **Analytics & Automation:** Conflict-safe atomic upserts into embedded DuckDB OLAP storage; scheduled daily autonomous scraping via containerized GitHub Actions CI.

---

### 💻 Technical Stack
* **Languages:** Python (Asyncio, Pydantic), TypeScript, SQL, C
* **Distributed & Data Platforms:** Redpanda, Apache Kafka, ClickHouse, DuckDB, PostgreSQL, Redis
* **Infrastructure & Observability:** Docker, Docker Compose, Grafana, Linux, Git, GitHub Actions CI/CD
