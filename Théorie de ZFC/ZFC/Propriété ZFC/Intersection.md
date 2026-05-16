#proposition 
Si $A$ est un ensemble non vide, alors il existe un _unique_ ensemble $V$ dont les éléments sont précisément tous les ensembles de $x$ qui satisfont :  $x$ est un élément de chaque élément de $A$. Ou encore $x$ est contenu dans chaque élément de $A$.

Autrement dit si $A$ est l'ensemble dont les éléments sont les ensembles $A_1,\cdots,A_n$ que l'on souhaite intersecté alors l'ensemble$A_1\cap \cdots \cap A_n := \cap \{A_1,\cdots,A_n\}$ existe et est unique

---


#Démonstration 
Soit $A$ un ensemble non vide
Puisque $A \neq \emptyset$, on peut choisir $E$ tel que $E \in A$.
Puisque $E$ est un ensemble et que  $\forall a\, (\,a\in A \Rightarrow x\in a\,)$ est une condition sur $x$
D'après l'[[Axiome de spécification]] : $$V = \{ \, x \in E \,| \,\forall a\, (\,a\in A \Rightarrow x\in a\,)\} $$ est un ensemble

Ainsi soit $x$ un ensemble, on a les équivalences :$$\begin{align}
x\in V &\iff x\in E \ et \, \forall a(a\in A \Rightarrow x \in a) \\
  &\iff x \in E \, et\,pour \,\, tout \,\, élément \,\, de \,\, a \,\, x \,\,est\,\, dans\,\,a\\
  &\iff x \,\, est \,\, dans \,\, tout \,\, les\,\,éléments\,\, de\,\,A\\
\end{align}$$
Pour passer de la 3eme à la 2eme equivalences il s'agit juste de remarquer que $x \in E$ signifie que $x$ est dans un élément particulier de $A$ et que l'assertion de droite nous l'assure déjà pour tout élément de $A$ y compris $E$.

Ainsi l'ensemble $V$ à la propriété voulue
Enfin d'après l'[[Axiome d’extensionnalité]] avec un résonnement d'unicité on trouve que $V$ est unique 

On note $\cap A := V$ 
ou encore $\cap_{X \in A} X := V$

$CQFD$

---

Remarque ceci généralise directement l'intersection Pour n'importe qu'elle type d'intersection:

On note généralement :
$A_1\cap \cdots \cap A_n := \cap \{A_1,\cdots,A_n\}$

