# Langage du 1er Ordre

L’alphabet d’un langage du premier ordre comporte d’abord les symboles suivants, qui sont communs à tous les langages :
1. les connecteurs $¬, ∧, ∨, →, ↔,$
2. les parenthèses (, ),
3. les quantificateurs universels $∀$ et existentiels $∃$,
4. un ensemble infini $V$ de symboles de variables , choisis habituellement parmi les lettres $x, y, z, u, v$ éventuellement indicées.

**Définition** 1 : Un langage $\mathcal{M}$ de la logique du premier ordre est caractérisé par l’ensemble de symboles suivants :
1. les symboles de **relations** (ou **prédicats**) ; à chaque symbole est associé un entier strictement positif, appelé l’**arité**,
2. les symboles de **constantes**.

En général, les langages du premier ordre peuvent comporter également des symboles permettant de représenter des fonctions. Tous ces symboles sont destinés à être interprétés par la suite dans des
structures. Pour le moment, la construction de l’ensemble des formules d’un langage est définie de manière purement syntaxique.

## L'ensemble des formules

Le langage $\mathcal{L}$ est supposé égalitaire (contient le symbole de relation $=$)

**Définition** 2 L’ensemble des **formules atomiques** est l’ensemble des formules de la forme :
• $t1 = t2$ où $t1$, $t2$ sont des termes,
• $Rt_1t_2...t_n$ où R est un symbole de relation d’arité $n$ et $t_1, t_2, \cdots, t_n$ sont des termes ; cette formule peut aussi être notée $R(t_1, t_2, ..., t_n)$.

L’ensemble des formules est le plus petit ensemble qui contient les formules atomiques et qui est clos par application des connecteurs et des quantificateurs.

**Définition** 3 L’ensemble des formules, que l’on désigne par $\mathcal{F}$, est le plus petit ensemble satisfaisant :
1. toute formule atomique est une formule,
2. si F est une formule, alors ¬F est une formule,
3. si F, G sont des formules, alors $(F ∧ G)$,$(F ∨ G)$,$(F → G)$ et $(F ↔ G)$ sont des formules,
4. si F est une formule et v une variable, alors $∀v F$ et $∃v F$ sont des formules

**Proposition** 1 Toute formule d’un langage du premier ordre se décompose de manière unique sous l’une, et une seule, des formes suivantes :
1. une formule atomique,
2. $¬F$ où $F$ est une formule,
3. $(F ∧ G)$, $(F ∨ G)$,$(F → G)$ ou $(F ↔ G)$, où $F$, $G$ sont des formules,
4. $∀v F$ ou $∃v F$ , où $F$ est une formule et $v$ une variable.

**Démo par récursion**

**Définition** 4 Une formule $G$ est une **sous-formule** de la formule $F$ si elle apparaît dans la décomposition de $F$ .

## Variables libre, variables liées


# Sémantique

La sémantique de la logique du premier ordre est définie en interprétant les formules d'un langage donné dans les structures correspondantes. Ces structures peuvent être d'ordre mathématique ou représenter des types de données en informatique, les domaines des relation dans une base de donnés relationnelle, ou encore l'univers du discours en linguistique

## Structures et langages

En logique du premier ordre, **une structure** (ou _interprétation_) est l’objet mathématique qui **donne un sens** aux symboles d’un langage formel.  C’est l’outil central de la **sémantique** : il permet de dire si une formule est vraie ou fausse.

Soit un langage ( $\mathcal{L}$ ).  
Une **structure** ( $\mathcal{M}$ ) pour ce langage est un objet composé de 

1. **Un domaine**
    - Noté ( $M$ )
    - C’est un ensemble non vide d’objets.
2. **Une interprétation** des symboles du langage :
    - Chaque **symbole de constante** ( $c$ ) est interprété par un élément ( $c^{\mathcal{M}} \in M$ ).
    - Chaque **symbole de fonction** ( $f$ ) de rang ( $n$ ) est interprété par une fonction  
        $f^{\mathcal{M}} : M^n \rightarrow M$.  
    - Chaque **symbole de relation** ( $R$ ) de rang ( $n$ ) est interprété par une relation  
        $R^{\mathcal{M}} \subseteq M^n$.  

En résumé :  
$\mathcal{M} = (M,; (c^{\mathcal{M}})_{c \in \text{Const}},; (f^{\mathcal{M}})_{f \in \text{Fonctions}},; (R^{\mathcal{M}})_{R \in \text{Relations}})$  

Langage :    
$\mathcal{L} = {0, S, +, \times}$

Structure :  

$\mathbb{N} = (\mathbb{N}, 0^{\mathbb{N}}, S^{\mathbb{N}}, +^{\mathbb{N}}, \times^{\mathbb{N}})$ 
avec :
- domaine : ( $\mathbb{N}$ )
- ( $0^\mathbb{N} = 0$ )
- ( $S^\mathbb{N}$ ) est l’application ( $n \mapsto n+1$ )
- ( $+^\mathbb{N}$) est l’addition
- ( $\times^\mathbb{N}$ ) est la multiplication

## Structure et satisfaction des formules

