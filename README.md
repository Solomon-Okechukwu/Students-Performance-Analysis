# Students-Performance-Analysis
Analysis of students' performance data to uncover insights that can help improve academic outcomes and boost school enrollment

## Table of Contents

- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/Findings](#resultsfindings)
- [Recommendation](#recommendation)
- [Dashboard Preview](#dashboard-preview)
- [Limitations](#limitations)
- [References](#references)
  
## Project Overview
The project “Analyzing Student Performance to Drive Enrollment Growth” aims to examine students’ academic data to identify factors affecting their performance. By analyzing trends across gender, race/ethnicity, parental education, lunch type, and test preparation, the project seeks to uncover key drivers of success. The insights will help the school design strategies to improve academic outcomes, enhance its reputation, and attract more student enrollments.

## Objectives
Analyze student performance data to identify key factors influencing academic outcomes.
- Examine trends in math, reading, and writing scores across gender, race/ethnicity, and parental education levels.
- Assess the impact of lunch type and test preparation on student performance.
- Determine the strongest predictors of high academic achievement.
- Provide actionable recommendations to improve student performance.
- Link improved academic results to strategies for increasing student enrollment.

## Data Source
The dataset for this project contains student academic performance records, focusing on factors that influence exam outcomes.
It includes details such as gender, race/ethnicity, parental level of education, lunch type, test preparation status, and scores in math, reading, and writing.
The data is used to analyze performance trends, identify key drivers of academic success, and develop strategies to improve results and boost student enrollment.
[Access Raw Data](https://github.com/Solomon-Okechukwu/Students-Performance-Analysis/blob/main/Student-Performance-Analysis-Raw.csv)  
[Access Cleaned Data](https://github.com/Solomon-Okechukwu/Students-Performance-Analysis/blob/main/Student_Performance_scores_cleaned%20(1).csv)

## Tools
- Python – for data cleaning, preparation, and analysis [Download_Python](https://www.python.org/downloads/)  
- Power BI – for data visualization and dashboard creation [Download_Power_BI](https://powerbi.microsoft.com/)  
- Microsoft Excel – for dataset storage and initial data inspection [Download_Microsoft_Excel](https://www.microsoft.com/microsoft-       365/excel)  
- GitHub – for project documentation and sharing [Download_GitHub](https://github.com/)  

## Data Cleaning/Preparation
Data was cleaned and prepared using Python before visualization in Power BI.  
The main steps included:
- Loaded the dataset using Pandas and inspected for missing or inconsistent values.
- Verified that the first row contained column headers.
- Checked and standardized data types (e.g., scores as numeric, categorical fields as strings).
- Removed duplicates to ensure each student record appeared only once.
- Standardized categorical values for consistency (e.g., "female" → "Female", "male" → "Male").
- Handled missing values by filling or removing incomplete records where necessary.
- Checked for and corrected typos or inconsistent text entries in columns like “Parental Level of Education” and “Race/Ethnicity.”
- Created new calculated columns:
  - **Average Score** – computed as the mean of math, reading, and writing scores.
  - **Performance Level** – categorized students into performance groups (e.g., High, Medium, Low) based on their average score.
- Renamed columns for clarity and readability.

## Exploratory Data Analysis
EDA involves exploring the student performance data to answer key academic and strategic questions such as:
- Analyze overall performance in math, reading, and writing.
- Identify performance trends across gender, race/ethnicity, and parental education levels.
- Examine how lunch type (standard or free/reduced) affects academic outcomes.
- Evaluate the impact of completing a test preparation course on student scores.
- Determine which demographic groups perform best or need additional academic support.
- Identify correlations among math, reading, and writing scores.
- Uncover key factors driving high performance to guide school improvement strategies.
- Provide insights on how academic improvements can enhance the school’s reputation and attract more student enrollments.

## Data Analysis
Data analysis was conducted in **Python** using Jupyter Notebook to explore and derive insights from the student performance dataset.  

The analysis steps included:
- Computing descriptive statistics (mean, min, max) for Math, Reading, and Writing.
- Creating an **Average Score** column and classifying students into **Performance Levels** (High, Medium, Low).
- Comparing scores across **Gender**, **Race/Ethnicity**, and **Parental Level of Education**.
- Evaluating how **Lunch Type** and **Test Preparation Course** affect performance.
- Checking correlations between Math, Reading, and Writing scores using a heatmap.
- Detecting outliers using the **IQR (Interquartile Range)** method.
- Exporting summarized results to Power BI for visualization.

**See full Python analysis here:**  
[View Python Notebook](https://github.com/Solomon-Okechukwu/Students-Performance-Analysis/blob/main/Student_Dataset%20Notebook.ipynb).

## Results/Findings
The results of the analysis are summarized as follows:
  
#### Student Demographics
- Gender: Female students slightly outperform males across all subjects — particularly in reading and writing.
- Parental Education: Students whose parents hold a bachelor’s degree or higher consistently achieve higher average scores compared to those whose parents have only high school or some   college education.
- Race/Ethnicity: Group E students record the highest average scores, while Group A students perform the lowest overall.
  
#### Academic Performance Trends
- Subject Scores:
Math: Average ≈ 66
Reading: Average ≈ 70
Writing: Average ≈ 68
Reading scores are generally higher than math scores across all demographics.

Performance Correlation: Strong positive correlation between Reading and Writing scores (≈ 0.95), indicating that students who perform well in one tend to perform well in the other..
  
#### Socialeconomic Factors
- Lunch Type: Students receiving standard lunch perform significantly better in all subjects than those on free/reduced lunch, showing the impact of socioeconomic background on
  performance.
- Test Preparation Course: Students who completed a test preparation course scored 10–15 points higher on average across all subjects compared to those who did not.
  
#### Performance Distribution
- Top Performers: Students with average scores above 80 are classified as High Performers — mostly those with educated parents and who completed test prep.
- Low Performers: Students with average scores below 60 are mainly from lower parental education levels and those who didn’t complete test preparation.

## Dashboard Preview
  Here is an overview of the Car Sales Performance Dashboard
  ![Dashboard Overview](Car%20Sales%20Dashboard.PNG)

## Recommendation
- Introduce free or subsidized test preparation courses to improve overall student scores.
- Provide nutrition support or lunch improvement programs for students on free/reduced lunch to bridge performance gaps.
- Encourage greater parental engagement, especially among families with lower education levels.
- Develop targeted academic support programs for underperforming demographic groups (e.g., specific race/ethnicity clusters).
- Use improved student results in marketing campaigns to attract more enrollments and strengthen the school’s academic reputation.
- Continuously track performance metrics by gender, parental education, and socioeconomic status to guide data-driven improvement strategies..

## Limitations
During the analysis, several data quality issues were identified and addressed:
- Inconsistent Text Entries: Corrected spelling and formatting issues such as “female” → “Female” and “bachelor’s degree ” → “Bachelor’s degree”.
- Missing Data: A few records had incomplete information (e.g., parental education or lunch type) and were excluded from analysis.
- Outliers: Unusually high or low test scores were reviewed and filtered using the IQR method to prevent skewed averages.
- Categorical Standardization: Race/ethnicity and parental education levels were grouped into predefined categories for consistency.

Limitations:

- Removing outliers and incomplete records may slightly affect the overall average scores.
- Grouping demographic variables (e.g., education levels, race/ethnicity) may mask subtle differences between subgroups.
- The dataset represents a specific sample, which may not fully reflect broader student populations or real-world diversity.
- Limited socioeconomic variables mean deeper insights into external factors (like income or school type) couldn’t be explored.

## References
- Dataset Source: Kaggle – Students Performance in Exams
- Python Libraries: Pandas, NumPy, Matplotlib, and Seaborn (for data cleaning, analysis, and visualization).
- Visualization Tool: Microsoft Power BI – used for dashboard creation and performance trend visualization.
- Personal study notes.

😄
💻
📊

| Tool | Purpose |
|------|----------|
| Excel | Used for basic data exploration and cleaning before visualization. |
| Power BI | Used for creating interactive dashboards and insights visualization. |
| Python | Used for data cleaning, analysis, and generating statistical insights. |


