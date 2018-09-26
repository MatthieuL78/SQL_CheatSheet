## Join

* Jointure
* Jointure externe (A faire)
* Jointure naturelle (A faire)

### Jointure
La methode JOIN permet de lier 2 tables a l'aide de cles.

```
SELECT COL_1 FROM TABLE_1 JOIN TABLE_2 ON CLE_TABLE_1 = CLE_TABLE_2
```

On joint les 2 tables en precisant les valeurs communes CLE_TABLE_1 et CLE_TABLE_2. Les lignes de la TABLE_1 comprenant une CLE_TABLE_1 egale a CLE_TABLE_2 de la TABLE_2 ne formeront qu'une seule ligne dans la nouvelle table qui joindra les tables TABLE_1 et TABLE_2.
On peut egalement ecrire de la facon suivante :

```
SELECT COL_1 FROM TABLE_1, TABLE_2 WHERE (CLE_TABLE_1 = CLE_TABLE_2)
```

Attention, il est possible que les noms des colonnes soient les memes pour differentes tables. C'est pourquoi on peut preciser de la maniere suivante :

```
SELECT COL_1 FROM TABLE_1 JOIN TABLE_2 ON TABLE_1.CLE_TABLE_1 = TABLE_2.CLE_TABLE_2

ou

SELECT COL_1 FROM TABLE_1, TABLE_2 WHERE (TABLE_1.CLE_TABLE_1 = TABLE_2.CLE_TABLE_2)
```

Nous pouvons egalement creer des combinaisons de plusieurs tables comme suit :

```
SELECT A.COL_1, B.COL_1, C.COL_1 FROM TABLE_1 A, TABLE_2 B, TABLE_3 C WHERE A.COL_1 = B.COL_1 AND B.COL_2 = C.COL_1
```

### Jointure externe

### Jointure naturelle
