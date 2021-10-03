JOIN

## JOIN
Combine informations of two tables
if informations exist in both tables


inner join
 `SELECT TrackID, Name, Title FROM Track INNER JOIN Album ON Track.AlbumId = Album.AlbumId LIMIT 3 OFFSET 200 ;`
 
 Return
```
201|Keep It To Myself (Aka Keep It To Yourself)|The Best Of Buddy Guy - The Millenium Collection
202|My Time After Awhile|The Best Of Buddy Guy - The Millenium Collection
203|Too Many Ways (Alternate)|The Best Of Buddy Guy - The Millenium Collection
```

Left Outer JOIN
you have as many rows as you have in the left table

