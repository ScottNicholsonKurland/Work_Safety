# 2012 U.S. Workplace Safety Analysis

## Executive Summary

This project analyzes 2012 U.S. workplace safety data by state and creates a composite risk score to compare states on fatality rates, injury and illness rates, inspection capacity, and penalty levels.

The goal is not to prove causation. The goal is to demonstrate analyst judgment: define useful metrics, clean and summarize public data, rank operational risk, and present the results in a recruiter-readable format.

## Business Question

Which U.S. states appear to have the highest workplace safety risk when fatalities, injuries, inspection delay, and penalty levels are considered together?

## Tools Used

- Microsoft Excel
- CSV files
- KPI design
- Composite scoring
- Summary workbook preparation

## Dataset and Files

This repository includes:

- `Scott's workplace safety analysis.xlsx` — original analysis workbook
- `workplace_safety_summary.xlsx` — summary workbook
- `cleaned_state_data.csv` — cleaned analytical dataset
- `summary_kpis.csv` — headline KPI output
- `top10_risk_states.csv` — ranked high-risk states
- `correlation_matrix.csv` — correlation output
- `Data Analytics Career Simulation Report.docx` — supporting report

## Derived Metrics

- **Injuries per Fatality** = injuries and illnesses / fatalities
- **Relative Fatality Rate vs US** = state fatality rate / U.S. fatality rate
- **Risk Score** =  
  `0.40 × fatality-rate percentile`  
  `+ 0.25 × injury-rate percentile`  
  `+ 0.25 × inspection-delay percentile`  
  `+ 0.10 × inverse-penalty percentile`

Higher **Risk Score** means a state appears riskier relative to peers based on incident rates and inspection capacity constraints.

## Key Findings

- **Highest composite risk score:** West Virginia — 84.5
- **Highest fatality rate:** North Dakota — 17.7
- **Median state fatality rate:** 3.5
- **U.S. injuries per fatality:** 625.9
- **Longest inspection cycle:** 521 years to inspect each workplace once
- **States analyzed:** 50

## Top 10 Risk States

| Rank | State | Risk Score | Risk Category |
|---:|---|---:|---|
| 1 | West Virginia | 84.5 | High |
| 2 | Montana | 84.2 | High |
| 3 | New Mexico | 76.8 | Moderate |
| 4 | South Dakota | 74.2 | High |
| 5 | Iowa | 73.6 | High |
| 6 | Alaska | 72.4 | High |
| 7 | Oklahoma | 72.0 | High |
| 8 | Kentucky | 67.8 | Moderate |
| 9 | Nebraska | 67.5 | Moderate |
| 10 | North Dakota | 64.6 | High |

## Analyst Notes

The composite score intentionally combines multiple indicators instead of relying on fatality rate alone. This better reflects the kind of judgment analysts use in business reporting: no single metric captures the whole operational picture.

The score should be interpreted as a prioritization tool, not a definitive safety ranking.

## Portfolio Value

This project demonstrates:

- Excel-based analytical workflow
- metric design
- data cleaning and summary reporting
- risk ranking
- clear communication of findings and limitations
