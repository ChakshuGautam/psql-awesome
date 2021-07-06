### Common Tasks

 - [Disk Usage Checks](https://wiki.postgresql.org/wiki/Disk_Usage)
 - Set working memory for a session ```SET work_mem = '256MB';```
 
 
### pg-stat-statements

### Common Error - fixes

### Docker setups

### Sharing localhost with someone
```zsh
ngrok tcp 5432
```
If things went correctly it should show something like this -> `tcp://0.tcp.ngrok.io:12646 -> localhost:15432`
For the connection url it should be something like this -> `postgres://username:password@0.tcp.ngrok.io:12646/dbName`

