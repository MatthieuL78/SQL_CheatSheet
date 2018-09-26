## Projection

### Basique
La projection utilise le terme SELECT pour selectionner les colonnes que l'on souhaite traiter.

```
SELECT NOM_COL_1, NOM_COL_2 FROM NOM_TABLE
```

On utilise le terme FROM qui indique a partir de quelle table on selectionne les colonnes.
On peut selectionner toutes les colonnes d'une table :

```
SELECT * FROM NOM_TABLE
```

L'option '*' permet de choisir toutes les valeurs de la table.

### Produit cartesien
Le produit cartesien de 2 tables permet d'obtenir toutes les combinaisons possibles de donnees entre les 2 tables.

```
SELECT * FROM NOM_TABLE_1, NOM_TABLE_2
```

Attention les calculs peuvent vite devenir tres lourd.

### Fonction scalaire, application de methode sur les colonnes
On peut ajouter une methode sur la colonne pour traiter les donnees :

```
SELECT (NOM_COL * 3) FROM NOM_TABLE

ou

SELECT SUM(NOM_COL_1) FROM NOM_TABLE
  GROUP BY NOM_COL_2
```
### Renommer une colonne, AS
Le mot cle 'AS' permet de modifier le nom d'une colonne.

```
SELECT NOM_COL AS NEW_NOM_COL FROM NOM_TABLE
```

### Concatenation
On peut concatener des valeurs de differents colonnes dans une seule a l'aide de l'operateur '||' ou de CONCAT (MYSQL).

```
SELECT NOM_COL_1 || '(' || NOM_COL_2 || ')' FROM NOM_TABLE

SELECT CONCAT(NOM_COL_1,'(',NOM_COL_2,')') FROM NOM_TABLE ;
```
