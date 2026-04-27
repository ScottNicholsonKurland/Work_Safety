# 2012 U.S. Workplace Safety Analysis

## Overview

This project analyzes state-level workplace safety outcomes in the United States using 2012 workplace injury, illness, fatality, inspection, and penalty data.

The goal is to identify which states appear to have the highest relative workplace safety risk, using both direct outcome measures and operational enforcement indicators. The analysis combines cleaned state-level data, derived metrics, summary KPIs, and a composite risk score designed to make state comparisons easier to interpret.

This project was built as a practical data analysis portfolio piece using Excel and CSV-based analysis outputs.

## Business Question

Which U.S. states show the highest relative workplace safety risk when comparing fatality rates, injury rates, inspection capacity, and penalty patterns?

A simple ranking by fatalities alone can be misleading because larger states naturally have more workers and more incidents. This analysis instead compares states using normalized rates and derived indicators.

## Key Findings

- **West Virginia** had the highest composite risk score: **84.5**
- **North Dakota** had the highest fatality rate in the dataset: **17.7**
- The **median state fatality rate** was **3.5**
- The U.S. overall had approximately **625.9 injuries per fatality**

These findings suggest that smaller or resource-intensive states may show elevated workplace safety risk when outcomes are normalized by rate rather than viewed only as raw incident counts.

## Methodology

The analysis used cleaned state-level workplace safety data and created several derived metrics to compare states more fairly.

### Derived Metrics

| Metric | Definition | Purpose |
|---|---|---|
| Injuries per Fatality | Injuries and illnesses / fatalities | Measures the relationship between nonfatal and fatal workplace outcomes |
| Relative Fatality Rate vs. U.S. | State fatality rate / U.S. fatality rate | Compares each state against the national baseline |
| Composite Risk Score | Weighted percentile score | Ranks states across multiple safety and enforcement indicators |

### Composite Risk Score

The composite risk score uses the following weighting:

```text
Risk Score =
0.40 × fatality-rate percentile
+ 0.25 × injury-rate percentile
+ 0.25 × inspection-delay percentile
+ 0.10 × inverse-penalty percentile
