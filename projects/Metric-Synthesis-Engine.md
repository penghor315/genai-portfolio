# Metric Synthesis Engine (AI Engineer Case Study)

**Repository:** [https://github.com/penghor315/metric-synthesis-engine](https://github.com/penghor315/metric-synthesis-engine)

### 🚀 Overview
A production-grade, hybrid AI architecture designed to generate strategic financial reports with **100% numerical accuracy**. This project addresses the common challenge of "hallucinations" in LLMs by strictly decoupling calculation from narrative synthesis.

### 🏗️ Architecture
* **Deterministic Layer (Python/Pandas):** Handles all ETL, aggregations, and statistical analysis. Acts as the immutable "Source of Truth."
* **Probabilistic Layer (Gemini 2.5 Flash):** Strictly limited to narrative synthesis using a grounded evidence payload provided by the Python layer.

### ✨ Key Highlights
* **Production-Ready:** Fully containerised using **Docker** for reproducible execution across environments.
* **Automated QA:** Implemented a custom evaluation framework (`evaluator.py`) that grades reports on structural integrity and data grounding (Score: 0.0 - 1.0).
* **Data Integrity:** Features strict type hinting, schema validation, and robust logging.
* **Outputs:** Generates professional Markdown reports and Matplotlib visualizations automatically.

### 🛠️ Tech Stack
* **Core:** Python 3.10+, Pandas
* **AI Model:** Google Gemini 2.5 Flash API
* **DevOps:** Docker, Git
* **Visualization:** Matplotlib
