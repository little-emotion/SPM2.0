# SPM2.0
###QueryTest
When you do a query test, you should let the parameter ‘IS_QUERY_TEST’=  true；
The parameters associated with query test are as follows：
+ QUERY_CHOICE: It decides the type of query statement to be tested.
+ QUERY_SENSOR_NUM: It decides the number of sensor in a query statement.
+ QUERY_AGGREGATE_FUN: It decides the type of aggregate function in a query statement.
+ QUERY_INTERVAL: It decides the time interval between startTime and endTime in a query statement.(ms)
+ QUERY_LOWER_LIMIT: It gives the lower bounds of the sensor values in conditional queries.
Currently, 7 types of queries are supported by setting parameter ‘QUERY_CHOICE’：
	1.precise point query.
	2.fuzzy point query.
	3.query statement with aggregate function. 
	4.range query (limit start stop time)
	5.conditional query (limit start and stop time and the value of each sensor is greater than QUERY_LOWER_LIMIT)
	6.nearest point query
7.query statement with groupBy

When QUERY_SENSOR_NUM = 2，QUERY_AGGREGATE_FUN = max_value, QUERY_INTERVAL = 25000, QUERY_LOWER_LIMIT = 0;
