# The purpose of this code is to run the VACUUM REINDEX ANALYZE task on all tables in all databases that have dead tuples.
<h2>This code was created for Linux environment.</h2>
<h3>You can download the vacuum.sh file and adjust it as needed.</h3>

<p>https://github.com/ramos-r29/PostgreSQL_VACUUM/blob/main/vacuum.sh</p>

<p>The database connection must be configured in the vacuum.sh file using the "pg_conn" variable.</p>

<p>The "db_list" variable will list all databases found using the "pg_conn" variable.</p>

<p>The variable "pg_query_tp" sets up a query that checks which tables have dead tuples with length greater than 0.
It can be adjusted as needed, changing the size in the "WHERE" field and defining it in bytes.</p>

<p>The variable "pg_tables_list" creates the list of tables with the dead tuples and then a repetition structure executes VACUUM, REINDEX and ANALYZE for each table in this list. </p>

