#proposition 
1. Si $a$ est un ensemble alors l'ensemble il existe un ensemble dont son seul élément est $a$ et on le note $\{a\}$.
2. Si $a$ et $b$ sont des ensembles alors l'ensemble il existe un ensemble qui admet pour élément seulement  $a$ et $b$ que l'on note $\{a,b\}$.

#Démonstration 

Prouvons (2)
Soient $a,b$ deux ensembles.
D'après l'[[Axiome de la paire]] il existe $c\,'$ un ensemble qui vérifie : $a \in c\,'$ et $b \in c\, '$ 
Ainsi ($x=a \vee x=b$) étant une condition sur x
D'après l'[[Axiome de spécification]] l'ensemble :$$c = \{ x = c\,'\,|\,x= a \vee x= b\}$$existe de plus, $a$ et $b$ sont les seuls élément de $c$ (on prend $x\in c$ ça marche)

Pour montrer (1) il suffit de prendre $a=b$

$CQFD$

---
Remarque :
l'ensemble vide existe donc les ensembles contenant le singleton vide existe etc... On est presque à la définition des entiers naturels !

#Corollaire Si $x_1,\cdots,x_n$ (nombre fini d'élément) sont des ensembles alors l'ensemble $\{x_1,\cdots,x_n\}$ existe

#Démonstration par **induction** 
_initialisation_
si $x_1,x_2$ sont des ensembles alors $\{x_1,x_2\}$ existe
_induction_
$\{x_1,\cdots,x_{n-1}\}$ et $x_n$ sont des ensembles 
alors $\{x_1,\cdots,x_n\}$ est un ens