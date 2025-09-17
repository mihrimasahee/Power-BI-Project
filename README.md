# Power-BI-Project

- Built an executive-level sales dashboard using the AdventureWorks dataset to track quarterly and monthly performance.

- Visualized Order Quantities by Region, Product Category, and Order Status using bar and line charts.

- Developed a monthly trend analysis view with filters for Region and Product Category, enabling granular analysis.

- Leveraged Power Query for data cleaning and transformation, and DAX for calculated metrics.

- Created an intuitive user experience with slicers, filters, and dynamic visuals for management reporting.

- Outcome: Delivered a sample report that clearly communicates business performance trends and supports decision-making.

## Tools & Technologies Used

- Power BI Desktop – Data modeling, DAX measures, dashboard design

- Power Query – ETL and data transformation

- SQL – Querying and preparing fact/dimension tables

- Excel – Ad-hoc validation and supporting analysis

- Power BI Service – Publishing dashboards and automating data refresh

- Collaboration Tools – Microsoft Teams, Email for stakeholder alignment

## Improving DAX performance
Use the Table view to examine the data in the report
Use the Performance Analyzer to identify slow visuals and DAX formulas
Test the changes with the Performance Analyzer to ensure improved report efficiency

In DAX, the CROSSJOIN function generates a cartesian product by pairing every row of the first table with every row of the second table. This operation is conducted regardless of any matching column values between the tables. It merges each row from one table with all the rows from the other table.

-Locate the Total Sales field of the area chart from the Table view on your right and select it to view the underlying DAX formula.

-To simplify the DAX formula, eliminate the nested CROSSJOIN and GENERATESERIES functions.

-Instead, use the SUMX function enclosed with a single CROSSJOIN
