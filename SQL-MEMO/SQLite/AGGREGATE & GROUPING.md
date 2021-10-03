AGGREGATE & GROUPING

## AGGREGATE & GROUPING
Examples : 
How many tracks by album ?
`SELECT AlbumID, COUNT(TrackId) FROM Track GROUP BY AlbumID;`
or

Nombre total d'éléments dans une table
`SELECT COUNT(trackId) FROM Track ;`

Classer par la longueur totale des morceaux par albums

`SELECT AlbumId, SUM(Milliseconds) FROM Track GROUP BY AlbumId ORDER BY SUM(Milliseconds);`

Trouver le morceau le plus long de l'album

 `SELECT AlbumId, MAX(Milliseconds), Name FROM Track GROUP BY AlbumId ORDER BY SUM(Milliseconds);`
 
 bien sûr y'a aussi MIN, et AVERAGE
 
 sort seulement albumm ayant plus de 10 chansons

  `SELECT AlbumId, COUNT(TrackId), Name FROM Track GROUP BY AlbumId HAVING COUNT(TrackId) > 10;`
 
 