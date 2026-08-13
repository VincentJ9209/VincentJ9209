# Hi, I'm Vincent 👋

### 資料工程 × Python 後端 × AI / LLM
### Data Engineering × Python Backend × AI / LLM

我專注於將 **實際需求、資料流程、AI 模型與後端系統** 整合成可驗證、可交付的工程成果。

I build **verifiable AI and data systems** that connect real-world requirements, data pipelines, evaluation, and backend engineering.

---

## About Me｜關於我

過去經驗涵蓋商業分析、系統整合與企業需求溝通，目前的工程實作聚焦於：

- **Data Engineering｜資料工程**
- **Python Backend｜Python 後端**
- **AI / LLM Application Engineering｜AI / LLM 應用工程**

我的工程實作重視：

**Requirements → Data → AI / Retrieval → Backend → Evaluation → Delivery**

除了功能能否執行，我也重視資料品質、客觀評估、測試、可重現性，以及系統是否能回到實際使用情境。

My engineering approach emphasizes **data quality, measurable evaluation, testing, reproducibility, and real-world usability**.

---

# Featured Projects｜代表作品

## 🚲 [YouBike Data Pipeline](https://github.com/VincentJ9209/youbike-data-pipeline)

**Data Engineering × ELT × Orchestration × CI/CD**

以臺北市與新北市官方 YouBike 即時資料為來源，建立從 source normalization、冪等 PostgreSQL 寫入、dbt 資料模型與品質驗證，到 Airflow orchestration、Docker、GitHub Actions 與 Docker Hub 發布的可重現 ELT pipeline。

A reproducible ELT pipeline that normalizes Taipei and New Taipei YouBike data, persists idempotent PostgreSQL snapshots, builds analytical models with dbt, orchestrates the workflow with Airflow, and validates delivery through CI/CD.

### Key Evidence

- Python adapters → canonical `StationSnapshot`
- Idempotency key: `(source_city, station_id, source_updated_at)`
- PostgreSQL 16 raw snapshot persistence
- dbt: `4` models + `15` data-quality tests
- Hosted CI: `8 passed`
- dbt build: `PASS=19 WARN=0 ERROR=0`
- Airflow 3.3.0: `extract_and_load → dbt_run → dbt_test`
- Docker Compose + GitHub Actions + Docker Hub publishing

**Focus**

`Data Engineering` · `ELT` · `PostgreSQL` · `dbt` · `Apache Airflow` · `Data Quality` · `pytest` · `Docker` · `CI/CD`

➡️ **[View Repository](https://github.com/VincentJ9209/youbike-data-pipeline)**

---

## 🔎 [RAG Knowledge Assistant](https://github.com/VincentJ9209/rag-knowledge-assistant)

**LLM / RAG × Python Backend × Evaluation**

建立一套可重現、可評估的 RAG 系統，在相同 frozen corpus 與 holdout protocol 下比較 Keyword 與 Vector Retrieval，並透過 FastAPI 提供 grounded answer service。

A reproducible RAG system that evaluates keyword and vector retrieval under the same frozen corpus and holdout protocol, with grounded generation exposed through FastAPI.

### Key Evidence

- `139` frozen FAQ documents
- `695` Ground Truth questions
- `486` tuning / `209` holdout
- Keyword Hit Rate@5: `0.9713`
- Vector Hit Rate@5: `0.9809`
- Vector MRR: `0.9120`
- `27` offline pytest tests
- FastAPI · Docker · GitHub Actions CI

**Focus**

`RAG` · `Retrieval Evaluation` · `Embeddings` · `Vector Search` · `Grounding` · `FastAPI` · `pytest` · `Docker` · `CI`

➡️ **[View Repository](https://github.com/VincentJ9209/rag-knowledge-assistant)**

---

## 🚗 [FleetVision｜車況之眼](https://github.com/VincentJ9209/FleetVision)

**Computer Vision × Data Engineering × Human-in-the-Loop**

以共享車輛車況影像為情境，建立具備資料治理、Annotation QA、Deduplication、模型評估與人工複核的 Computer Vision workflow。

An evidence-first computer-vision workflow for governed vehicle-image data, annotation QA, reproducible evaluation, and human review.

### Key Engineering Areas

- Metadata inventory & data-quality controls
- Annotation QA & bounding-box validation
- Exact / perceptual deduplication
- Dataset split & leakage checks
- YOLOv8 evaluation and FP / FN analysis
- Streamlit + SQLite human-review workflow
- Reproducible pytest-based data workflows

**Focus**

`Computer Vision` · `Data Engineering` · `Data Governance` · `Annotation QA` · `Model Evaluation` · `Human-in-the-Loop`

➡️ **[View Repository](https://github.com/VincentJ9209/FleetVision)**

---

# Core Stack｜核心技術

### Backend & Data

`Python` · `SQL` · `PostgreSQL` · `dbt` · `Apache Airflow` · `FastAPI` · `SQLite` · `ETL / ELT`

### AI / ML / LLM

`RAG` · `OpenAI API` · `Embeddings` · `Vector Search` · `Function Calling` · `Agentic Loop` · `YOLOv8` · `OpenCV` · `scikit-learn`

### Engineering & Delivery

`pytest` · `Docker` · `Docker Compose` · `Docker Hub` · `Git` · `GitHub` · `GitHub Actions` · `CI/CD`

---

# What I Focus On｜目前聚焦方向

### Data Engineering
資料處理、驗證、品質管理與可重現的 Data Pipeline。

Data processing, validation, quality control, and reproducible pipelines.

### Python Backend
API、service integration、自動化測試與 containerized delivery。

API development, service integration, automated testing, and containerized delivery.

### AI Application Engineering
RAG / LLM、Retrieval Evaluation、Computer Vision 與 Human-in-the-Loop system。

RAG / LLM, retrieval evaluation, computer vision, and human-in-the-loop systems.

---

## Engineering Mindset｜工程實作原則

### Build → Evaluate → Test → Deliver

從實際需求出發，將資料、AI 與後端流程整合為：

**可驗證 · 可測試 · 可重現 · 可維護**

Starting from real-world requirements, I turn data, AI, and backend workflows into:

**Verifiable · Testable · Reproducible · Maintainable systems**
