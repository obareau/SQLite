SQLite


# SQLite MEMO

*BDD de test = chinook.db*


- Avoir une vue générale de la DB

`.tables`

- Avoir une vue d'une table

`.schema foo`

- Selectionne une colone d'une table

`SELECT foo FROM Footable;` 

- Sélectionner plusieurs colone d'une table

`SELECT foo, foo2, foo3 FROM Footable; `

-Sélectionner 10 ligne des 3 colones choisies de la table

`SELECT foo, foo2, foo3 FROM Footable LIMIT 10; `

- Sélectionner N lignes suivantes des colones choisies à partir de N position

`SELECT foo, foo2, foo3 FROM Footable LIMIT 10 OFFSET 20; `
***
- Afficher une selection sans les doublons

`SELECT DISTINCT foo FROM Footable;` 

ou

`SELECT DICTINCT foo, foo2 FROM Footable;` 

Collapse  les valeurs NULLES
.nullvalue NULL
puis
`SELECT DISTINCT foo FROM Footable;`
du coup on n'a plus qu'une seule entrée Null
***









