# 2012 U.S. Workplace Safety Risk Analysis

This Excel portfolio project analyzes 2012 U.S. workplace safety data by state and builds a composite risk score using fatality rates, injury and illness rates, inspection capacity, and penalty levels.

The purpose is not to prove causation. The purpose is to demonstrate practical analyst judgment: define usable metrics, clean and summarize public data, rank operational risk, and communicate limitations clearly.

## At a Glance

| Area | Detail |
|---|---|
| Dataset | 2012 U.S. workplace safety data by state |
| Tools | Excel, CSV, KPI design, composite scoring |
| States analyzed | 50 |
| Main output | State-level workplace safety risk ranking |
| Top composite-risk state | West Virginia — 84.5 |
| Highest fatality-rate state | North Dakota — 17.7 |
| Best-fit roles | Data Analyst, Reporting Analyst, Operations Analyst, Program Analyst, Public-Sector Analyst |

## Business Question

Which U.S. states appear to have the highest workplace safety risk when fatalities, injuries, inspection delay, and penalty levels are considered together?

## Repository Files

| File | Purpose |
|---|---|
| `Scott's workplace safety analysis.xlsx` | Original analysis workbook |
| `workplace_safety_summary.xlsx` | Summary workbook for portfolio review |
| `cleaned_state_data.csv` | Cleaned analytical dataset |
| `summary_kpis.csv` | Headline KPI output |
| `top10_risk_states.csv` | Ranked high-risk states |
| `correlation_matrix.csv` | Correlation output |
| `Data Analytics Career Simulation Report.docx` | Supporting written report |
| `docs/project_summary.md` | Recruiter-readable project summary |

## Derived Metrics

- **Injuries per Fatality** = injuries and illnesses / fatalities
- **Relative Fatality Rate vs. U.S.** = state fatality rate / U.S. fatality rate
- **Risk Score** =  
  `0.40 × fatality-rate percentile`  
  `+ 0.25 × injury-rate percentile`  
  `+ 0.25 × inspection-delay percentile`  
  `+ 0.10 × inverse-penalty percentile`

Higher **Risk Score** means a state appears riskier relative to peers based on the selected incident-rate and inspection-capacity indicators.

## Key Findings

| Metric | Result |
|---|---:|
| States analyzed | 50 |
| U.S. fatalities, 2012 | 2,814 |
| U.S. fatality rate | 3.4 |
| U.S. injuries and illnesses | 1,761,200 |
| U.S. injuries per fatality | 625.9 |
| Median state fatality rate | 3.5 |
| Highest state fatality rate | 17.7 |
| Median years to inspect each workplace once | 111.5 |
| Longest years to inspect each workplace once | 521.0 |

## Top 10 Risk States

| Rank | State | Risk Score | Fatality Rate | Injury/Illness Rate | Years to Inspect Once | Risk Category |
|---:|---|---:|---:|---:|---:|---|
| 1 | West Virginia | 84.5 | 6.9 | 4.1 | 173 | High |
| 2 | Montana | 84.2 | 7.3 | 5.0 | 135 | High |
| 3 | New Mexico | 76.8 | 4.8 | 3.9 | 191 | Moderate |
| 4 | South Dakota | 74.2 | 6.7 | 3.5 | 521 | High |
| 5 | Iowa | 73.6 | 6.6 | 4.5 | 98 | High |
| 6 | Alaska | 72.4 | 8.9 | 4.6 | 58 | High |
| 7 | Oklahoma | 72.0 | 6.1 | 3.6 | 131 | High |
| 8 | Kentucky | 67.8 | 4.9 | 4.1 | 124 | Moderate |
| 9 | Nebraska | 67.5 | 5.2 | 3.9 | 128 | Moderate |
| 10 | North Dakota | 64.6 | 17.7 | 3.5 | 111 | High |

## Analyst Notes

The composite score intentionally combines multiple indicators instead of relying on fatality rate alone. A single metric does not capture the whole operational picture.

This ranking should be interpreted as a prioritization tool, not a definitive safety ranking or causal model. It is useful for identifying states that may deserve deeper review.

## Portfolio Value

This project demonstrates:

- Excel-based analytical workflow
- KPI design and metric weighting
- data cleaning and summary reporting
- risk ranking and prioritization logic
- clear communication of findings and limitations

## Recommended Next Evidence

The next improvement is to export workbook screenshots and place them in an `images/` folder, such as:

```text
images/kpi_summary.png
images/top10_risk_states.png
images/risk_score_methodology.png
```

Those screenshots would make the Excel workbook easier to preview without downloading it.
