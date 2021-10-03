SORTING

## SORTING
**sorting ascending :** 
Warning the sorting criteria must be in the query
so
`SELECT foo, foo2 FROM Footable ORDER BY foo2;` 
is valid
and
`SELECT foo, foo2, FROM Footable ORDER BY foo3;`
will not work

**sorting descending :**
 
`SELECT foo, foo2 FROM Footable ORDER BY foo2 DESC;`

Examples : 

`
SELECT Name, Milliseconds, AlbumId FROM Track ORDER BY AlbumId ASC, Milliseconds DESC LIMIT 5;`
***