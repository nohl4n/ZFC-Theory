# Théorie précédente
## Principe de Cantor

### 1er principe
Deux ensembles sont égaux si et seulement si ils ont les mêmes éléments.

---

### 2eme principe
Etant donné une condition P, il existe un ensemble dont les éléments sont précisément tous les objets qui satisfont cette condition

---

### Paradoxe de Russel

Si on prend $P$ : "$X$ est un ensemble et $X \notin X$" 

alors d'après le [[Théorie ZFC#2eme principe|2eme principe]] l'ensemble : $R = \{X \, | \, P(X)\}$ existe

1. Si $R\in R$, alors $R$ étant un ensemble qui vérifie $P(X)$ $R\notin R$
2. Si $R\notin R$, alors $R$ vérifie $P(X)$ donc $R\in R$

Ainsi $R$ doit vérifier $R \in R \wedge R \notin R$ ce qui est impossible.

# Language ZFC

Le language de la théorie des ensemble, que nous désignerons par le symbole $\mathcal{L}$, est constitué de touts les formules logique qu'on peut écrire en utilisant seulement les symboles suivants qui constitue nôtre alphabet $\mathcal{A}$ :
1. une infinité de variable (lettres qu'on peut aussi indicer) $a,\cdots,z,A,\cdots,Z,a_1,a_2,\cdots, etc$ 
2. Les sept symboles logiques : $\neg,\wedge,\vee,\forall,\exists$
3. les parenthèses : $(,)$
4. Les deux symboles $\in$ et $=$

Il est permis d'élargir le langage $\mathcal{L}\,'$ en ajoutant des nouveaux symbole en utilisant seulement les symbole de $\mathcal{A}$. Ainsi il ne permet pas d'exprimer plus d'idée

exemple:

$\exists y (\cup x \in y)$
$\exists y \exists w \bigl[w \in y \;\land\; w = \cup x \bigr]$
$\exists y \exists w \bigl[w \in y \;\land\; \forall t\, (t \in w \;\Longleftrightarrow\; t \in \cup x )\bigr]$
$\exists y \exists w \Bigl[w \in y \;\land\; \forall t\bigl(t \in w \;\Longleftrightarrow\; \exists x_0\, (t \in x_0 \;\land\; x_0 \in x)\bigr)\Bigr]$

Définition :

1. Une **occurrence** d’une variable $x$ dans une formule $F$ est une **occurrence libre** si elle ne se trouve dans aucune sous-formule de $F$, qui commence par une quantification $∀x$ ou $∃x$. Dans le cas contraire, la variable $x$ est une **variable liée** dans $F$ .
2. Une **variable** est **libre** dans une formule si elle a au moins une occurrence libre dans cette formule.
3. Une **formule close** est une formule sans variable libre

Définition :
1. Si $F$ est une formule de $\mathcal{L}$ dont la seul variable libre est $x$, alors $F$ est une _condition_
2. Si $F\,'$ est une formule de $\mathcal{L}\,'$ qui satisfait :
	1. $F,'$ peut s'exprimer sous la forme d'une formule $F$ de $\mathcal{L}$
	2. la seul variable libre de $F$ est $x$
	alors $F\,'$ est une condition sur $x$

# Univers

Avant de commencer il est important de comprendre ce que contient l'univers:

1. Des objets / ensembles
2. Une Relation "$\in$" entre ces objets
   
il est important de comprendre que "$\in$" est une **brique fondamentale** de la théorie elle lie deux ensembles comme un Relation Binaire d'un language du premier ordre. Elle est a différentier des Relation Binaire définit par la théorie ZFC, qui elle peut se définir par des couple d'ensembles.

Pour Discuter dans cette univers on utilise le Langages du premier ordre :
1. $\wedge , \vee , \neg$ 
2. $\forall , \exists$
3. variables souvent en minuscule
4. objet spécifique en Majuscule
5. parenthèses

## nature des objets

Dans la théorie ZFC tout objets est un ensemble. Pour donner une idée intuitive de ce qu'est un ensemble en mathématiques, disons qu'il s'agit d'une collection d'objets que l'on sait différencier, comme les lettres de l'alphabet, des élèves dans une classe,... Un ensemble peut être défini de deux façons :

- en donnant la liste de ses éléments, que l'on écrit entre accolades (on parle de définition en extension).
- en donnant une propriété caractéristique des éléments qui le compose (on parle de définition en compréhension).

Lorsque les objets ne sont pas clairement distinguables, alors on n'a pas affaire à un ensemble. Ainsi, un sac de pommes de terre n'illustre pas bien la notion d'ensemble. Ceci permet ainsi d'éviter de considérer l'ensemble de tous les ensembles, et donc d'éviter les paradoxes à l'origine d'une crise des mathématiques vers 1900.

## Notion d'existence

le $\exists x (...)$ nous donne le fait "qu'il existe un tel objet qui vérifie une telle propriété"
le $\forall x (...)$ nous donne le fait "tout objet vérifie cette propriété"

## Autres mots du langages

les Autres mots du languages seront définit par une définition sémantique équivalente $:=$ écrit dans le langages décrit au dessus :

exemple : 
1. $A \Rightarrow B :=  \neg A \vee B$
2. $A \Leftrightarrow B:= (A\Leftarrow B) \wedge (A\Rightarrow B)$

Les valeurs logique des propriété $A$ et $B$ sont donnés par les axiomes.
Ils servent a donnés des relations entres les objets.

# Axiomes

## [[Axiome d’extensionnalité]] :$$\forall x \forall y (x=y \Leftrightarrow \forall z (z \in x \Leftrightarrow z \in y))$$
Deux ensemble sont égaux si et seulement si ils ont les mêmes éléments. Cette définition axiomatique dans le langage du premier ordre est équivalent au [[Théorie ZFC#1er principe|1er principe]] de Cantor.

## [[Axiome de spécification]] :$$\forall x (x\in B \Leftrightarrow [x\in A \,\wedge \, P(x)]) $$
Dans ce cas on note : $B = \{x\in A \,|\, P(x)\}$ . Il s'agit d'une version affaiblie du [[Théorie ZFC#2eme principe|2eme principe]] de Cantor. En effet, celui ci énonce que si un ensemble $A$ existe alors $\{x\in A \,|\, P(x)\}$ existe mais n'affirme pas que $\{x \,| \,x\notin x\}$ existe.

Pour être plus clair il faut définir correctement ce que l'on entend par une condition $P(x)$ . On dit que $P(x)$ est une condition sur $x$ si la seul variable libre est $x$ exemple:
1. $x\notin x$
2. $\exists y\exists y(x \in y \wedge y\in z)$
3. $x \in y$ n'est pas une condition sur x car il y a deux variables libres
4. $x \in Y$ est une condition à $Y$ fixé (on peut écrire $\exists Y,x\in Y$)

## [[Axiome d'existence]] :$$\exists x (x=x)$$
Il existe au moins un ensemble

## [[Axiome de la paire]]: $$\forall x \forall y \exists z(x\in z \wedge y\in z)$$ 
Etant donnés des ensembles $x$ et $y$, il existe $z$ tel que $x$ et $y$ sont dans $z$ 

## [[Axiome de la réunion]]$$\forall A \, \exists W \, \forall x \,(\exists a \,(\,a\in A \wedge x \in a) \Rightarrow x \in W)$$
Quel que soit l'ensemble A, il existe au moins un ensemble $W$ qui satisfait : tout élément d'un élément de $A$ est élément de $W$

Par exemple si $A = \{\{a,b\}\{c,d\}\}$ alors il existe un ensemble $W$ tel que $a,b,c,d$ appartiennent a $W$ 

Remarque cela ne signifie pas que les seules élément sont $a,b,c,d$ Mais on peut celui qui ne contient que cela a l'aide de l'[[Axiome de spécification]]

## [[Axiome de l'ensemble des parties]] $$\forall z \,\exists p\,\forall x\,(x\subseteq z \Rightarrow x \in p)$$
Quelque soit l'ensemble $z$, il existe au moins un ensemble p qui se nome l'ensemble des parties

## [[Axiome de l'infini]]$$\exists x (\emptyset \in x \wedge \forall y(y\in x \Rightarrow Sx \in x)$$$$Sx = x\cup\{x\}$$
il existe une ensemble inductif