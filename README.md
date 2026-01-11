Project Overview
Duration: [Insert timeframe - e.g., September 2024 - January 2025]
Role: Data Analyst | Researcher
Tools: Power BI Desktop, Excel, Power Query, DAX
Industry: Energy & Sustainability
Problem Statement
The Australian government required comprehensive analysis of renewable energy adoption trends to inform policy decisions and track progress toward 2030 sustainability goals.
Methodology
1. Data Collection & Sources

Australian Energy Statistics (Government database)
International energy databases (New Zealand, Papua New Guinea, Indonesia)
Global Renewable Power Sector Targets database
Multiple fiscal year datasets from regional authorities

2. ETL Process

Extracted data from 8+ separate sources (Excel, HTML tables)
Cleaned and standardized inconsistent formats across datasets
Created calculated columns for renewable/non-renewable classification
Merged datasets using fiscal year and country as keys
Transformed wide-format data to long-format for analysis

3. Data Modeling

Designed star schema with fact and dimension tables
Created relationships: Dim_Date, Dim_Country, Dim_Energy_Source
Established one-to-many and one-to-one relationships
Optimized for query performance

4. Analysis & Visualization

Developed 15+ DAX measures for dynamic calculations
Created 4 comprehensive dashboard pages answering key business questions
Built interactive visualizations: line charts, 100% stacked columns, gauge charts, matrix tables
Implemented filters and slicers for user exploration

Key Findings
1. Overall Growth

Renewable energy: 9.34% (2005-06) → 33.92% (2022-23)
328% increase over 18 years

2. Energy Source Transformation

Hydro: Declined from 73.72% to 17.90% of renewable mix
Solar: Exploded from 0.42% to 45.07% (dominant source)
Wind: Projected to be largest contributor by 2030 (40.04%)

3. Regional Comparison

Australia surpassed Indonesia by 2015
Matched New Zealand's strong performance
Overtook Papua New Guinea around 2021

4. 2030 Forecast

Target: 82.64% renewable energy
Gap from current: 48.72%
Wind energy will lead the transition

Technical Implementation
Power Query Transformations:

16 transformation steps per dataset
Custom conditional columns for categorization
Unpivoting for analysis-ready format
Date parsing and standardization

DAX Measures Examples:
% Renewable Energy = 
DIVIDE(
    CALCULATE(SUM('AUS FY'[Value(GWh)]), 
              'AUS FY'[Renewable] = "Renewable Fuel"),
    CALCULATE(SUM('AUS FY'[Value(GWh)]), 
              ALL('AUS FY'[Renewable]))
)
Visualizations Created:

3 KPI cards with dynamic titles
4 line charts for trend analysis
2 matrix tables with conditional formatting
2 100% stacked column charts
1 gauge chart comparing current vs. target
1 donut chart for energy mix

Business Value

Policy Impact: Insights inform government renewable energy strategy
Investment Guidance: Identifies growth opportunities in solar and wind
Performance Tracking: Monitors progress toward 2030 targets
Regional Benchmarking: Contextualizes Australia's performance

Challenges Overcome

Integrating inconsistent data formats across multiple sources
Handling missing values and data quality issues
Creating meaningful comparisons across different measurement systems
Balancing detail with usability in dashboard design

Skills Demonstrated
✅ Business Intelligence & Analytics
✅ Data Cleaning & ETL
✅ Advanced DAX & Power Query M-Code
✅ Data Modeling & Optimization
✅ Statistical Analysis & Forecasting
✅ Data Visualization Best Practices
✅ Stakeholder Communication
✅ Project Documentation
