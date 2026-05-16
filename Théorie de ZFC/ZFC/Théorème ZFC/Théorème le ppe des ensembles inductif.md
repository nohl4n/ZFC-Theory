#Théoreme Il existe exactement un ensemble $\omega$ qui satisfait les deux conditions suivantes :
1. $\omega$ est un [[Axiome de l'infini|ensemble inductif]]
2. $\omega$ est [[Sous-Ensembles|inclus]] $\subseteq$ dans tout ensemble inductif

#lemme #admis 
supposons que E est un ensemble non vide doint chaque élément est un ensemble inductif alors $\cap E$ est un ensembles inductif.


#Démonstration  
En vertu de l'[[Axiome de l'infini]], il existe un ensemble inductif $A$. ainsi l'ensembles des [[Parties]] de $A$ existe et "x est un ensemble inductif" est une condition sur x
d'après l'[[Axiome de spécification]] : $$E = \{x \in \mathcal{P}(A),\emptyset \in x \wedge \forall y (y\in x \Rightarrow y\cup\{y\} \in x \}$$Notons que $E$ est non vide ($A\in E$), d'après le lemme précédent $\cap E$ est un ensemble inductif et on note $$\omega = \cap E$$
Montrons a présent que omega est inclus dans tout ensemble inductif. Soit $B$ un ensemble inductif quelconque.
Alors $A\cap B$ est un ensemble inductif #admis et $A\cap B\in \mathcal{P}(A)$, donc $A\cap B\in E$, Or par définition de [[Intersection]] pour tout $C\in E$,  $\cap E \subseteq C$ . Ainsi $$\omega \subseteq A\cap B \subseteq B$$
On a montré l'existence d'au moins un ensembles inductif $\omega$ qui est inclus dans tout les autres

Unicité 
Soit $\omega '$ ensembles inductif inclus dans tout les autres. On a $\omega \subseteq \omega '$