#Théoreme 
Quels que soient les ensembles $a$, $b$, $a\,'$, $b\,'$ on a :$$(a,b) = (a\,',b\,') \iff (a=a\,' \wedge b=b\,')$$

---

Prérequis :
1. [[Intersection]]
2. [[Réunion]]
3. [[n-uplet ordonné Ordonnées]]

#Démonstration 
1. $\Leftarrow$
	   Supposons $a=a\,'$ et $b=b$ alors d'après l'[[Axiome d’extensionnalité]] $\{a\} = \{a'\}$ et  $\{a,b\} = \{a\,',b'\}$
	   d'où $\{\{a\},\{a,b\}\} = \{\{a\,'\},\{a\,',b\,'\}\}$
	   _ccl_ : $(a,b) = (a\,',b\,')$
2. $\Rightarrow$
	   Supposons que $E = (a,b) = (a\,',b\,')$
	1. montrons que $a =a\,'$$$\cap E = \cap (a,b) = \cap  \{\{a\},\{a,b\}\} =  \{a\}\cap\{a,b\}= \{a\}$$et$$\cap E = \cap (a\,',b\,') = \cap  \{\{a\,'\},\{a\,',b\,'\}\} =  \{a\,'\}\cap\{a\,',b\,'\}= \{a\,'\}$$on a ainsi $\{a\} = \{a\,'\}$ à présent on à $a\in \{a\}$ donc $a\in \{a\,'\}$, donc $a=a\,'$ 
	2. Similairement $$\cup E = \cup (a,b) = \cup  \{\{a\},\{a,b\}\} =  \{a\}\cup\{a,b\}= \{a,b\}$$et$$\cup E = \cup (a\,',b\,') = \cup  \{\{a\,\},\{a\,',b\,'\}\} =  \{a\,'\}\cup\{a\,',b\,'\}= \{a\,',b\,'\}$$ donc $\{a,b\}= \{a\,',b\,'\}$ à présent $b\in \{a,b\}$ donc $b \in \{a\,',b\,'\}$
		1.  Si $a=b$, $\{a,b\} = \{b\}$ donc $b\,' \in \{a\,',b\,'\} = \{b\}$ donc $b=b\,'$
		2. Sinon, avec $b\in \{a,b\}$,  $b \in \{a\,',b\,'\}$ or $b \neq a\,'$ car $a=a\,'$ donc $b=b'$dans les 2 cas on a $b=b\,'$
	ainsi on à $a=a\,'$ et $b=b$ 


$CQFD$

---
#Théoreme 
Généraliser au n-uplet par recurrence