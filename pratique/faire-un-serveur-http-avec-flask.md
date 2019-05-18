# Faire un serveur HTTP avec Flask

{% embed url="https://www.youtube.com/watch?v=ltxW1ixL6w4" %}

Pour savoir de quoi on parle : [https://fr.wikipedia.org/wiki/Serveur\_HTTP](https://fr.wikipedia.org/wiki/Serveur_HTTP)

## Flask 

Flask est considéré comme un "micro-framework" Python. Il se veut minimaliste et simple mais offrant toutes les fonctionnalitées afin de développer unh serveur web de qualité. 

## Première impression 

Voici un exemple de code simple : 

```python
import flask 

app = flask.Flask() 

# On accedera à cette page web via http://monsite/premiere_page
@app.route("/premiere_page")  
def index():
    # Quand le client accède à http://monsite/premiere_page, le navigateur 
    # retournera en tant que titre HTML "Première page web"  
    return "<h1>Première page web</h1>" 
    
app.run(host="0.0.0.0") # On "lance" le serveur
```

## Exemple 

![](../.gitbook/assets/ezgif.com-video-to-gif-1.gif)

### Pourquoi http://localhost:5000 ?

Décortiquons l'adresse : 

| http:// | localhost | :5000 |
| :--- | :--- | :--- |
| Indique que l'on souhaite utiliser le protocole http | Indique l'on souhaite communiquer avec sa propre machine en réseau | Indique que l'on souhaite communiquer via le port 5000 |

_**Plus d'infos concernant "localhost" ici :**_ [https://fr.wikipedia.org/wiki/Localhost](https://fr.wikipedia.org/wiki/Localhost)

_**Plus d'infos  concernant les ports ici :**_ [https://fr.wikipedia.org/wiki/Port\_\(logiciel](https://fr.wikipedia.org/wiki/Port_%28logiciel%29)\)

