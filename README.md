# hiv-aids-economic-growth-nigeria.
HIV/AIDS Prevalence and Economic Growth in Nigeria (1991–2022)

An undergraduate Economics research project examining the two-way relationship between HIV/AIDS prevalence and economic growth in Nigeria using annual time-series data.



Research note: This repository documents the research design and reported findings in the original project. The underlying dataset and reproducible analysis files have not yet been added, so the numerical results should be treated as reported results from the original study rather than independently reproduced estimates.



Research questions


What is the effect of HIV/AIDS prevalence on economic growth in Nigeria?

How does economic growth relate to HIV/AIDS prevalence in Nigeria?


Study objectives


Examine the effect of HIV/AIDS prevalence on economic growth in Nigeria.

Examine the effect of economic growth on HIV/AIDS prevalence in Nigeria.


Study period and data


Country: Nigeria

Period: 1991–2022

Frequency: Annual time series

Sources identified in the project: World Bank World Development Indicators (WDI), World Health Organization (WHO), and Central Bank of Nigeria statistical publications.

Software reported: EViews 12


The project describes the study as using secondary data. The exact series names, indicator codes, units, and transformations should be recorded in data/DATA_DICTIONARY.md once the source dataset is assembled.


Variables and model specification

The project uses four main variables:


Symbol	Variable	Role in the reported model
GDP	GDP growth rate / economic growth proxy	Dependent variable in Model 1; explanatory variable in Model 2
HA	HIV/AIDS prevalence	Explanatory variable in Model 1; dependent variable in Model 2
PSH	Public spending on health	Explanatory variable in both models
LE	Life expectancy at birth	Explanatory variable in Model 1

The two equations as specified in the source document are:


Model 1 — Economic growth


[
GDP_t = \beta_0 + \beta_1 HA_t + \beta_2 PSH_t + \beta_3 LE_t + u_t
]


Model 2 — HIV/AIDS prevalence


[
HA_t = \alpha_0 + \alpha_1 GDP_t + \alpha_2 PSH_t + \varepsilon_t
]


The source document uses GDP growth rate in the results discussion, while its model specification sometimes refers more generally to GDP. The precise indicator definition and units should be confirmed against the original dataset before reproducing the estimates.


Findings reported in the original project

The document reports the following regression equations and fit statistics:



Model 1: GDP growth rate = -47.53350 + 0.544LE + 14.968HA + 0.013PSH; reported (R^2 = 0.411502), Durbin–Watson = 1.541874, and F-statistic = 3.729219.

Model 2: HA = 1.107 + 0.024GDP + 0.025PSH; reported (R^2 = 0.626073), Durbin–Watson = 0.935106, and F-statistic = 14.23169.


These are transcribed as reported, not independently validated. Some interpretations and statistical descriptions in the source document appear inconsistent with the reported coefficients/statistics. In particular, Durbin–Watson values below 2 do not, by themselves, establish the absence of serial correlation; the test requires more careful interpretation. The repository should not present these findings as causal evidence without further diagnostics and a reproducible re-estimation.


Repository structure

.
├── README.md
├── data/
│   ├── DATA_DICTIONARY.md
│   └── README.md
├── docs/
│   └── METHODOLOGY.md
├── notebooks/
│   └── README.md
├── outputs/
│   └── README.md
└── requirements.txt

Reproducibility status

At present, this is a research documentation scaffold. To make the project reproducible:



Obtain and archive the annual source series for 1991–2022.

Record indicator codes, units, source URLs, retrieval date, and any transformations.

Clean and merge the series by year, checking missing values and changes in definitions.

Re-estimate both models and document diagnostics, including stationarity and serial-correlation checks as appropriate.

Export cleaned data, code/notebooks, regression tables, and charts to this repository.

Compare the reproduced estimates with the values reported in the original document and explain any differences.


Limitations


The raw dataset and estimation files are not included yet.

The reported results have not been independently reproduced.

The source document's descriptions of variables, units, and some statistical tests need verification.

Regression associations alone do not establish causation.

HIV/AIDS is a sensitive public-health topic; analysis should be reported respectfully and without stigmatizing people living with HIV.


Suggested next steps


Add the original project report in a clearly named docs/ file if you have permission to share it.

Add a source-data file only after checking source licensing and documenting the indicator definitions.

Create a Python or R notebook that imports, cleans, visualizes, and estimates the models.

Add plots for the time trends, correlation matrix, and model diagnostics.


Citation

If you use this repository, cite the original undergraduate research project and add the author's name, institution, department, and submission year here before publishing. Those details were not inferred in this README because they should be copied accurately from the title page of the report.

