# EDA: U.S. Business Formation Statistics

## Libraries Used
- pandas
- matplotlib
- seaborn

## Project Motivation
This project explores weekly U.S. business applications from 2006–2026 to understand changes in total, high-propensity, planned-wage, and corporate applications.

## Files in the Repository
- `code.ipynb`: Jupyter Notebook containing data assessment, cleaning, EDA, visualizations, and conclusions.
- `bfs_us_apps_weekly_nsa.csv`: Weekly Business Formation Statistics dataset.
- `README.md`: Project overview and results summary.

## methodology
This project follows the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** framework, organized into five phases:

1. **Business Understanding:** Defined research questions to investigate business application growth, proportional changes across categories, correlations, and long-term trends.
2. **Data Understanding:** Explored the dataset's structure, data types, reporting periods, and feature definitions.
3. **Data Preparation:** Investigated missing values, duplicates, and statistical outliers. Retained the original observations and created an approximate `Date` feature for chronological analysis.
4. **Modeling/Analysis:** Applied descriptive statistics, distribution analysis, Pearson and Spearman correlations, scatterplots, and time-series visualizations to answer the research questions.
5. **Evaluation:** Interpreted the findings, evaluated limitations, and identified opportunities for further analysis.

## Summary of Results
The analysis of U.S. Business Formation Statistics from 2006 to 2026 revealed five key findings:

1. **Significant growth after 2020:** Average weekly Business Applications (`BA_NSA`) increased from approximately 53,635 before 2020 to 102,795 from 2020 onward, representing a **91.7% increase**.

2. **High-propensity applications did not grow proportionally:** Although High-Propensity Business Applications (`HBA_NSA`) increased after 2020, their growth was smaller relative to total applications. The annual HBA-to-BA share analysis indicates a general decline in the proportion of applications classified as high-propensity.

3. **Strong relationship between WBA and CBA:** Applications with Planned Wages (`WBA_NSA`) and Corporate Business Applications (`CBA_NSA`) showed a strong positive relationship, with **Pearson correlation = 0.956** and **Spearman correlation = 0.914**.

4. **Different relationships among application categories:** BA and HBA were strongly correlated (Pearson = 0.879), while BA showed weak correlations with WBA (0.157) and CBA (0.115). This suggests that total business applications and specific categories follow different patterns.

5. **Distinct long-term trends:** BA showed a substantial and persistent increase after 2020. HBA also increased, while WBA and CBA experienced earlier declines and comparatively limited sustained growth in recent years. The weekly series also revealed recurring fluctuations and unusually large year-over-year changes.

**Overall conclusion:** Total business applications in the United States have increased substantially, but this growth has not been proportional across all application categories. The findings suggest a changing composition of business applications, potentially reflecting differences between broader entrepreneurial activity and applications associated with future employer businesses.



## Acknowledgements
Data source: U.S. Census Bureau Business Formation Statistics.
Blog post: https://medium.com/@farzanfarahaniiii/an-exploratory-analysis-of-weekly-u-s-business-application-data-2006-2026-00ae30a53bb3

