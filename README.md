
# Diversity & Inclusion Dashboard

## Table of Content
- [Discription](#Discription)
- [Project Background](#Project-Background)
- [Key Skills](#Key-Skills)
- [Key Performance Indicators](#Key-Performance-Indicators)
  - [Calculated Measured KPIs](#Calculated-Measured-KPIs)
    - [Hiring Measures](#Hiring-Measures)
    - [Promotion Measures](#Promotion-Measures)
    - [Performance and Turnover Measures](#Performance-and-Turnover_Measures)
  



---------------------------------------------------------------------------------------------------------------------------------------------------------------

## Discription
This project tackled the challenge of improving gender balance in a telecom client's executive management. I leveraged  **data analysis techniques**  to assess their diversity and inclusion efforts. This involved **creating a Power BI dashboard** to visualize key metrics and **designing KPIs**. The project aimed to provide data-driven insights to facilitate informed decision-making.

---------------------------------------------------------------------------------------------------------------------------------------------------------------

## Project Background
Human Resources at a telecom company is highly into diversity and inclusion. They’ve been working hard to improve gender balance at the executive management level, but they’re not seeing any progress.

They’re reaching out to help them in the analysis and create visualizations to -
- Represent HR data, particularly focusing on gender-related KPIs
- Identify and discuss potential root causes for the slow progress in achieving gender balance at the executive management level.

---------------------------------------------------------------------------------------------------------------------------------------------------------------

## Key Skills
- Data Cleaning
> Using Power Query I removed Null values, Duplicate values and Errors from the dataset.
- Data Transformation
> Transformed the data by eleminating Unwanted Columns, hiding irrelevant tables and creating conditional columns.
- Data Analysis
> Performed data analysis by discovering pattern and trends in the report.
- Data Visualization
> Created visualizations by adding different visuals like bar chart, time-series chart, slicers, card visual and gauge visual.

---------------------------------------------------------------------------------------------------------------------------------------------------------------

## Key Performance Indicators
KPIs, or Key Performance Indicators, are like goal markers for businesses. They're specific, measurable values that track progress towards achieving important objectives. They are like a dashboard that shows how well a company is doing on its journey to success. By following these KPIs, businesses can make smart decisions based on real data and identify areas where they can improve.

### Calculated Measured KPIs
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
