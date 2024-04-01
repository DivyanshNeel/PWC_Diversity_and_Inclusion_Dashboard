
# Diversity & Inclusion Dashboard

## Table of Content
- [Discription](#Discription)
- [Project Background](#Project-Background)
- [Key Skills](#Key-Skills)

## Discription
This project tackled the challenge of improving gender balance in a telecom client's executive management. I leveraged  **data analysis techniques**  to assess their diversity and inclusion efforts. This involved **creating a Power BI dashboard** to visualize key metrics and **designing KPIs**. The project aimed to provide data-driven insights to facilitate informed decision-making.

## Project Background
Human Resources at a telecom company is highly into diversity and inclusion. They’ve been working hard to improve gender balance at the executive management level, but they’re not seeing any progress.

They’re reaching out to help them in the analysis and create visualizations to -
- Represent HR data, particularly focusing on gender-related KPIs
- Identify and discuss potential root causes for the slow progress in achieving gender balance at the executive management level.

## Key Skills
- Data Cleaning
> Using Power Query I removed Null values, Duplicate values and Errors from the dataset.
- Data Transformation
> Transformed the data by eleminating Unwanted Columns, hiding irrelevant tables and creating conditional columns.
- Data Analysis
> Performed data analysis by discovering pattern and trends in the report.
- Data Visualization
> Created visualizations by adding different visuals like bar chart, time-series chart, slicers, card visual and gauge visual.

## Key Performance Indicators
KPIs, or Key Performance Indicators, are like goal markers for businesses. They're specific, measurable values that track progress towards achieving important objectives. They are like a dashboard that shows how well a company is doing on its journey to success. By following these KPIs, businesses can make smart decisions based on real data and identify areas where they can improve.

### Calculated Measured KPIs
1. **Hiring Measures**
- Total no of hire
`= CALCULATE(COUNT('Pharma Group AG'[New hire FY20?]),'Pharma Group AG'[New hire FY20?]="Y")`
 -
 - Percentage of Total hire
 `= DIVIDE([count_of_hire],COUNT('Pharma Group AG'[New hire FY20?]))`
 -

- Number of Female hire 
`= CALCULATE(COUNT('Pharma Group AG'[New hire FY20?]),'Pharma Group AG'[New hire FY20?]="Y",'Pharma Group AG'[Gender]="Female")`
 -

 - Percentage of Female hire 
 `= DIVIDE([count_of_female_hire],[count_of_hire])`
 -

- Number of Male hire 
`= CALCULATE(COUNT('Pharma Group AG'[New hire FY20?]),'Pharma Group AG'[New hire FY20?]="Y",'Pharma Group AG'[Gender]="Male")`
 -
 - Percentage of Male hire
 `= DIVIDE([count_of_male_hire],[count_of_hire])`
 -


2. **Promotion Measures**
- Total no of Promotions
`= CALCULATE(COUNT('Pharma Group AG'[Promotion in FY21?]),'Pharma Group AG'[Promotion in FY21?]="Yes")`
 -
 - Percentage of Total Promotion
 `= DIVIDE([count_employee_promoted_FY21],COUNT('Pharma Group AG'[Promotion in FY21?]))`
 -

 - Number of Female Promotions
`= CALCULATE(COUNT('Pharma Group AG'[Promotion in FY21?]),'Pharma Group AG'[Promotion in FY21?]="Yes",'Pharma Group AG'[Gender]="Female")`
 -
 - Percentage of Female Promotion
 `= DIVIDE([count_female_employee_promoted_FY21],[count_employee_promoted_FY21])`
 -

  - Number of Male Promotions
`= CALCULATE(COUNT('Pharma Group AG'[Promotion in FY21?]),'Pharma Group AG'[Promotion in FY21?]="Yes",'Pharma Group AG'[Gender]="Male")`
 -
 - Percentage of Male Promotion
 `= DIVIDE([count_male_employee_promoted_FY21],[count_employee_promoted_FY21])`
 -

> [!IMPORTANT]
> Key information users need to know to achieve their goal.
3. **Performance and turnover Measures**






