#Théoreme 
Etant donnés des ensembles $A$ et $B$, il existe un ensemble $P$ dont les éléments sont toutes les paires $(a,b)$ telles que $a\in A$ et $b\in B$

On appelle P le _produit cartésien de A et B_ et on note $P=A\times B$

#Démonstration 
Si au moins un des deux est vides : alors il n'existe aucune paire Donc $P = \emptyset$

Supposons à présent $A$ et $B$ non vide

1. Montrons dans un premier temps qu'il existe $E$ tel que : $\forall a \forall b (a \in A \wedge b\in B \Rightarrow (a,b)\in E)$

Puisque A et B sont des ensembles, les ensembles $A\cup B$ existe ( [[Si A et B existe le l'ensemble {A,B} existe]] puis on fait la [[Réunion]] de cette ensemble ) ensuite d'après la propriété sur les [[Parties]] $\mathcal{P} (A\cup B)$ existe, et de même $\mathcal{P}(\mathcal{P} (A\cup B))$ existe.

Soient $a\in A$ , $b\in B$
alors $\{a\}$ et $\{a,b\}$ existe et son par définition des [[Sous-Ensembles]] de $A \cup B$. Ainsi  par définition des [[Parties]] de $A\cup B$ , $\mathcal{P} (A\cup B)$ contient tout les _sous ensembles_ de $A\cup B$ en particulier $\{a\}$ et $\{a,b\}$. De même on obtient $\{\{a\} ,\{a,b\}\} \in \mathcal{P}(\mathcal{P} (A\cup B))$ 

Ainsi $E=\mathcal{P}(\mathcal{P} (A\cup B))$ existe et vérifie bien : $$\forall a \forall b (a \in A \wedge b\in B \Rightarrow (a,b)\in \mathcal{P}(\mathcal{P} (A\cup B)))$$ 
2. $\exists a \exists b [a\in A \wedge b\in B \wedge x = (a,b)]$ est un condition sur $x$

d'après l'[[Axiome de spécification]] l'ensemble $$P = \{x\in E\,| \, \exists a \exists b [a\in A \wedge b\in B \wedge x = (a,b)]\}$$existe et on a les équivalences :$$\begin{align}
x\in P &\iff  x\in E\,et\, \exists (a\in A) \exists (b\in B)  ,x = (a,b)\} \\
  &\iff \exists (a\in A) \exists (b\in B)  ,x = (a,b)\}\\
  &\iff x \,\, est \,\, une \,\, paire \,(a,b)\, telle\,\,que\,\,(a\in A)\,\, et\,\,(b\in B)\\
\end{align}$$
Ainsi on a construit un ensemble $P$ qui satisfait la condition demandée.