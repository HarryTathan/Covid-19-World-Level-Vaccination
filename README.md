# Covid-19-World-Level-Vaccination

**An Analysis of the Global COVID-19 Vaccination Rollout**

This repository contains a comprehensive exploratory data analysis (EDA) of the global COVID-19 vaccination campaign, using a real-world, time-series dataset from "Our World in Data." The project demonstrates a complete analytical workflow, moving from robust data cleaning and preprocessing to advanced, insightful visualizations that tell the story of one of the largest public health initiatives in history.

# 1. Project Goal
The primary objective of this project was to clean, analyze, and visualize the complex vaccination dataset to answer key questions about the global rollout. The analysis aimed to uncover trends, compare national strategies, and explore the socio-economic factors influencing vaccination success.

**Key analytical questions:**

What was the overall timeline and scale of the global vaccination effort?

Which countries were the leaders in both total and per-capita vaccination rates?

What was the relationship between a country's wealth and its vaccination success?

# 2. Workflow & Key Methodologies
This project followed a structured, multi-stage workflow to ensure analytical rigor and produce insightful conclusions.

# a. Data Cleaning & Preprocessing

The most critical step was handling the extensive missing values inherent in the time-series data. A simple fillna(0) would have been analytically incorrect. Instead, a robust imputation strategy was implemented:

The date column was converted to a proper datetime format.

The data was sorted by country and date to establish a correct time-series.

A grouped forward-fill (ffill) was applied to all core time-series metrics. This correctly handles reporting lags by assuming the value on a non-reported day is the same as the last known value.

# b. Exploratory Data Analysis (EDA)

The analysis moved from a high-level global view to specific, granular insights. Key visualizations included:

A time-series plot of the global daily vaccination trend.

An interactive choropleth map showing vaccinations per 100 people for a fair comparison of national efforts.

Ranked bar charts of the top and bottom 10 performing countries.

A breakdown of the most widely adopted vaccine types.

<img width="945" height="489" alt="1" src="https://github.com/user-attachments/assets/73442274-2ec3-4da8-a7b0-bdf00e2c6a29" />

# c. Advanced & Creative Analysis

To go beyond a simple descriptive report, several advanced techniques were employed:

**Rolling Averages:** A 7-day rolling average was applied to the noisy daily data to reveal the true underlying trends of campaign acceleration and peaks.

**"Time to Milestone" Benchmarking:** A more sophisticated comparison of rollout speed was created by calculating the number of days it took for top countries to reach a key milestone (25 doses per 100 people).

**Data Enrichment:** The project was elevated by integrating an external dataset for GDP per capita. This allowed us to perform a socio-economic analysis and test the real-world hypothesis about the link between a country's wealth and its vaccination rate.


**EDA and Visualizations using ptyhon**

<img width="935" height="545" alt="2" src="https://github.com/user-attachments/assets/5e6e53f3-9d26-4586-88a2-3e6f848b71ff" />
<img width="947" height="718" alt="3" src="https://github.com/user-attachments/assets/1a156d26-0d80-4bae-a683-bd31c8e52132" />
<img width="945" height="480" alt="4" src="https://github.com/user-attachments/assets/81ada7f8-d6e6-44b9-9297-a23ae908dd66" />
<img width="960" height="477" alt="5" src="https://github.com/user-attachments/assets/cbed1b9b-6edf-4587-bef9-5d0d01328c6a" />
<img width="930" height="336" alt="6" src="https://github.com/user-attachments/assets/eee901b4-94c4-4a93-89c3-0c1ed4098ab4" />
<img width="942" height="564" alt="7" src="https://github.com/user-attachments/assets/ea3a79dd-2773-4611-9e85-891952f6d665" />
<img width="953" height="333" alt="8" src="https://github.com/user-attachments/assets/2e9f378f-9ef8-4ae1-bb7c-2fe86b004fb8" />
<img width="941" height="554" alt="9" src="https://github.com/user-attachments/assets/7a287102-1228-4d90-9737-cd1d15429e36" />

# 3. Key Findings & Conclusion
This analysis successfully transformed a raw, messy dataset into a set of clear, actionable insights.

**Our main findings include:**

**Global Disparity:** There was a stark contrast between the vaccination campaigns in different nations. The analysis of per-capita rates and rollout speed revealed that smaller, well-organized countries were often the most efficient.

**The Wealth-Health Correlation:** Our data enrichment analysis confirmed a strong positive correlation between a country's GDP per capita and its ability to achieve a high vaccination rate, highlighting the significant global inequalities in the response to the pandemic.

**The Backbone of the Campaign:** The analysis of vaccine types showed that a few key vaccines, particularly Oxford/AstraZeneca and Pfizer/BioNTech, were the most widely adopted and formed the foundation of the initial global effort.

# 5. Technologies Used

**Data Analysis:** Python, Pandas, NumPy

**Data Visualization:** Matplotlib, Seaborn, Plotly Express

**Development Environment:** Jupyter Notebook / Google Colab



# POWER BI (Visualizations)

# Interactive Dashboard Companion (Power BI)
To complement the deep-dive analysis in Python, an interactive analysis was done in Power BI to provide a high-level, accessible summary of the key findings for a non-technical audience.


# Key Features represented:
**Vaccine Availability:** 

An interactive map and slicers that allow users to select a specific vaccine and instantly see all the countries where it has been administered.

**Hierarchical Drill-Down:** 

A treemap visual that provides a clear overview of the Country -> Vaccine relationship.

**Quarterly Performance Tracking:**

A column chart that tracks the progress of people_fully_vaccinated vs. people_vaccinated on a quarter-by-quarter basis, clearly visualizing the "completion gap" over time.


<img width="1306" height="725" alt="1" src="https://github.com/user-attachments/assets/c570a5b1-d690-4855-98a0-0007773dbd48" />
<img width="592" height="728" alt="2" src="https://github.com/user-attachments/assets/1daf0a36-6e8c-4525-be27-fe5985babaa0" />
<img width="1272" height="712" alt="3" src="https://github.com/user-attachments/assets/026c50eb-e683-4f51-ad06-92285663d7d9" />

