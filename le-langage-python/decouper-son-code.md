# Découper son code

{% embed url="https://www.youtube.com/watch?v=LCDfphxORuA" %}

Dès que votre base de code grossis ou que vous souhaitez conceptualisé vos fonctionnalités, mettre ses différentes fonctions dans plusieurs fichiers à beaucoup d'intêrets.

Admettons que nous souhaitons créer plusieurs fonctions liées au math.

On va créer nos fonctions dans un fichier nommé `mathematique.py`

```python
# Nous sommes dans le fichier mathematique.py
def au_carre(x)
    """ Eléve un nombre donné au carré """
    return x**2

def sont_egaux(x, y):
    """ Vérifie si deux nombres sont égaux """
    if x == y:
        return True
        
    return False    
```

Maintenant, on souhaite utiliser ces fonctions dans notre programme principal. Il suffit d'utiliser le mot-clé "import".

```python
# Nous sommes dans le fichier main.py
import mathematique 

# On peut utiliser notre fonction pour mettre au carré le nombre deux par exemple : 
c = mathematique.au_carre(2)
print(c) # Affichera 4 étant donné que 2 * 2 = 4
```

