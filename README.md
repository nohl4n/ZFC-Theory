# Théorie de ZFC — Notes de cours

> Vault [Obsidian](https://obsidian.md/) présentant une introduction formelle à la **théorie des ensembles de Zermelo–Fraenkel avec axiome du choix (ZFC)**. La principale force de ce document est la capacité à visualiser les liens d'implications montrant quels axiomes sont nécessaires à quelle propriété. Ce projet est amené à grandir,  l'objectif final serait de construire tous les objets mathématiques nécessaires jusqu'en L2 voire L3 de mathématiques.

---

## Structure du projet

```
Théorie de ZFC/
├── Logique du 1er Ordre.md          # Prérequis : langage et sémantique
├── Modèle/
│   └── Axiome - Template.md         # Template Obsidian pour les axiomes
└── ZFC/
    ├── Théorie ZFC.md               # Document principal : langage, univers et axiomes
    ├── Axiome ZFC/                  # Les axiomes un par un
    ├── Définition ZFC/              # Définitions construites à partir des axiomes
    ├── Propriété ZFC/               # Propositions et leurs démonstrations
    └── Théorème ZFC/                # Théorèmes majeurs
```

---

## Contenu

### 1. Logique du premier ordre

Introduction au cadre formel nécessaire à la théorie ZFC :
- Alphabet et syntaxe des formules
- Variables libres et variables liées
- Formules atomiques, connecteurs, quantificateurs
- Sémantique : structures et interprétations, satisfaction des formules

### 2. Théorie ZFC

Le document `Théorie ZFC.md` pose les bases :
- Critique du naïf (principes de Cantor, paradoxe de Russell)
- Définition du **langage $\mathcal{L}$** de la théorie des ensembles
- Nature des objets dans l'univers ZFC
- Liste et formulation de tous les **axiomes**

### 3. Axiomes

| Axiome | Énoncé informel |
|---|---|
| **Axiome d'existence** | Il existe au moins un ensemble |
| **Axiome d'extensionnalité** | Deux ensembles sont égaux ssi ils ont les mêmes éléments |
| **Axiome de spécification** | On peut former `{x ∈ A | P(x)}` pour toute condition P |
| **Axiome de la paire** | Pour tous x, y il existe un ensemble contenant x et y |
| **Axiome de la réunion** | Pour tout ensemble A, l'union de ses éléments existe |
| **Axiome de l'ensemble des parties** | Pour tout z, l'ensemble 𝒫(z) existe |
| **Axiome de l'infini** | Il existe un ensemble inductif |

### 4. Définitions

Constructions formelles bâties sur les axiomes :
- **Sous-ensembles** — inclusion et inclusion propre
- **Paires ordonnées** et **n-uplets** — définition via Kuratowski
- **Familles** — ensembles de paires ordonnées indexés
- **Fonctions** — triplets (A, B, F), domaine, codomaine, image, injectivité, surjectivité, bijectivité
- **Transitivité** d'un ensemble
- **Entiers naturels dans ZFC** — ∅ = 0, S0 = 1, S1 = 2, …

### 5. Propriétés démontrées

| Proposition | Description |
|---|---|
| Existence et unicité de ∅ | L'ensemble vide existe et est unique |
| {A, B} existe | Si A et B existent, la paire {A, B} existe (+ corollaire fini) |
| Réunion ∪A | Existence et unicité de la réunion d'une famille |
| Intersection ∩A | Existence et unicité (pour A non vide) |
| Ensemble des parties 𝒫(z) | Existence pour tout z |
| L'ensemble de tous les ensembles n'existe pas | Paradoxe de Russell formalisé |
| Ensemble des fonctions B^A | Existence pour tous ensembles A et B |
| Composition de fonctions | g ∘ f existe et est une fonction |
| Condition à plusieurs variables | {(x,y) ∈ A×B | P(x,y)} existe |

### 6. Théorèmes

| Théorème | Description |
|---|---|
| Théorème fondamental des paires ordonnées | (a,b) = (a',b') ⟺ a=a' ∧ b=b' |
| Théorème du produit cartésien | A×B existe pour tous ensembles A, B |
| Théorème des projections | Toute relation admet une 1ère et 2ème projection |
| Principe de double inclusion | A=B ⟺ A⊆B ∧ B⊆A |
| Principe des ensembles inductifs | Il existe un plus petit ensemble inductif ω |
| ZFC contient Peano | ω vérifie les 5 axiomes de Peano |

---

## Prérequis recommandés

- Logique propositionnelle de base
- Intuition naïve des ensembles (niveau lycée/première année)

---

## Utilisation

Ce vault est conçu pour **Obsidian**. Pour l'ouvrir :

1. Télécharger et installer [Obsidian](https://obsidian.md/)
2. Extraire l'archive `Théorie_de_ZFC.zip`
3. Dans Obsidian : *Ouvrir un coffre* → sélectionner le dossier `Théorie de ZFC`

Les liens `[[...]]` entre notes sont navigables directement dans l'interface Obsidian.

---

## Notations

| Symbole | Signification |
|---|---|
| ∈, ∉ | Appartenance / non-appartenance |
| ⊆, ⊂ | Inclusion large / stricte |
| ∅ | Ensemble vide |
| 𝒫(A) | Ensemble des parties de A |
| ∪A, ∩A | Réunion / intersection d'une famille |
| (a, b) | Paire ordonnée (définition de Kuratowski) |
| A×B | Produit cartésien |
| B^A | Ensemble des fonctions de A vers B |
| ω | Plus petit ensemble inductif (entiers naturels) |
| Sx | Successeur de x : x ∪ {x} |
