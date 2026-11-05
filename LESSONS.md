# LESSONS.md

Short notes on corrections, preferences, and mistakes. Each line: what happened, then the rule for next time.

## Corrections and preferences
- Reviewed the cleaning notebook and offered fixes; user said none needed. Rule: when reviewing their code, report findings only and don't edit or rewrite it unless asked.

- User gave two sample notebooks (Tables and Figures, OLS) as the model. Rule: mimic them. Setup cell, then numbered sections with a short text cell. Print the weighted table (`groupby` + `wmean`, 1 decimal), then chart it. Regressions use `wls` with `asecwt`, `HC1` errors, outcome in percent.
- User said table and chart prompts must use the variables and coding from NEET_data_cleaning.ipynb. Rule: use them as saved in neet_data.csv; do not rebuild or recode them.

## Errors and causes
- (none yet)
