**Python Project for ETL Process**

This project performs ETL process for operating flight revenue analysis by using Python ETL tool (Pandas) and PostgreSQL. There are six CSV files for monthly available seat-miles (ASM), monthly revenue passenger-miles (RPM), monthly flights, monthly passengers, quarterly net income and quarterly operating revenue for all airports and regions operated by American Ailines. The data used in this project is from Bureau of Transportation Statics website (https://www.transtats.bts.gov/Data_Elements.aspx?Data=2).

Load Factor (LF), also known as passenger load factor (PLF), is an airline industry metric that measures how much of an airline’s passenger carrying capacity is used. PLF is calculated by dividing RPM by ASM. The ratio is usually multiplied by 100 to obtain a percentage value. ASM is the number of seats available for passengers per mile of flight in thousands (000). RPM is the number of revenue passengers flown for each mile in thousands (000).

For ETL process, first extract data from csv files. Second, transfrom extracted data into passenger load factor as mentioned above. In this stage, PLF is calculated for domestic and international respectively. Third, the transformed data and revenue data from extracted data are loaded into PostgreSQL database. Regarding database testing, some rows from the resptive tables are retrived to make sure that the loaded data is correct. The Operating Flight Revenue(OFR) data model (ER diagram) could be seen under the data modeling folder.