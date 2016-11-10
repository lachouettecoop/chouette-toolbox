# La Chouette Coop - Toolbox

Ce projet contient différents outils / prototypes pour "[La chouette coop](http://lachouettecoop.fr/)".

* Générateur de feuille imprimable de codes-barres des produits : https://lachouettecoop.github.io/chouette-toolbox/barcodes/ 
* Générateur de code-barre unique à La Chouette Coop pour des produits : https://lachouettecoop.github.io/chouette-toolbox/barcode-gen/ 

*Pour rejoindre l'aventure au sein du groupe informatique contactez moi ou
utilisez le site !*

## Pré-requis

* récupérer le projet (`git clone`)
* avoir [Docker](http://docs.docker.com/) et [Docker Compose](http://docs.docker.com/compose/install/) installé

## Utilisation

Pour lancer l'application exécutez simplement la commande :

```
docker-compose up -d
```

## Déploiement

La branche `master` est automatiquement rendue disponible sur le web. Il suffit donc de publier vos modifications afin qu'elles apparaissent en ligne en quelques minutes.

### Bonus

Si vous avez [nginx-proxy](https://github.com/jwilder/nginx-proxy) en place (suivre procédure de lancement très simple sur la doc) le site sera accessible à l'url : http://toolbox.lachouettecoop.test/

Il vous faudra un long timeout configuré pour nginx-proxy sinon des problèmes pourraient survenir à l'installation d'extensions. Exemple :

```
proxy_connect_timeout 600;
proxy_send_timeout 600;
proxy_read_timeout 600;
send_timeout 600;
```

## Licence

[GPL v2.0](LICENSE)