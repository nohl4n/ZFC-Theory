#proposition 
Si $A$ est un ensemble alors il existe un et un seul ensemble $W$ dont les éléments sont précisément tous les ensembles $x$ qui satisfont :

$x$ est un élément d'au moins un élément de $A$

---

#Démonstration 
Soit $A$ un ensemble
D'après l'[[Axiome de la réunion]] il existe un ensemble $W\, '$ qui satisfait :
Tout élément _d'un élément_ de $A$ est élément de $W\,'$ 
Puisque $W\,'$ est un ensemble et que $\exists a \,(\,a\in A \wedge x\in a \,)$ est une condition sur $x$, d'après l'[[Axiome de spécification]] l'ensemble :$$W=\{ x\in W\,'\,|\, \exists a \,(\,a\in A \wedge x\in a \,)\}$$ existe et on a les equivalences :$$\begin{align}
x\in W &\iff x\in W\,' \ et \, \exists a(a\in A \wedge x \in a) \\
  &\iff \exists a(a\in A \wedge x \in a)\\
  &\iff x \,\, est \,\, un \,\, élément \,\, d'au\,\,moins\,\,un\,\, élément\,\,A\\
\end{align}$$

Remarque on passe de la 1er a la 2eme equivalences car pour tout $x$ l'implication suivante est vraie :$$\exists a \,(\,a\in A \wedge x\in a \,) \Rightarrow x\in W\,'$$ 
En vertu de l'[[Axiome d’extensionnalité]] il ne peut y avoir qu'un seul $W$ ayant cette propriété.

$CQFD$

---
Notation Dans ce cas on note $W := \cup A$


#Définition 
On note $A_1\cup \cdots \cup A_n := \cup \{A_1,\cdots,A_n\}$
