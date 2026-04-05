* Dataset Overview



The data used in this project is imported from Excel files and organized using a fact and dimension table structure. The dataset includes the following tables:



Date\_Dim – Contains calendar information such as year, month, and date details.

Customer\_Dim – Stores customer information and segmentation data.

Product\_Dim – Includes details about products.

Sales\_Fact – Holds the main sales transaction records.

Returns\_Fact – Contains information related to returned sales.

Region\_Dim – Stores geographic and regional data for analysis.



This structure ensures better performance and supports scalable reporting





* Data Modeling



The data model follows a star schema design, where fact tables are connected with dimension tables using primary and foreign key relationships.





* DAX Measures \& Calculated Columns



Several DAX formulas are implemented to create KPIs and analytical measures. Functions such as CALCULATE, FILTER, ALL, SUMX, COUNTX, and AVERAGEX are used for advanced calculations



Additionally, calculated columns are created for tasks such as:



Generating Customer Full Name by combining first and last names

Creating Profit Margin categories

Building Year-Month formatted fields to support time-based reportingTime Intelligence





* Time Intelligence



Time intelligence plays a key role in this dashboard. Various calculations are implemented to track performance over time, including:



Time intelligence plays a key role in this dashboard. Various calculations are implemented to track performance over time, including:



Year-over-Year (YOY) comparison

Year-to-Date (YTD) sales and returns tracking





* Dashboard Layout \& Visualizations



The report consists of one main summary page, two detailed analysis pages, and one drillthrough page. Different types of visuals are used to present insights effectively, including cards, KPI indicators, line charts, bar charts, donut charts, and matrix tables. The dashboard also highlights Top N Products and Top N Customers, along with trend analysis and forecasting features to support better business decisions.





* Filtering \& Interactivity



Interactive slicers are provided for filtering data by product, customer segment, region, and date. Users can explore information at different levels using drill-up, drill-down, and drillthrough capabilities. Custom numeric range parameters are also included to allow flexible filtering options.





* Navigation \& User Experience



To improve usability, custom buttons and bookmarks are used for smooth navigation between report pages.





* Mobile Layout



The dashboard is also optimized for mobile devices. Important visuals such as KPI cards and Top N charts are prioritized in the mobile layout to ensure that users can quickly view critical insights on smaller screens.

