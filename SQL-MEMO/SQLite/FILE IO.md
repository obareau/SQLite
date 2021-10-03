FILE IO

## FILE IO

we can save our queries in a .sql file
and write the outpout in a .csv file

Examples :
`.read tracks-and-albums.sql`

**write process :** 

```
.headers on
.mode csv
.output foo.csv
```

now every single queries i will pass to the database will not be written **ON SCREEN** but on the file
