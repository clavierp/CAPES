Boucles : principes et exemples.
===
## Paul Clavier
Jeudi 18 Janvier

---
# Boucle
Instruction permettant de modifier le flot d'éxécution en fonction d'une condition booléenne et permettant la répétition d'un segent de l'algorithme.
Il en existe plusieurs types:
1. Boucle à pré-condition
2. Boucle à post-condition
3. Boucle itérative
4. Boucle de parcours

---
# Boucle à pré-condition
Boucle *while* ou *tant que*:
```
while condition:
	bloc répété
```
Tant que la condition est vrai, on recommence la boucle.
Si la condition est vrai, la boucle n'est pas parcourue.

---
# Exercice
En utilisant une boucle à pré-condition, faire la somme des 100 premiers entiers.

---
# Boucle à post-conditon
Boucle *do while*:
Identique à la boucle *while* mais la boucle est au moins parcourue une fois
```
int i = 1;
do {
i++;
} while(i < 10);
```
N'existe pas en Python

---
# Boucle itérative
Boucle *for* ou *pour*:
Parcours tous les états pour une variable entre l'état initial et l'état final en suivant le changement d'état donné.
```
for(int i = 0; i < 10; i++){
 printf("%d", i);
}
```
Affichera 0 1 2 3 4 5 6 7 8 9
En Python, on la retrouve avec une boucle de parcours et l'objet *range*
```
for i in range(10):
    print(i)
```
---
# Boucle de parcours
Boucle *for in*.
```
for i in [1,2,3,4,5]:
	foo(i)
```
La variable sera afféctée par les valeurs de l'objet parcouru successivement.





