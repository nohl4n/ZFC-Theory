#Définition 
Soit $z$ un ensemble fini alors **si** il existe un ensemble $p$ qui satisfait :$$\forall x (x\in p \Leftrightarrow x \subseteq z)$$ alors $p$ est appelé _l'ensemble des parties de_ $z$  et est noté $\mathcal{P}(z)$ .

Ainsi cette axiome énonce que peut importe l'ensemble $A$ on peut former l'ensemble des parties de $A$ et on le note $\mathcal{P}(z)$.

#proposition 
Quel que soit l'ensemble $z$ , $\mathcal{P}(z)$ existe.

#Démonstration 
Soit $z$ un ensemble
D'après l'[[Axiome de l'ensemble des parties]] il existe un ensemble $p\,'$ qui satisfait : tout [[Sous-Ensembles]] de  est élément de $p\,'$. A présent $p\,'$ étant un ensemble et  $x \subseteq z$ une condition sur $x$ ($z$ étant fixé) d'après l'[[Axiome de spécification]] l'ensemble suivant existe :$$p = \{x \in p\,' \,|\, x\subseteq z\}$$ et pour tout $x$ on a les equivalences :$$x\in p \iff (x\in p\,' \wedge x\subseteq z) \iff x\subseteq z$$donc l'ensemble p satisfait : $\forall x(x\in p \iff x\subseteq z)$
D'où $p=\mathcal{P}(x)$ 

$CQFD$

---
Remarque : 

Cette axiome a besoin de la définition préalable de [[Sous-Ensembles]]

il est possible de ce passé de cette axiome dans le cas des ensembles fini pour cela on a besoin de :
1. corollaire de l'axiome de la réunion si $x_1,\cdots,x_n$ (nombre fini d'élément) sont des ensembles alors l'ensemble contenant uniquement les $x_k$ existe et on le note $\{x_1,\cdots,x_n\}$
2. axiome d'extensivité
3. axiome de spécification

---

#proposition 
Si $z$ est un ensemble fini alors $\mathcal{P}(z)$ existe.

#Démonstration 
Puisque $z$ a un nombre fini d'éléments, il existe un nombre fini d'ensemble $x$ qui satisfont $x\subseteq z$ .
En effet on le démontre par récurrence fini

Pas sur de l'idée encore


on numérote $x_1,\cdots,x_n$ ces ensemble qui vérifie la condition. En vertu du corollaire présenté dans les propriété de l'axiome de  paire et l'axiome de la spécificité et d'extensivité $\{x_1,\cdots,x_n\}$ existe