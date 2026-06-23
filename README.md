# Investor Intelligence Knowledge Graph

## Overview

This project aims to model analyst behavior during earnings calls using a Knowledge Graph (KG)-based approach.

The objective is to identify recurring analyst interests, thematic questioning patterns, and cross-company linkages to improve prediction of likely questions in future earnings calls.

The system will leverage historical earnings call transcripts, analyst interactions, and thematic relationships across multiple companies to build a structured representation of analyst behavior.

---

## Problem Statement

Analysts often participate in multiple earnings calls and industry conferences, asking recurring questions around topics such as:

- Net Interest Margin (NIM)
- Deposit Growth
- CASA
- Asset Quality
- Credit Costs
- Loan Growth
- Capital Adequacy

Understanding these patterns can help Investor Relations (IR) teams anticipate likely questions and prepare more effectively for future interactions.

---

## Objectives

- Collect and organize historical earnings call transcripts.
- Extract analysts, companies, themes, and questions from transcripts.
- Build a Knowledge Graph representing analyst-company-theme relationships.
- Analyze recurring analyst behavior across companies and time periods.
- Identify thematic trends and follow-up questioning patterns.
- Develop a framework for predicting future analyst questions.

---

## Proposed Knowledge Graph Structure

### Node Types

| Node Type | Description |
|------------|-------------|
| Analyst | Individual analyst participating in calls |
| Company | Listed company (e.g., Axis Bank, HDFC Bank) |
| Earnings Call | Quarterly earnings conference call |
| Question | Analyst question from Q&A section |
| Theme | Topic discussed (NIM, CASA, Deposits, etc.) |
| Metric | Financial metric referenced in discussion |

### Relationship Types

| Relationship | Description |
|---------------|-------------|
| ASKED | Analyst asked a question |
| ABOUT | Question relates to a theme |
| DIRECTED_TO | Question addressed to a company |
| OCCURRED_IN | Question occurred during a specific call |
| FOLLOWS_UP | Question builds upon a previous topic |
| RELATED_TO | Connection between themes |

---

## Project Structure

```
investor-intelligence-kg/
│
├── data/
│   ├── raw_transcripts/
│   └── processed/
│
├── notebooks/
│
├── outputs/
│
├── docs/
│
├── requirements.txt
│
└── README.md
```

---

## Technology Stack

- Python
- pandas
- spaCy
- NetworkX
- pdfplumber
- Jupyter / Google Colab

---

## Current Status

### Completed

- Historical transcript collection
- Transcript inventory creation
- Project repository setup
- Folder structure creation
- Python environment setup

### In Progress

- Manual transcript review
- Theme identification
- Knowledge Graph schema refinement

### Upcoming

- Entity extraction pipeline
- Graph construction
- Analyst behavior analysis
- Question prediction framework

---

## Expected Outcome

A graph-driven analyst intelligence system capable of:

- Mapping analyst behavior patterns
- Tracking recurring themes across companies
- Identifying cross-company questioning trends
- Supporting prediction of likely future analyst questions
