# Hi, I'm Hai

Data engineer in Helsinki. I build data pipelines and ML systems that are tested, monitored and
easy to explain. B.Eng. in Data Engineering and AI (Turku UAS, 2026); before tech I taught for over
ten years and built my own learning platform, [HaiEduTech](https://haiedutech.com).

## Projects

### Data engineering

| Project | What it is | What it shows |
| --- | --- | --- |
| [hsl-realtime-pipeline](https://github.com/HaiNguyen-python/hsl-realtime-pipeline) | Live Helsinki tram delays: MQTT → Kafka → Spark Structured Streaming → Postgres → Grafana | Watermarks, de-duplication, dead-letter queue, exactly-once results proven by a crash/restart test |
| [oulad-lakehouse](https://github.com/HaiNguyen-python/oulad-lakehouse) | Batch medallion lakehouse for the Open University learning-analytics dataset | PySpark bronze/silver with data contracts and quarantine, DuckDB star schema, partition-level incremental rebuilds, reconciliation checks, Airflow |
| [learning-events-platform](https://github.com/HaiNguyen-python/learning-events-platform) | Event platform for a learning app: FastAPI ingestion → warehouse → dbt → teacher reports | Versioned event contracts with a compatibility check, idempotent ingest, GDPR erasure, dbt sessionization and SCD2, dbt tests in CI |
| [cdc-iceberg-lakehouse](https://github.com/HaiNguyen-python/cdc-iceberg-lakehouse) | Postgres change data capture with Debezium into Apache Iceberg | LSN-ordered merges, idempotent replay, schema evolution, SCD2, time travel, compaction |
| [subscription-analytics](https://github.com/HaiNguyen-python/subscription-analytics) | Stripe-style subscription analytics with dbt and Dagster | MRR movements, cohorts and NRR from one semantic layer; MRR reconciled to billing |

### Machine learning

| Project | What it is | What it shows |
| --- | --- | --- |
| [fi-energy-forecast-mlops](https://github.com/HaiNguyen-python/fi-energy-forecast-mlops) | Day-ahead electricity demand forecasts for Finland (Fingrid + FMI data) | Leakage-safe features, time-series validation, MLflow registry with a promotion rule, calibrated prediction intervals, drift monitoring, Airflow |
| [fair-early-intervention](https://github.com/HaiNguyen-python/fair-early-intervention) | Which students to contact early, under a budget and a fairness constraint (from my thesis) | Temporal validation, recall at fixed capacity, per-group fairness audit and mitigation, Q-learning policy in a Gymnasium simulator, model card |
| [knowledge-tracing-srs](https://github.com/HaiNguyen-python/knowledge-tracing-srs) | Predict vocabulary recall and schedule reviews | BKT with EM, PFA and half-life regression vs baselines, calibration, model-based scheduling vs Leitner and SM-2 in a learner simulator |
| [ielts-essay-scorer](https://github.com/HaiNguyen-python/ielts-essay-scorer) | IELTS Writing Task 2 band scores with grounded AI feedback | Agreement measured against two human raters, first-language fairness audit, feedback that must quote the essay |
| [learning-recommender](https://github.com/HaiNguyen-python/learning-recommender) | Next-lesson recommendations for learners | Implicit ALS, level-aware re-ranking, cold start, offline metrics and a simulated A/B test |
| [edtech-experimentation](https://github.com/HaiNguyen-python/edtech-experimentation) | A/B testing pipeline for a learning app | SRM checks, CUPED, delta method, sequential tests, simulations that prove the false-positive rate |
| [k8s-model-serving](https://github.com/HaiNguyen-python/k8s-model-serving) | Model serving on Kubernetes with a canary controller | Automatic promote or rollback on errors, latency and drift; kind end-to-end test in CI |

### AI and RAG

| Project | What it is | What it shows |
| --- | --- | --- |
| [socratic-tutor-agent](https://github.com/HaiNguyen-python/socratic-tutor-agent) | AI tutor agent that helps students without giving away answers | Tool use, guardrails against answer leaks and prompt injection, eval harness, LLM judge checked against hand labels |
| [multilingual-rag-fi](https://github.com/HaiNguyen-python/multilingual-rag-fi) | English and Vietnamese questions answered from Finnish documents | Cross-lingual retrieval compared per language, citations, refusal threshold |
| [course-rag-evals](https://github.com/HaiNguyen-python/course-rag-evals) | Course Q&A assistant that cites sources and refuses off-topic questions | Hybrid retrieval (BM25 + vectors), pgvector, a 42-question eval set with a CI gate, data-chosen refusal threshold |

Every repo has a `docs/how-it-works.md` (code walkthrough) and `docs/decisions.md` (why each
choice was made), CI with lint, type checks and tests, and runs offline with one command. Results that come from
generated data are labelled synthetic.

## Thesis

[Reinforcement Learning for Early Educational Intervention: A Cost-Aware and Fairness-Aware
Approach](https://urn.fi/URN:NBN:fi:amk-202605018815) — Q-learning, DQN and PPO on the OULAD
dataset, deciding which students get early support under budget and fairness constraints.

## Tools I use

Python · SQL · PySpark · Apache Airflow · Dagster · dbt · Kafka · Debezium · Apache Iceberg · PostgreSQL ·
DuckDB · Docker · Kubernetes · AWS · Databricks · MLflow · LightGBM · scikit-learn · Gymnasium · FastAPI ·
Prometheus · Grafana

## Contact

[LinkedIn](https://www.linkedin.com/in/hainguyen2401/) · [haiedutech.com](https://haiedutech.com)
