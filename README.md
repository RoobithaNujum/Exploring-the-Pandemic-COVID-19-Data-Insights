FIRST PHASE : Data Preprocessing - Excel Project

In Excel, the dataset was first cleaned by removing empty rows, handling duplicates, and checking for consistency to ensure that confirmed cases equaled the sum of deaths, recovered, and active cases, with no negative values in new cases or deaths. Derived columns such as Case Fatality Rate (CFR = Deaths/Confirmed), Recovery Rate (Recovered/Confirmed), and Active % (Active/Confirmed) were created for deeper insights. Conditional formatting was applied to highlight key patterns—for example, high fatality rates in red, strong recovery rates in green, and active cases in varying shades based on severity. 

SECOND PHASE : COVID-19 Global Insights Dashboard – Power BI Project

Project Overview
This project explores the COVID-19 pandemic using Power BI, combining multiple datasets into a unified model. The dashboard provides insights into global and country-level spread, severity, recovery, and time-based trends.The report applies data cleaning, star schema modeling, DAX measures, and interactive visualizations to tell a complete story of the pandemic.

Datasets Used
- Exploring the COVID-19 Grouped.xlsx : Daily COVID-19 cases (Confirmed, Deaths, Recovered, Active) per country and date.
- Exploring the COVID-19 Pandemic.xlsx : Country-wise latest snapshot data.
- Exploring the COVID-19_Worldometer_Data.xlsx : Demographics: population, tests, cases per million, continent.
- Dimension_Date.xlsx : Custom calendar/date table for time intelligence (Year, Month, Quarter).
- Exploring the Pandemic COVID-19 Data Insights.pbix : Final Power BI report with all transformations, measures, and visuals.

Data Preparation, Modeling & DAX

The project began with preparing the raw datasets in Excel, where initial cleaning steps such as fixing inconsistent country names, removing null values, trimming extra spaces, and ensuring consistent data types were applied. After cleaning, the data was loaded into Power BI for advanced modeling. A proper dimensional model was created in which a central fact table containing daily case counts was connected to supporting dimension tables such as date, geography, and demographics. Relationships were defined in a star schema structure, ensuring that filters flow from dimensions to the fact table in a controlled manner. This modeling approach allowed flexible slicing and dicing of the data across time, region, and population metrics.

To derive meaningful insights, a series of DAX measures were created. These included basic aggregations (total cases, deaths, recovered, active), calculated rates (fatality, recovery, active percentages), per capita metrics (cases or deaths per million), and time intelligence measures (month-to-date, quarter-to-date, year-to-date). Together, these measures provided both absolute and relative views of the pandemic, enabling analysis across regions and time periods with accuracy and comparability.

Key Insights

- Case outcomes (Recovery vs Death vs Active) provide severity context.
- Some countries show disproportionately high cases per 1M population.
- Mortality (CFR %) varies significantly across continents.
- Growth curves reveal waves of infections in certain time periods.


Conclusion

This project demonstrates how Power BI can transform raw COVID-19 data into actionable insights through:
 - Robust data modeling (star schema).
 - Advanced DAX measures (KPIs & time intelligence).
 - Interactive visualizations (maps, trends, comparisons).
 - The dashboard helps explore global spread, severity, and impact of COVID-19 across countries and time.

