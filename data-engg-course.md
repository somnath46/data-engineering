# 22-02-2026
## databrics components
- Storage
	- catalog: For structured data
	- volume: Both Structured and unstructured data
- Upload data using DataIngesition loke csv and it will relect in the Catalog section
- managed and external data
	- manage is data directly ingested to databrics
	- external is when data is stored in other service like in any database and databrics uses this data
- lazy evaluation in spark
- data action in spark: If any action is not called -  the work will not done, like data reading, transformation etc.

# 28-02-2026
## databrics
- Under Jobs and pipeline menu we can set triggers - means when a Job will run
	- it can be time based
	- it can be event trigger based
- temp table
- rename column
	- df.withColumnRemane("from_col", "to_col")
	- df.select(col("from_col").alias("to_col"))
- filter
	- df.filter(df.country == "India")
	- df.filter(col("country")) == "India") // faster
	
# 01-03-2026
## databrics
- duplicate removal
- agg funtions like group by
- overrite and append mode - overrite mode is used most of the cases
- table join - union
	- dominant col name like df1.union(df2) then df1 col will be dominant
- whwn and otherwise operator - like if or case statement

# 07-03-2026
## databrics
- join - same like sql
- broadcast join
- window function

# 08-03-2026
## Azure data Factory - 1
- linked services
	- can connect to differnet datasources
	- create storage account 
	- zone - in where it's going to store, can relicate the data into differemt region
	- zone is same like availability zone in aws
	- creating blob storage - one is from and other is to
- copy data
- combination of multiple activity is call ed as a pipeline
- pulish all measns saving data like ctrl+s
- add trigger to trigger the job 

# 14-03-2026
## Azure data Factory - 2
- ADLS

# 21-03-2026
## Data  Modeling
- Data lake
	-store structured  or semi structured data (csv, xml, json etc)
- data warehouse
	- store structured data (Use postgres mostly)
	- snowflake, redshift, teradata
- data mart
	- subset of data warehouse
- data warehos vs database
- olap and oltp
- homework
Use case:
Vishal Mega Mart: 1000 stores across India, 5 regions, 20 states
1000 products in one store
Vishal -> Owner (Maximise the profit, reduce operational cost)
Make it azure compatible

# 22-03-2026
## Data  Modeling
 - use case
 - fact and dimension table in data warehouse
 -star schema vs snowflake schema