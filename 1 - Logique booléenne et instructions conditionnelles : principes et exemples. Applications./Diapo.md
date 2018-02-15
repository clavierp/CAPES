Logique booléenne et instructions conditionnelles : principes et exemples. Applications.
===
## Paul Clavier
Jeudi 18 Janvier

---

# Logique booléenne
Algèbre de Boole: Soit $B$ l'ensemble constitué de de deux __valeurs de vérité__ Vrai et Faux. 
Pour la suite, on notera Vrai par $1$ et Faux par $0$, $B := \{1,0\}$
On munit cet ensemble de deux lois (ET et OU) et d'une transformation (NON)

---

# ET
A et B est vrai si et seulement si A est vrai _et_ B est vrai.
On la note $\wedge$, $&$ ou  $AND$. Pour la suite, on la notera $\cdot$
$0$ est l'élément absorbant et $1$ l'élément neutre.
Sa table de vérité est:
A | B | A$\cdot$B
:---:|:---:|:---:
0 | 0 | 0
0 | 1 | 0
1 | 0 | 0
1 | 1 | 1

---
# OU
A ou B est vrai si et seulement si A est vrai _ou_ B est vrai.
On la note $\vee$, $|$ ou  $OR$. Pour la suite, on la notera $+$
$1$ est l'élément absorbant et $0$ l'élément neutre
Sa table de vérité est:
A | B | A$+$B
:---:|:---:|:---:
0 | 0 | 0
0 | 1 | 1
1 | 0 | 1
1 | 1 | 1

---
# NON
non A est vrai si et seulement si A est faux.
On la note $\neg A$, $/A$, $!A$, $not$ $A$. Pour la suite, on la notera $\bar A$
On a $\overline{(\bar A)} = A$
Sa table de vérité est:
$A$ | $\bar A$
:-: | :-:
0 | 1
1 | 0

---
# Propriétés
1. $+$ et $\cdot$ sont associatives, commutatives et distributives
2. Idempotence $A+A=A$ et $A\cdot A= A$
3. Tiers exclus: $A + \bar A = 1$
4. Non contradiction: $A\cdot \bar A= 0$

---
# Théorème de De Morgan
1. $\overline{A+B} = \bar A \cdot \bar B$
2. $\overline{A\cdot B} = \bar A + \bar B$

---
# Fonctions logiques
Application de $B^n$ dans $B$
Toute fonction logique est une composition de $(+,\cdot,\bar.)$
Il y a exactement $2^n$ fonctions logiques de $B^n$ dans $B$

---
# Fonctions logiques composées
Fonctions logiques à 2 variables (de $B^2$ dans $B$)
Fonctions logiques notables:
1. XOR: $A\oplus B = A\cdot\bar B + \bar A\cdot B$
2. Equivalence: $A\Leftrightarrow B = A\cdot B + \bar A\cdot\bar B$
3. Implication: $A\Rightarrow B = \bar A + B$

---

# Exercice
Développer les propositions suivantes
1. $(A \cdot B) + (\bar A \cdot B)$
0. $\overline{(A\cdot\bar B)} + B$
0. $\overline{(A \ \Rightarrow B)} \Rightarrow (B + \bar C)$

Montrer l'équivalence entre:
1. $(A\Rightarrow B)\cdot(B\Rightarrow A)$
2. $A \Leftrightarrow B$

---

# Forme clausale
Toute proposition peut être mise sous forme clausale, c'est à dire une disjonction de .
Cette forme clausale peut être trouvée en utilisant la table de vérité de la proposition.

---

# Exercice 

Donner la forme clausale des propsitions suivantes:
1. $(\bar A + B)\cdot \bar C$
2. $\overline{(A + \bar B \cdot C)} + D$
3. $(A \Rightarrow B) \Rightarrow C$

---
# Instruction Conditionelle
Instruction qui modifie le flot d'éxécution en fonction d'une condition booléenne.
En algorithimque, elle suit une structure *Si Alors Sinon Finsi.*
```
abs(n) := Si n < 0 Alors -n Sinon n Finsi
```
En python, on utilise les mots clés *if then else*
```Python3
def abs(n):
    if n < 0:
        return -n
    else:
        return n
```
Il exixte aussi un mot clé *elif* qui correspond à *sinon-si* 

---
#  Branchement conditionel multiple










