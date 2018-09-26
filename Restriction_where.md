## Restriction
* WHERE
* Operateur de comparaison

### WHERE
Pour limiter les donnees recuperes a partir d'une condition, on utilise la methode WHERE.

```
SELECT COL_1 FROM TABLE_1
  WHERE COL_1 = VALUE
```

Ici on ne recupere les lignes possedant dans leurs COL_1 la valeur VALUE.

### Operateur de comparaison
Voici la liste des operateurs de comparaison :
* A = B : Si A est egale a B
* A <> B : Si A est different de B
* A > B : Si A est plus grand que B (>= Plus grand ou egal)
* A < B : Si A est plus petit que B (<= Plus petit ou egal)
* A BETWEEN B AND C : Si A est comprit entre B et C
* A LIKE 'string%' : Si A commence par la chaine de caractere 'string' (NOT LIKE pour l'opposer)
* A LIKE '%string' : Si A finit par la chaine de caractere 'string' (NOT LIKE pour l'opposer)
* A LIKE '%string%' : Si A possede la chaine de caractere 'string' (NOT LIKE pour l'opposer)
* A IN (VALUE1, VALUE2, ..., VALUEX) : Si A est comprit dans la liste indiquée
* A IS NULL : Si A est NULL

### Operateur AND, OR et XOR
Les operateurs AND, OR et XOR permettent de creer des combinaisons de conditions a respecter. Le XOR est un OU exclusif, soit l'un soit l'autre, mais pas les 2.

### Operateur NOT
Permet de faire le contraire de la condition mit en place.
