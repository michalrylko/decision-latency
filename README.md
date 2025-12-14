
Ten jeden błąd może „rozjechać” całe README na GitHubie.

---

# ✅ POPRAWIONA, FINALNA WERSJA README.md (WKLEJ 1:1)

```markdown
# Decision Latency Analytics

This project analyzes **decision-making latency** using real-world data from
GitHub Pull Requests.

A Pull Request (PR) is treated as a proxy for a **decision process**:
- a proposal is submitted,
- reviewers evaluate the change,
- a final decision is made (merge or close).

The goal of the project is to understand **how long decisions take**,  
**what factors contribute to delays**, and **how stalled decisions can be identified early**.

---

## Project structure

```text
decision-latency-analytics/
├── notebooks/
│   ├── 00_data_extraction.ipynb
│   ├── 01_eda.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_modeling.ipynb
│   └── 04_decision_playbook.ipynb
├── data/
│   └── apache_airflow_pull_requests_raw.csv
├── README.md
└── requirements.txt

Notebooks

00_data_extraction.ipynb – data extraction pipeline using the GitHub API

01_eda.ipynb – exploratory data analysis of decision latency

02_feature_engineering.ipynb – construction of decision-related features

03_modeling.ipynb – predictive modeling of delayed (stalled) decisions

04_decision_playbook.ipynb – actionable insights and decision design recommendations

Data source

Public GitHub Pull Request data from the
apache/airflow repository.

All data used in this project is publicly available and collected via the
GitHub REST API.

Methodology (high level)

Extract Pull Request metadata and timestamps

Define decision latency as the time between PR creation and closure

Explore latency distributions and review dynamics

Engineer features describing decision complexity and collaboration

Build predictive models for stalled decisions

Translate findings into practical decision design guidelines

Status

🚧 Work in progress
This repository is under active development. New notebooks and analyses
are added incrementally.
