# Listes, tuples et dictionnaires

## Structurer ces données

Les listes, tuples et dictionnaires sont ce qu'on appelle des structures de données. Ces "structures" permettent de stocker de la donnée d'une certaine manière. Python étant un langage avec une forte abstraction, il vous permet nativement de stocker vos valeurs

* Sous forme de variables/constantes \(ce qui a été vu auparavant\)

```python
X = 5 # La donnée 5 est stockée dans une valeur appellé X
```

* Sous forme de listes et de tuples

```python
# Les données 1, 2 et 3 sont stockées dans une liste appellée MA_LISTE 
MA_LISTE = [1, 2, 3]

# Les données "Bonjour" et 1.5 sont stockées dans une liste appellée MA_LISTE 
UNE_AUTRE_LISTE = ["Bonjour", 1.5]

# Les données 1, 2 et 3 sont stockées dans un tuple appellée MON_TUPLE
MON_TUPLE = (1, 2, 3)
```

On peut évidemment stocker n'importe quels types dans une liste et un tuple. La différence entre un tuple et une liste est qu'**un tuple est immuable, c'est-à-dire qu'on ne peut pas ajouter, modifier ou supprimer des valeurs dans un tuple alors que les listes nous le permet.**

On peut accéder aux valeurs d'une liste ou d'un tuple en spécifiant "l'index" de l'élément voulu dans la liste/le tuple. L'index correspond à la position de l'élément par rapport à la liste.

```python
MA_LISTE = [21, 2.7, 98]

# X aura comme donnée 21.
# En informatique, on commence toujours par zéro.
X = MA_LISTE[0]

# Y aura comme donnée 2.7.
Y = MA_LISTE[1]

# Z aura comme donnée 98.
Z = MA_LISTE[2]

# Et ainsi de suite ...
```

On peut aussi utiliser la boucle "for" pour parcourir une liste ou un tuple : 

```python
T = ("Jean", "Paul", "Jack")

for prenom in T:
    print(f"Votre prénom est {prenom}")
    
"""
Ce nous affiche : 

Votre prénom est Jean
Votre prénom est Paul
Votre prénom est Jack 
"""
```

* Sous forme de dictionnaires  

```python
PERSONNAGE = {"age": 18, "poids": 150, "prenom": "René"}
```

On peut accéder à une valeur via une clé. Ainsi, pour accéder à l'age de notre personnage on fait : 

```python
PERSONNAGE = {"age": 18, "poids": 150, "prenom": "René"}

AGE_DU_PERSO = PERSONNAGE["age"]
print(AGE_DU_PERSO) 

"""
Ce qui nous affiche :
18
"""    
```

On peut accéder au poids en récupérant la clé `"poids"` en écrivant`PERSONNAGE["poids"]` et ainsi de suite ...

## Quelques opérations sur les listes, tuples et dictionnaires

_TODO_

## Les slices

_TODO_

