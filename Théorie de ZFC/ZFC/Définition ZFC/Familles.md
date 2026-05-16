#Définition 
Une _famille_ est un ensemble $F$ qui satisfait les conditions suivantes:
1. Chaque élément de $F$ est une [[n-uplet ordonné Ordonnées|paire ordonnée]]
2. $\forall xy_1y_2([(x,y_1)\in F \wedge (x,y_2)\in F] \Rightarrow y_1 = y_2)$

en gros chaque élément de cette ensemble est un couple dont la [[Théorème des projections|première projection]] est noté $I$ et représente l'ensemble des _indices_ et que $F$ est une **famille indicée** par $I$. La définition de famille implique que pour chaque $i\in I$ il existe un seul et unique y tel que que $(i,y)\in F$: si cette ensemble est noté $A_i$ on écrit alors $F=(A_i)_{i\in I}$

#Notation 
Si $F=(A_i)_{i\in I}$ est une famille quelconque alors F est un ensemble de paire ordonnées, donc la seconde projection de $F$ existe. on le note $$\{A_i\,|\,i \in I\}$$

On définit les ensembles (attention il faut non vide pour [[Intersection]]) $$\bigcap_{i\in I} A_i = \cap\{A_i\,|\, i\in I\}$$et$$\bigcup_{i\in I} A_i = \cup\{A_i\,|\, i\in I\}$$