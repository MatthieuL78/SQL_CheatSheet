## Creer des lignes
Pour ajouter une nouvelle ligne dans une table, il faut utiliser la methode :

```
INSERT INTO NOM_TABLE (NOM_COL_1, NOM_COL_2, ..., NOM_COL_X) VALUES (VALUE_COL_1, VALUE_COL_2, ..., VALUE_COL_X)
```

La premiere partie indique les valeurs que l'on veut remplir dans la table que l'on choisit. On est pas oblige de remplir toutes les colonnes. Les seules valeurs obligatoires sont celles indiquer comme NOT NULL a la creation de la table. La 2nd partie indique les valeurs dans l'ordre pour chaque colonne de la ligne a inserer.
