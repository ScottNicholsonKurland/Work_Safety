# Workplace Safety Risk Analysis — Project Summary

## Project Purpose

This project analyzes 2012 U.S. workplace safety data by state and creates a composite risk score to compare states on fatality rates, injury and illness rates, inspection capacity, and penalty levels.

The goal is not to prove causation. The goal is to demonstrate analyst judgment: define useful metrics, clean and summarize public data, rank operational risk, and explain the limits of the result.

## Business Question

Which U.S. states appear to have the highest workplace safety risk when fatalities, injuries, inspection delay, and penalty levels are considered together?

## Method

The project uses a weighted composite score:

```text
Risk Score =
  0.40 × fatality-rate percentile
+ 0.25 × injury-rate percentile
+ 0.25 × inspection-delay percentile
+ 0.10 × inverse-penalty percentile
```

This gives the most weight to fatality rates, while still accounting for broader safety burden, inspection capacity, and penalty levels.

## Headline KPIs

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

## Top Risk States

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

## Interpretation

The composite score is a prioritization tool. It does not prove that one state is objectively more dangerous than another, and it does not explain causation. It helps identify states that may deserve closer review based on multiple operational safety indicators.

## Analyst Skills Demonstrated

- Excel-based data analysis
- CSV cleaning and summary reporting
- KPI design
- metric weighting
- risk ranking
- clear communication of limitations
