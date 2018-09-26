## Creer une nouvelle table
Suivre la methode suivante pour creer une nouvelle table :

``
CREATE TABLE NOM_DE_LA_TABLE (
  NOM_COL_1 TYPE_COL_1,
  NOM_COL_2 TYPE_COL_2,
  ...
  NOM_COL_X TYPE_COL_X
)
``

## Conditions
On peut ajouter des conditions de creation de ligne avec : 

``
NOT NULL
``

A ajouter apres la creation de colonne :

``
CREATE TABLE NOM_DE_LA_TABLE (
  NOM_COL_1 TYPE_COL_1 NOT NULL
)
``

## Cles
On peut ajouter des colonnes en indiquant que se sont les cles de la table :

``
PRIMARY KEY(NOM_COL)
FOREIGN KEY(NOM_COL)
``

A ajouter a la fin de la creation de table :

``

CREATE TABLE NOM_DE_LA_TABLE_1 (
  NOM_COL_1 TYPE_COL_1, 
  NOM_COL_2 TYPE_COL_2,
  ... ,
  NOM_COL_X TYPE_COL_X,
  PRIMARY_KEY(NOM_COL_1),
  FOREIGN KEY(NOM_COL_2) REFERENCE NOM_DE_LA_TABLE_2(NOM_COL_1)
)

CREATE TABLE NOM_DE_LA_TABLE_2 (
  NOM_COL_1 TYPE_COL_1
)

``

## Domaine
Il existe different domaine pour les colonnes (int, char, ...). Suivre ce lien pour plus d'information : [ICI] (https://www.w3schools.com/sql/sql_datatypes.asp) - Domaine possible SQL

### Attention
* Ne pas mettre de ',' a la derniere colonne creer.
