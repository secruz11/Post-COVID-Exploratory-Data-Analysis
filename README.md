# Exploring Long COVID Outcomes in the United States

## Project Overview

This project explores patterns in **Long COVID prevalence, activity limitations, and racial/ethnic disparities in the United States** through exploratory data analysis (EDA).

Using national survey data from the U.S. Department of Health & Human Services, the analysis examines how common Long COVID is relative to prior COVID infection, how Long COVID affects daily activity, and how prevalence varies across racial and ethnic groups.

## Research Questions

1. How do national COVID and Long COVID prevalence measures compare?
2. How do activity limitations differ between adults with Long COVID and the overall adult population?
3. Do Long COVID rates differ by race/ethnicity?

## Dataset

The analysis uses the **Post-COVID Conditions** dataset published by the U.S. Department of Health & Human Services and available through Data.gov.

* **18,639 observations**
* **16 variables**
* Survey data spanning multiple time periods
* Includes COVID and Long COVID prevalence estimates
* Includes demographic subgroups such as age, sex, race/ethnicity, disability status, education level, and state

Key variables include `Indicator`, `Group`, `Subgroup`, `Value`, confidence interval measures, and survey time-period variables.

## Tools & Technologies

* Python
* Pandas
* Matplotlib
* Jupyter Notebook

## Data Preparation

The data were prepared for analysis by:

* Standardizing column names
* Converting percentage values to numeric format
* Converting survey dates to datetime format
* Evaluating missing values
* Excluding missing `Value` observations when necessary for visualization
* Filtering observations to the most recent survey period for selected comparisons
* Examining the use of different population denominators across indicators

## Exploratory Data Analysis

The analysis included:

* Examination of the overall distribution of reported percentage values
* Identification and interpretation of apparent outliers
* Comparison of national COVID and Long COVID prevalence
* Comparison of activity limitations among adults with Long COVID versus the overall adult population
* Comparison of current Long COVID prevalence across racial and ethnic groups

## Key Findings

### COVID vs. Long COVID Prevalence

Approximately **60% of adults reported ever having COVID**, while roughly **18% reported ever experiencing Long COVID** and approximately **6% reported currently experiencing Long COVID**.

This indicates that Long COVID affects a smaller subset of individuals who have experienced COVID.

### Activity Limitations

Although current Long COVID prevalence is relatively low within the overall adult population, its impact is substantial among individuals experiencing it.

Approximately:

* **80%** of adults with Long COVID reported **any activity limitations**
* **22%** reported **significant activity limitations**

This comparison also demonstrates the importance of considering the population denominator when interpreting health statistics.

### Racial and Ethnic Differences

Current Long COVID prevalence differed across racial and ethnic groups in the most recent survey period.

* **Highest observed prevalence:** Non-Hispanic adults identifying as other or multiple races — **7.3%**
* **Lowest observed prevalence:** Non-Hispanic Asian adults — **2.8%**

The difference between the highest and lowest observed groups was approximately four percentage points.

## Limitations

Several limitations should be considered when interpreting these results:

* Survey responses are self-reported and may be subject to reporting or interpretation bias.
* Different indicators use different population denominators, limiting direct comparison between some percentages.
* Missing values may affect the results.
* The analysis is exploratory and descriptive; **no causal relationships are inferred**.

Future analyses could incorporate additional variables such as socioeconomic status and initial infection severity.

## Conclusion

The analysis shows that although Long COVID affects a smaller portion of the population than prior COVID infection, individuals experiencing Long COVID can face substantial activity limitations.

Differences in current Long COVID prevalence were also observed across racial and ethnic groups. Together, these findings highlight the importance of examining not only the prevalence of Long COVID, but also its impact among affected populations and differences across demographic groups.

## Repository Contents

* `Post Covid EDA.ipynb` — Python notebook containing data preparation, exploratory analysis, and visualizations
* `Post Covid EDA.pdf` — Full written project report
* `README.md` — Project overview and key findings
* Dataset — Post-COVID Conditions data used for the analysis

## Data Source

**U.S. Department of Health & Human Services — Post-COVID Conditions**
Published through Data.gov / Centers for Disease Control and Prevention.
