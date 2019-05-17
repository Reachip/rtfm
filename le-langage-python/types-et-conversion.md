# Types et conversion

Si vous ne savez pas ce qu'est un type : [https://fr.wikiversity.org/wiki/Python/Les\_types\_de\_base](https://fr.wikiversity.org/wiki/Python/Les_types_de_base)

## Les concepts de typage dynamique et de typage fort

Python est un langage au typage dynamique est fort. C'est-à-dire très concrètement que :

* On ne peut pas faire d'opérations quelconques entre deux types différents
* On peut manipuler des données sans devoir préciser son type et réaliser des opérations qui s'adapte au contexte du code que l'on écrit. Il s'agit du duck-typing.

## Exemple

### Le typage fort

Essayons d'additionner un nombre de type "int" en Python avec un caractère de type "string" en Python : 

```python
>>> 1 + "1" 
```

L'interpréteur Python renvoie : 

```text
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for +: 'int' and 'str'
```

On ne peut tout simplement par additionner une chaîne de caractères ou un caractère avec un nombre à cause du typage fort.

Par contre, si je veux additionner deux nombres ou deux chaînes de caractères : 

```python
>>> 1 + 1
2
>>> "Salut " + "ça va ?"
'Salut ça va ?'
>>>
```

Python ne renvoie aucune erreur.

### Le typage dynamique

Déclarons une variable : 

```python
a = "Une chaîne de caractère" 
b = 10
c = 1.5
```

On observe que nous n'avons pas besoin de préciser que la variable "a" est une chaîne de caractère, que "b" est de type int ou que "c" est de type float.

L'interpréteur Python le déduira tout seul.

## Convertir un type en un autre type

Il est donc très courant de vouloir convertir un type en un autre type en programmation. Tellement que Python nous permet de le faire avec beaucoup de facilité.

L'exemple le plus courant pour un débutant est le fait de vouloir convertir l'entrée clavier de l'utilisateur renvoyer par la fonction input\(\) de type "str" \(chaîne de caractères\) en type "int". 

```python
nombre_utilisateur = input("Saisir un nombre à additioner avec deux") 
"""
Pour convertir la chaîne de caractères 
stocké dans la constante "nombre_utilisateur", 
on applique la fonction int() sur la valeur en 
question à convertir en type int. 
"""
print(2 + int(nombre_utilisateur)) 
```

Les fonctions de conversion portent le même nom que le type que l'on veut récupérer lors de la conversion.

Par exemple, pour convertir le nombre 10 en str, on va utiliser la fonction str\(\), on obtiendra donc "10" à la place de 10.

## Connaître le type d'une variable/valeur

Parfois, il est utile lors des phases de développement de vouloir connaître le type d'une entité que l'on a dans notre programme. Pour ça on utilise la fonction type.

### Exemple 

```python
>>> x = 23333.89999
>>> type(x)
<class 'float'>
```

Ici, on nous indique que la valeur x est de type "float". Nous nous intéresserons plus tard au terme "class" indiqué par l'interpréteur.

