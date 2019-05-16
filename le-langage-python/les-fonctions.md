---
description: Comme en math ...
---

# Les fonctions

{% embed url="https://www.youtube.com/watch?v=3kw2sttGXMI" %}



## Introduction : la fonction print

En général, dans la plupart des guides en programmation et dans n'importe quels lanages, on apprend en tout premier lieu à afficher quelque chose à l'écran. En Python on peut très facilement faire ça avec une fonction qui s'appelle print.

### Qu'est ce qu'une fonction en programmation ?

Tout est expliqué ici : 

[https://fr.wikiversity.org/wiki/Introduction\_g%C3%A9n%C3%A9rale\_%C3%A0\_la\_programmation/Fonctions](https://fr.wikiversity.org/wiki/Introduction_g%C3%A9n%C3%A9rale_%C3%A0_la_programmation/Fonctions) 

### Comment concrètement afficher quelque chose à l'ecran ?

Comme ça : 

```text
print("Bonjour") 

# Sur votre écran sera affiché "bonjour"     
```

Techniquement parlant, print est une fonction prenant n'importe quel type afin de l'afficher.

On peut donc aussi facilement afficher un nombre, une addition, ou même le résultat d'une autre fonction:

```python
print(1) 
```

##  Créer une fonction 

On peut utiliser une fonction mais aussi en créer une. 

### Créer une fonction par l'exemple 

```python
def le_nom_de_ma_fonction(un_parametre, un_autre_parametre):
    print(un_parametre + un_autre_parametre) 
```

Ici, j'ai créer une fonction nommée le\_nom\_de\_ma\_fonction acceptant deux paramètres qui affiche l'addition de ses paramètres.

