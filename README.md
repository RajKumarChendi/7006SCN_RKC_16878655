# 7006SCN — Machine Learning and Big Data

**Student:** Raj Kumar | **SID:** 16878655 | **Module:** 7006SCN

## Project

Predicting US domestic flight arrival delays (≥15 minutes) using the BTS On-Time Performance dataset and PySpark distributed machine learning.

## Dataset

| Property | Detail |
|----------|--------|
| Source | Bureau of Transportation Statistics (BTS) |
| URL | https://transtats.bts.gov |
| Rows | ~13.3 million flights |
| Features | 110 columns (8 used for modelling) |
| Licence | US Public Domain / Open Government Data |

## Task Progress

| Task | Week | Notebook | Status | Commits |
|------|------|----------|--------|---------|
| T1 — Problem & Dataset | 1–2 | [Task1.ipynb](notebooks/Task1.ipynb) | Done | 3 |
| T2 — Data Engineering | 2 | [Task2.ipynb](notebooks/Task2.ipynb) | Done | 4 |
| T3 — ML Models | 3 | [Task3.ipynb](notebooks/Task3.ipynb) | Done | 4 |
| T4 — Distributed Computing | 4 | [Task4.ipynb](notebooks/Task4.ipynb) | Pending | — |
| T5 — Evaluation & Stability | 5 | [Task5.ipynb](notebooks/Task5.ipynb) | Pending | — |
| T6 — Tableau | 6 | [Task6.ipynb](notebooks/Task6.ipynb) | Pending | — |

## Results Summary (Task 3)

| Model | AUC-ROC | AUC-PR | Train Time |
|-------|---------|--------|------------|
| GBT | 0.6601 | 0.3410 | 219s |
| Logistic Regression | 0.6208 | 0.2763 | 159s |
| Random Forest | 0.5000 | 0.2095 | 80s |
| Naive Bayes | 0.4722 | 0.1958 | 97s |

## Environment

- Python 3.11, PySpark 4.1.1, Java 17
- Conda env: spark311
- SparkSession: local[2], 8g driver memory
