# Methodology

## Research design

The source project describes a quantitative time-series study of the relationship between HIV/AIDS prevalence and economic growth in Nigeria over 1991–2022. It reports the use of secondary data and EViews 12.

## Data sources

The report identifies the following sources:

- World Bank, World Development Indicators (WDI)
- World Health Organization (WHO)
- Central Bank of Nigeria statistical publications

The exact series identifiers and transformations must be documented after the source files are obtained. Do not assume that similarly named indicators from different sources are interchangeable.

## Variables

- GDP: GDP growth rate / economic growth measure (the source report alternates between GDP and GDP growth rate; verify the exact series).
- HA: HIV/AIDS prevalence.
- PSH: public spending on health.
- LE: life expectancy at birth.

Record the exact indicator name, indicator code, unit, source, and transformation for each series in `data/DATA_DICTIONARY.md`.

## Model 1: Economic growth

The source document specifies:

\[
GDP_t = \beta_0 + \beta_1 HA_t + \beta_2 PSH_t + \beta_3 LE_t + u_t
\]

GDP is the dependent variable; HA, PSH, and LE are explanatory variables.

## Model 2: HIV/AIDS prevalence

The source document specifies:

\[
HA_t = \alpha_0 + \alpha_1 GDP_t + \alpha_2 PSH_t + \varepsilon_t
\]

HA is the dependent variable; GDP and PSH are explanatory variables.

## Reported estimation outputs

The report presents descriptive statistics, a correlation matrix, and multiple-regression results. It reports using EViews 12. This repository does not yet contain the raw data or executable estimation code, so the published estimates are not independently reproducible at this stage.

## Recommended reproducibility and diagnostics workflow

Before drawing conclusions from a new estimation:

1. Verify the variable definitions, units, frequency, and source series.
2. Check the year coverage, missing observations, outliers, and any changes in statistical definitions.
3. Plot each series and inspect its time-series properties.
4. Assess stationarity and choose a suitable specification for the properties of the data.
5. Estimate the specified models and report coefficient estimates, standard errors, p-values, confidence intervals, sample size, and model fit.
6. Conduct appropriate residual diagnostics, including serial-correlation tests. A Durbin–Watson statistic below 2 does not alone prove the presence or absence of serial correlation.
7. Distinguish statistical association from causal effects.
8. Record software versions and make the code and cleaned data available where licensing permits.

This workflow is a recommendation for strengthening reproducibility; it is not a claim that these additional tests were completed in the original project.
