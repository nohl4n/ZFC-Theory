#proposition 
Il n'existe pas d'ensemble $A$ qui satisfait $\forall x (x\in A)$

#Démonstration 
Soit $A$ un ensemble, par **l'absurde**
Supposons qu'il existe $A$ tel que $\forall x(x\in A)$

puisque $A$ est un ensemble et que "$x\notin x$" est une propriété alors d'après l' [[Axiome de spécification]] l'ensemble : $R = \{x \in A\, | \, x \notin x\}$ existe :

1. Si $R\in R$, alors (puisque pour tout $x\in R$, $x\notin x$), $R$ étant un ensemble qui vérifie $P(X)$ donc $R\notin R$
2. Si $R\notin R$, alors $R$ vérifie $P(X)$ donc $R\in R$

Ainsi $R$ doit vérifier $R \in R \wedge R \notin R$ ce qui est impossible. 

**CONTRADICTION**