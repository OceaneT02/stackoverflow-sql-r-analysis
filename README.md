# stackoverflow-sql-r-analysis
SQL + R project analysing Stack Overflow answer speeds using Kaggle BigQuery data.

**Tools:** SQL (BigQuery on Kaggle), R (tidyverse, ggplot2)  

## Problem
Which Stack Overflow tags get the fastest answers, and how has this changed over time?

## Dataset
- Source: BigQuery public dataset on Kaggle (`bigquery-public-data.stackoverflow.*`)
- Tables: `posts_questions`, `posts_answers`, `tags`

## Method
1. SQL: Extracted time-to-first-answer & acceptance rates by tag/year.
2. R: Cleaned + visualised trends with ggplot2.

## Key Metrics
- Median minutes to first answer
- % answered within 1h / 24h
- Acceptance rate

## Results (teaser only, full in notebook)
- Chart 1: Fastest 10 tags by answer speed
- Chart 2: Time-to-first-answer trends for Python, R, SQL, JavaScript

## Repo Structure
- `sql/`: Queries used
- `r/`: Analysis notebooks
- `data/`: Exported CSVs
- `figures/`: Visuals

## Next Steps
- Add survival analysis for time-to-accepted-answer
- Compare new vs experienced users
