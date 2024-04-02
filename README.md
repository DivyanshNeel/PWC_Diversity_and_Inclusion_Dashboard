
# Diversity & Inclusion Dashboard

# Table of Content
- [Discription](#Discription)
- [Project Background](#Project-Background)
- [Key Learning Skills](#Key-Learning-Skills)
- [Key Performance Indicators](#Key-Performance-Indicators)
  - [Calculated Measured KPIs](#Calculated-Measured-KPIs)
    - [Hiring Measures](#Hiring-Measures)
    - [Promotion Measures](#Promotion-Measures)
    - [Performance and Turnover Measures](#Performance-and-Turnover_Measures)
- [Insights and Recommendation ](#Insights-and-Recommendation)
  



---------------------------------------------------------------------------------------------------------------------------------------------------------------

# Discription
This project tackled the challenge of improving gender balance in a telecom client's executive management. I leveraged  **data analysis techniques**  to assess their diversity and inclusion efforts. This involved **creating a Power BI dashboard** to visualize key metrics and **designing KPIs**. The project aimed to provide data-driven insights to facilitate informed decision-making.

---------------------------------------------------------------------------------------------------------------------------------------------------------------

# Project Background
Human Resources at a telecom company is highly into diversity and inclusion. They’ve been working hard to improve gender balance at the executive management level, but they’re not seeing any progress.

They’re reaching out to help them in the analysis and create visualizations to -
- Represent HR data, particularly focusing on gender-related KPIs
- Identify and discuss potential root causes for the slow progress in achieving gender balance at the executive management level.

---------------------------------------------------------------------------------------------------------------------------------------------------------------

# Key Learning Skills
- Data Cleaning
> Using Power Query I removed Null values, Duplicate values and Errors from the dataset.
- Data Transformation
> Transformed the data by eleminating Unwanted Columns, hiding irrelevant tables and creating conditional columns.
- Data Analysis
> Performed data analysis by discovering pattern and trends in the report.
- Data Visualization
> Created visualizations by adding different visuals like bar chart, time-series chart, slicers, card visual and gauge visual.

---------------------------------------------------------------------------------------------------------------------------------------------------------------

# Data Source 
PwC provided the dataset as an excel file from the Human Resources department of a telecom client during the PwC Power BI in Data Analytics Virtual Case Experience. The dataset contained records of 500 employees and included major fields such as Employee ID, Gender, Age Group, Job Level after FY20 Promotions, New Hire FY20, FY20 Performance Rating, FY20 Leaver, Last Department in FY20, Time in Job Level, Promotion in FY20, Last Hire Date, and so on.

---------------------------------------------------------------------------------------------------------------------------------------------------------------

# Tech Stack
- Microsoft Excel
- Microsoft Power BI
- Power Query
- DAX

---------------------------------------------------------------------------------------------------------------------------------------------------------------

# Key Performance Indicators
KPIs, or Key Performance Indicators, are like goal markers for businesses. They're specific, measurable values that track progress towards achieving important objectives. They are like a dashboard that shows how well a company is doing on its journey to success. By following these KPIs, businesses can make smart decisions based on real data and identify areas where they can improve.

## Calculated Measured KPIs
A calculated measured Key Performance Indicator (KPI) is a quantifiable metric that is derived through specific formula to assess performance in a systematic manner. It involves the strategic computation of data points to gauge progress or success against predefined objectives or benchmarks.

1. **Hiring Measures**
- Total no of hire
`= CALCULATE(COUNT('Pharma Group AG'[New hire FY20?]),'Pharma Group AG'[New hire FY20?]="Y")`

 - Number of Female hire 
`= CALCULATE(COUNT('Pharma Group AG'[New hire FY20?]),'Pharma Group AG'[New hire FY20?]="Y",'Pharma Group AG'[Gender]="Female")`

- Number of Male hire 
`= CALCULATE(COUNT('Pharma Group AG'[New hire FY20?]),'Pharma Group AG'[New hire FY20?]="Y",'Pharma Group AG'[Gender]="Male")`

> [!NOTE]
> OTHER MEASURES INCLUDE PERCENTAGE VALUE OF THESE KPIs
---------------------------------------------------------------------------------------------------------------------------------------------------------------

2. **Promotion Measures**
- Total no of Promotions
`= CALCULATE(COUNT('Pharma Group AG'[Promotion in FY21?]),'Pharma Group AG'[Promotion in FY21?]="Yes")`

 - Number of Female Promotions
`= CALCULATE(COUNT('Pharma Group AG'[Promotion in FY21?]),'Pharma Group AG'[Promotion in FY21?]="Yes",'Pharma Group AG'[Gender]="Female")`

 - Number of Male Promotions
`= CALCULATE(COUNT('Pharma Group AG'[Promotion in FY21?]),'Pharma Group AG'[Promotion in FY21?]="Yes",'Pharma Group AG'[Gender]="Male")`

 
> [!NOTE]
> OTHER MEASURES INCLUDE PERCENTAGE VALUE OF THESE KPIs

> [!IMPORTANT]
> THESE KPIs BELONGS TO **FY21**, WE CAN DO THE SAME FY20 .

---------------------------------------------------------------------------------------------------------------------------------------------------------------

3. **Performance and Turnover Measures**
- Total Turnover
  `= CALCULATE(COUNT('Pharma Group AG'[In base group for turnover FY20]),'Pharma Group AG'[In base group for turnover FY20]="Y")`

- Turnover by Females
  `= CALCULATE(COUNT('Pharma Group AG'[In base group for turnover FY20]),'Pharma Group AG'[In base group for turnover FY20]="Y",'Pharma Group AG'[Gender]="Female")`

- Turnover by Males
 `= CALCULATE(COUNT('Pharma Group AG'[In base group for turnover FY20]),'Pharma Group AG'[In base group for turnover FY20]="Y",'Pharma Group AG'[Gender]="Male")`


> [!NOTE]
> OTHER MEASURES INCLUDE PERCENTAGE VALUE OF THESE KPIs

---------------------------------------------------------------------------------------------------------------------------------------------------------------

# Insights and Recommendation 

- In the executive and senior management ranks of the company, there is an absence of diversity, with a majority of men holding these positions. This may suggest that there is a bias in the hiring process and a gender imbalance in promotions among employees. Majority of these employees age between 20 and 40 with predominantly positions acquired by males.

- The promotions for FY21 also have a lack of diversity. Over 60% of the promotions given were taken by men, which is even worse in FY20, which is close to 80%.  Especially, at the junior level that is sales and marketing, around 90% promotion are given to males. The organization should do a survey and maybe provide career growth oportunities to female employees to imporve diversity in promotion for a healthy work culture.

- Most number of employees leaving the organization are males, they belong to the executive and management roles of the company, this has a direct co-relation with their performance ratings in the company. The males at these executive level have a perfomance rating below the targeted value. The company should take a feedback and maybe provide benefits to eliminate the retion rate.

- The turnover rate has been determined to be approximately 87%. A distinct pattern emerges from the analysis, specifically when examining the junior roles within the company. In these positions, the turnover rate remains relatively consistent. However, as we progress to higher seniority levels, we observe a contrasting trend. The turnover rate for males steadily increases, while for females, it steadily decreases.

