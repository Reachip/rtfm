# Installer un package avec pip sur Debian

{% embed url="https://www.youtube.com/watch?v=IhvUhQeQ7Nk" %}

## Qu'est ce qu'un package Python ? 

Un package est un ensemble de fichier Python qui contiennent un ensemble de fonctions et/ou de classes Python. Il permet d'englober une API. Cette dernière permet d'utiliser des fonctions spécifiques à un besoin. 

Par exemple , il existe une API Python pour faire un serveur HTTP  : Flask 

Ou encore une API pour extraire du contenu en HTML : Beautiful Soup 

Python livre plusieurs API nativement \(c'est à dire sans devoir les installer manuellement comme nous allons le voir\).

Par exemple, on peut utiliser l'API Tkinter sans devoir l'installer qui sert à réaliser des interfaces graphiques. 

### Les gestionnaires de packages

Un gestionnaire de paquets est un outil automatisant le processus d'installation, désinstallation, mise à jour de logiciels installés sur un système informatique. En l'occurence, un package est aussi reconnu comme un logiciel.

#### PIP pour Python

PIP est le gestionnaire de paquets officiel de Python. Il permet très brièvement de récupérer un package Python. On peut facilement l'installer avec le gestionnaire de paquet intégrer à la distribution LInux utilisé. Sur Windows, PIP est installé automatiquement, dans les deux cas il faudra juste un accès à un terminal de commande \(invite de commande sur Windows\).

#### Le gestionnaires de paquet Debian

C'est le gestionnaire de package utilisé par la distribution LInux Debian. On retrouve cette distribution sur les Raspberry PI par exemple et dans la majorité des serveurs.

#### Quelques commandes nécessaires

```bash
# Mettre à jour les logiciels de la machine cible
sudo apt update; sudo apt upgrade 

# Installer PIP
sudo apt install python3-pip 
```

## Installer un package Python

Maintenant que pip est installé, il suffit d'indiquer à ce dernier quel package on souhaite installer sur notre machine.

Pour connaître la liste des packages disponibles, sur internet vous pouvez consulter ce site : [https://pypi.org/](https://pypi.org/)

Par exemple, je souhaite installer le module `requests` dont on peut s'informer à cette adresse : [https://pypi.org/project/requests/](https://pypi.org/project/requests/)

Pour l'installer dans l'espace utilisateur, il suffit d'indiquer au terminal : 

```bash
pip3 install --user requests
```

On peut alors importer le package dans n'importe quel script crée : 

```python
import requests # Comme un module interne 

# ...
```

