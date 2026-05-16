#Définition 1
Une _fonction_ est un triplet ordonné $(A,B,F)$ satisfaisant :$$F\subseteq A\times B \, \wedge \, \forall (x\in A) \exists ! (y\in B),[(x,y)\in F \,] $$
#Définition 2
Une _fonction_ est un triplet ordonné $(A,B,F)$ satisfaisant : $F$ est une [[Familles]], $F_1=A$ et $F_2 \subseteq B$ où $F_i$ qui sont respectivement la première et deuxième [[Théorème des projections|projections]] de $F$

#Définition on note $f= (A,B,F)$
1. $A$ est appelé le _domaine_ de $f$ ( $dom(f)=A$ )
2. $B$ est appelé le _codomaine_ de $f$ ( $codom(f)=B$ )
3. On dit que $f$ est une fonction de $A$ vers $B$ : on écrit $f:A \to B$
4. Si $(a,b)\in F$ on écrit $f(a)=b$. autrement dit si $a\in A$ alors $f(a)$ existe et est l'unique élément de B qui vérifie $(a,b)\in F$
5. Puisque $F$ est l'ensemble de paire ordonnées, on peut considérer les [[Théorème des projections|projection]] $F_1$ et $F_2$ de $F$. $F_2$ et dit l'_image_ de $f$ et est noté $f(A)$: autrement dit,$$im(f)= F_2 = \{ y\in B\,|\, \exists (a\in A), (x,y)\in F \} = \{ y\in B\,|\, \exists (a\in A), f(x) = y \} $$
---
Remarque :
d'après la généralisation des [[Condition avec plusieurs variable]] $$D = \{(x,y)\in E\times E\,|\, x=y\}$$existe et $(E,E,D)$ vérifie la définition d'une _fonction_ on la note $i_E$ et vérifie pour tout $x\in E$, $i_E(x)=x$

#Définition $f:A \to B$
1. $f$ est dit **surjective** si $im(f) = B$
2. $f$ est dite **injective** si $\forall x_1 x_2 \in A(f(x_1) = f(x_2) \Rightarrow x_1 = x_2$
3. $f$ est dite **bijective** si elle est injective et surjective

#definition 
Une fonction est  **inversible** s'il existe exactement une fonction $g:B \to A$ tel que $$g\circ f = i_A \wedge f\circ g = i_B$$
#Théoreme 
Une fonction est inversible alors $ssi$ elle est bijective

#admis
