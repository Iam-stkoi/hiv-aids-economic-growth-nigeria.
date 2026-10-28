# Data Dictionary

This file should be completed from the downloaded source files before analysis begins. It documents the exact definitions, sources, units, and processing steps for each variable used in the HIV/AIDS prevalence and economic growth study for Nigeria (1991–2022).

## Variable table

| Repository field | Original indicator name | Source | Indicator code / table | Unit | Transformation | Notes |
|---|---|---|---|---|---|---|
| year | Calendar year | — | — | Year | None | Expected coverage: 1991–2022 |
| gdp_growth | To be verified | To be verified | To be verified | To be verified | To be verified | Source document alternates between GDP and GDP growth rate; verify whether the series is GDP growth (%) or GDP level in constant/nominal terms |
| hiv_prevalence | To be verified | To be verified | To be verified | To be verified | To be verified | Define population group (e.g., adults 15–49, total population), whether the value is percentage or count, and whether the series is prevalence or incidence |
| public_health_spending | To be verified | To be verified | To be verified | To be verified | To be verified | Clarify the spending measure: total government health expenditure, public health expenditure as share of GDP, or another operational definition |
| life_expectancy | Life expectancy at birth (exact series to verify) | To be verified | To be verified | To be verified | To be verified | Confirm the exact series, coverage, and unit used in the original analysis |

## Source metadata to record

- Retrieval date: To be completed from the source files and download logs
- Source URL(s): To be completed
- Access date: To be completed
- Source name and institution: To be completed
- Data version or revision date: To be completed
- Whether the data are annual, quarterly, or monthly: Annual time series (1991–2022)
- Any geographic coverage note: Nigeria
- Any age/sex/population definitions used by the source: To be completed

## Data processing notes

- Missing values: To be completed. State whether missing values were left blank, imputed, or dropped.
- Units: To be completed for each variable after checking the original source.
- Transformations: To be completed. Examples include annual growth rate, log transformation, winsorization, inflation adjustment, or re-basing.
- Revisions applied: To be completed. Record any corrections, redefinitions, or changes in base year.
- Merging logic: To be completed. Explain how the annual series were aligned by year.

## Quality-assurance checklist

Before running analysis, confirm the following:

- The exact indicator name and source for each variable are verified against the downloaded file(s).
- The measurement unit is recorded in the final cleaned dataset.
- The study period covers 1991–2022 without unexplained gaps.
- Any missing values are documented and justified.
- The final dictionary matches the variable names used in the analysis scripts and notebooks.

## Example of final completed record

Use this as a template for the final cleaned version after source verification:

| Repository field | Original indicator name | Source | Indicator code / table | Unit | Transformation | Notes |
|---|---|---|---|---|---|---|
| year | Calendar year | World Bank / WHO / CBN | — | Year | None | 1991–2022 annual series |
| gdp_growth | GDP growth (annual %) | World Bank WDI | NY.GDP.MKTP.KD.ZG | % | Annual percent change | Verify exact WDI indicator definition |
| hiv_prevalence | HIV prevalence, adult (% ages 15–49) | UNAIDS / World Bank | SH.DYN.AIDS.ZS | % | None | Confirm whether this is the exact series used |
| public_health_spending | Government health expenditure | World Bank / CBN | To be verified | Local currency or % of GDP | To be verified | Clarify whether nominal or real and whether public expenditure share is used |
| life_expectancy | Life expectancy at birth, total (years) | World Bank WDI | SP.DYN.LE00.IN | Years | None | Confirm exact series and year coverage |

This table is intentionally left as a placeholder until the actual source files are inspected and the series definitions are validated.
