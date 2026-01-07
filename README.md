# Automotive-Aftersales-Performance-Dashboard
The Aftersales Performance Dashboard was developed to provide a focused evaluation of General Repair (GR) workshop performance across the year. Below are the end-to-end project technical details:

1. Unit entry data from each branch workshop is downloaded from the Dealer Management System. The data is then cleaned using Power Query in Microsoft Excel, including date standardization, removal of unnecessary rows and columns, and merging all files into a single dataset called revenue_gr.

2. The revenue_gr dataset is further processed using Python. In this step, unit entries categorized as SBE (periodical service) are separated, service kilometers are standardized to determine the service level, and a new dataset called sbe_df is generated.
   ![Alt text atau deskripsi gambar](https://github.com/budds98/Automotive-Aftersales-Performance-Dashboard/blob/main/python-01.jpg)
 
4. Since the dataset is large, all cleaned data is loaded into a PostgreSQL database using Python for efficient storage and data management.

5. For data visualization and analysis, PostgreSQL is connected to Power BI to build dashboards that analyze key workshop business metrics.



