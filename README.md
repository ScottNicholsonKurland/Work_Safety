# Workplace Safety Analysis (GitHub-ready)

## Files
- `cleaned_state_data.csv` — cleaned state-level dataset with derived metrics
- `summary_kpis.csv` — compact headline metrics
- `top10_risk_states.csv` — highest-risk states based on the composite score
- `correlation_matrix.csv` — correlations among major numeric variables
- `workplace_safety_summary.xlsx` — formatted Excel workbook with overview, cleaned data, rankings, and correlations

## Cleaning performed
- Used the workbook's `Cleaned Data` sheet as the canonical source because it already resolved the major missing-data issues in the raw CSV.
- Removed the empty helper column (`Unnamed: 12`).
- Removed the U.S. aggregate row from state-level ranking analysis.
- Corrected one state code typo: `NB` -> `NE`.
- Standardized numeric columns and added full state names.

## Derived metrics
- **Injuries per Fatality** = injuries and illnesses / fatalities
- **Relative Fatality Rate vs US** = state fatality rate / U.S. fatality rate
- **Risk Score** = 0.40 × fatality-rate percentile + 0.25 × injury-rate percentile + 0.25 × inspection-delay percentile + 0.10 × inverse-penalty percentile

Higher **Risk Score** means a state appears riskier relative to peers based on incident rates and inspection capacity constraints.

## Highlights
- Highest composite risk score: **West Virginia** (84.5)
- Highest fatality rate in the dataset: **North Dakota** (17.7)
- Median state fatality rate: **3.5**
- U.S. injuries per fatality: **625.9**
