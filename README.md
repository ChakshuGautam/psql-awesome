### Common Tasks

 - [Disk Usage Checks](https://wiki.postgresql.org/wiki/Disk_Usage)
 - Set working memory for a session ```SET work_mem = '256MB';```
 
 
### pg-stat-statements

### Common Error - fixes

### Docker setups

### Sharing localhost with someone
`ngrok tcp 5432`

If things went correctly it should show something like this -> `tcp://0.tcp.ngrok.io:12646 -> localhost:15432`
For the connection url it should be something like this -> `postgres://username:password@0.tcp.ngrok.io:12646/dbName`


### Generated Columns
- AGE => https://fluca1978.github.io/2019/11/04/PostgreSQL12GeneratedColumns.html

### size of tables
```psql
SELECT
   relname as "Table",
   pg_size_pretty(pg_total_relation_size(relid)) As "Size",
   pg_size_pretty(pg_total_relation_size(relid) - pg_relation_size(relid)) as "External Size"
   FROM pg_catalog.pg_statio_user_tables ORDER BY pg_total_relation_size(relid) DESC;
```

