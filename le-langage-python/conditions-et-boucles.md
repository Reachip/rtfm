# Conditions et boucles

{% embed url="https://www.youtube.com/watch?v=LYlHV6ikPLQ" %}

## Les conditions

Prenons l'exemple d'un fast-food américain pour vieux beauf. Vous êtes équipier dans le fast-food, logiquement,  chaque client à un choix à faire entre plusieurs menus : 

* Hamb -bourgeur diabète Premium 
* Frites haute-pression artérielle
*  Glace nappé de gras

A chaque commande, vous avez le choix de choisir ces deux choses en fonction du choix du client.

On peut traduire ce procéder comme ça :

```text
Si le client choisis Hamb-bourgeur diabète Premium alors lui donner le Hamb-bourgeur diabète Premium
Sinon si le client choisis Frites haute-pression artérielle alors lui donner Frites haute-pression artérielle
Sinon si le client choisis Glace nappé de gras alors lui donner Glace nappé de gras
Sinon, ne rien lui donner
```

En Python ça donne ça :

```python
choix_client = input("Quel est votre choix monsieur ?") 

if choix_client == "Hamb-bourgeur diabète Premium":
    print("Et voilà votre Hamb -bourgeur diabète Premium. Bonne journée") 
    

elif choix_client == "Frites haute-pression artérielle":
    print("Et voilà vos Frites haute-pression artérielle. Bonne journée")

elif choix_client == "Glace nappé de gras":
    print("Et voilà votre Glace nappé de gras. Bonne journée")
    
else:
    print("Ce menu n'existe pas, bonne journée")
```

Ici, "if" veut dire "si" en anglais, "elif" peut se traduire par "sinon si" et "else" par sinon. Remarquez que l'on met toujours les ":" à la fin de la déclaration de la condition en Python.

Ici, j'ai tester une égalité avec l'opérateur "==". On peut aussi tester la différence avec l'opérateur "!=" qu'on peut traduire par : "Si ceci est différent de cela" ou comme en math, tester si on nombre et supérieur ou inférieur avec "&gt;" ou "&lt;". 

## Les boucles

Virez directement votre client parce qu'il n'a pas fait le bon choix semble vraiment bête. On va une "boucle" dans notre algorithme afin d'exprimer cela : **"Tant que le client ne choisis pas un menu proposé par le fast-food, on lui repose la question : "Quel est votre choix monsieur ?"."** 

Pour faire ce genre de boucle, on va utiliser la boucle "while" qui peut-être traduite par "tant que". 

```python
choix_client = input("Quel est votre choix monsieur ?") 
a_choisis = False 

# Tant que a_choisis est faux, on lui re-demande son choix et vérifie ce qu'il a choisis
while a_choisis == False: 
    choix_client = input("Quel est votre choix monsieur ?") 
    
    if choix_client == "Hamb -bourgeur diabète Premium":
        print("Et voilà votre Hamb -bourgeur diabète Premium. Bonne journée")
         # On met a_choisis à True, ce qui fait arrêter la boucle 
        a_choisis = True
    
    elif choix_client == "Frites haute-pression artérielle":
        print("Et voilà vos Frites haute-pression artérielle. Bonne journée")
         # On met a_choisis à True, ce qui fait arrêter la boucle
        a_choisis = True
    
    elif choix_client == "Glace nappé de gras":
        print("Et voilà votre Glace nappé de gras. Bonne journée")
        
    else:
        print("Ce menu n'existe pas, bonne journée")
```

##  La boucle for avec la fonction range\(\)

Revenons à un exemple plus "académique".

## Cas d'utilisation de la boucle for 

La boucle for s'utilise quand on sait que quand la boucle va s'arrêter. Par exemple on veut afficher 10 fois quelque chose, on ne va pas utiliser la boucle "while" mais plutot la boucle "for"

Un exemple d'algorithme en langage naturelle :

```text
Pour x allant de 0 à 10
    Afficher "Bonjour"
```

Ici, x est le "compteur" de la boucle. C'est une variable qui à chaque tours va s'incrémenter

* Au premier tour X = 0
* Au deuxième X = 1
* Au troisième X = 2
* Et ainsi de suite 

La même chose en Python donne :

```python
for x in range(0, 10):
    print("Bonjour") 
```

Rien de bien compliqué. La chose nouvelle est la fonction range\(\), sont rôle et de généré une liste de nombre allant de 0 à 10. Cela permet d'afficher 10 fois "bonjour".

Afin de se rendre compte que X change à chaque tours, on peut afficher "Bonjour" avec la valeur de X.

```text
for x in range(0, 10):
    print(f"Bonjour {x} fois")
```

**N'oubliez pas le "f" entre la parenthèses ouvrante et la chaîne de caractère à afficher !** 

