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

### Machine learning

| Project | What it is | What it shows |
| --- | --- | --- |
| [fi-energy-forecast-mlops](https://github.com/HaiNguyen-python/fi-energy-forecast-mlops) | Day-ahead electricity demand forecasts for Finland (Fingrid + FMI data) | Leakage-safe features, time-series validation, MLflow registry with a promotion rule, calibrated prediction intervals, drift monitoring, Airflow |
| [fair-early-intervention](https://github.com/HaiNguyen-python/fair-early-intervention) | Which students to contact early, under a budget and a fairness constraint (from my thesis) | Temporal validation, recall at fixed capacity, per-group fairness audit and mitigation, Q-learning policy in a Gymnasium simulator, model card |
| [knowledge-tracing-srs](https://github.com/HaiNguyen-python/knowledge-tracing-srs) | Predict vocabulary recall and schedule reviews | BKT with EM, PFA and half-life regression vs baselines, calibration, model-based scheduling vs Leitner and SM-2 in a learner simulator |
| [course-rag-evals](https://github.com/HaiNguyen-python/course-rag-evals) | Course Q&A assistant that cites sources and refuses off-topic questions | Hybrid retrieval (BM25 + vectors), pgvector, a 42-question eval set with a CI gate, data-chosen refusal threshold |

Every repo has a `docs/how-it-works.md` (code walkthrough) and `docs/decisions.md` (why each
choice was made), CI with lint, type checks and tests, and runs offline with one command.

## Thesis

[Reinforcement Learning for Early Educational Intervention: A Cost-Aware and Fairness-Aware
Approach](https://urn.fi/URN:NBN:fi:amk-202605018815) — Q-learning, DQN and PPO on the OULAD
dataset, deciding which students get early support under budget and fairness constraints.

## Tools I use

Python · SQL · PySpark · Apache Airflow · dbt · Kafka · PostgreSQL · DuckDB · Docker · Kubernetes ·
AWS · Databricks · MLflow · LightGBM · scikit-learn · Gymnasium · FastAPI · Grafana

## Contact

[LinkedIn](https://www.linkedin.com/in/hainguyen2401/) · [haiedutech.com](https://haiedutech.com)
