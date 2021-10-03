WHERE

## WHERE
 examples : 
 
`SELECT TrackId, Name, Composer FROM Track WHERE Composer="Miles Davis";`

ou
`
SELECT TrackId, Name, Composer FROM Track WHERE AlbumId="1";
`

ou
`SELECT TrackId, Name, Composer FROM Track WHERE AlbumId=1 AND Milliseconds >320000 ;`

**USEFULL TRICK**

What if the composer is not spelled correctly ?

`SELECT TrackId, Name, Composer FROM Track WHERE Composer LIKE "%ozart%" ;`

RETURN

```
3412|"Eine Kleine Nachtmusik" Serenade In G, K. 525: I. Allegro|Wolfgang Amadeus Mozart
3413|Concerto for Clarinet in A Major, K. 622: II. Adagio|Wolfgang Amadeus Mozart
3451|Die Zauberflöte, K.620: "Der Hölle Rache Kocht in Meinem Herze"|Wolfgang Amadeus Mozart
3454|Symphony No. 41 in C Major, K. 551, "Jupiter": IV. Molto allegro|Wolfgang Amadeus Mozart
3502|Quintet for Horn, Violin, 2 Violas, and Cello in E Flat Major, K. 407/386c: III. Allegro|Wolfgang Amadeus Mozart
```

We can use list ofcourse
`SELECT TrackId, Name, Composer FROM Track WHERE Composer IN ("Miles Davis", "James Brown") ;`
***