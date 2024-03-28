# Projet de Scraping et Analyse de Données de Crypto-Monnaies
Ce projet consiste à scraper les données des crypto-monnaies à partir d'un site web et à les analyser. Le code est écrit en Python et utilise les bibliothèques BeautifulSoup pour le scraping web et matplotlib pour l'analyse des données.

## Contenu du Projet
Le projet comprend les fichiers suivants :

**crypto_scrap.py:** Ce fichier contient le code Python pour scraper les données des crypto-monnaies à partir d'un site web, les filtrer et les insérer dans une base de données MySQL.

**README.md:** Ce fichier contient la documentation du projet, expliquant comment utiliser le code et fournissant des informations sur son fonctionnement.

## Installation
Pour exécuter ce projet, vous aurez besoin d'installer Python ainsi que Docker. Vous aurez également besoin d'un serveur MySQL pour stocker les données si vous le faites en local.

Assurez-vous d'avoir Python installé sur votre système. Vous pouvez le télécharger depuis le site officiel de Python.

Installez les bibliothèques requises en exécutant la commande suivante dans votre terminal :

```
pip install bs4 matplotlib mysql-connector-python requests
```

Assurez-vous d'avoir un serveur MySQL en cours d'exécution. Vous pouvez installer MySQL depuis MySQL Downloads.

## Utilisation

Lancer la commande suivante avec docker en fonctionnement sur votre poste si vous devez build le fichier py : 

```
docker-compose up --build 
```

Sinon :

```
docker-compose run
```

### Options

-e VERBOSE=true app : Affiche les datas scrapées avant la mise en BDD (commande pour docker)

-e URL="Votre_URL" app : Permet de changer l'url de requête (déconseillé de modifier sauf si changement sur CoinMarketCap)

Vous pouvez également explorer les autres parties du code pour personnaliser ou étendre les fonctionnalités du projet selon vos besoins.

