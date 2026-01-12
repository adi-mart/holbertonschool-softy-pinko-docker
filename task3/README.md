

# Softy Pinko - Task 3


Ce dossier contient la solution Dockerisée de l'application Softy Pinko, composée d'un back-end (API Flask avec flask-cors) et d'un front-end statique (servi par Nginx).

## Structure du dossier
- **back-end/** : Contient l'API Flask et son Dockerfile
- **front-end/** : Contient le site statique, la configuration Nginx et son Dockerfile
- **README.md** : Ce fichier d'explication global

## Démarrage rapide


### 1. Construire les images
Dans chaque dossier (`back-end` et `front-end`), exécutez :

Pour le back-end :
```bash
cd back-end
docker build -t softy-pinko-back-end:task3 .
```

Pour le front-end :
```bash
cd ../front-end
docker build -t softy-pinko-front-end:task3 .
```

### 2. Lancer les conteneurs


Back-end (API Flask sur le port 5252) :
```bash
docker run -it --rm -p 5252:5252 --name softy-pinko-back-end softy-pinko-back-end:task3
```

Front-end (site statique sur le port 9000) :
```bash
docker run -it --rm -p 9000:9000 --name softy-pinko-front-end softy-pinko-front-end:task3
```


### 3. Accès
- API : http://localhost:5252/api/hello
- Site : http://localhost:9000/


## Détails
Consultez les README dans `back-end/` et `front-end/` pour plus d'informations sur chaque service (notamment l'utilisation de flask-cors côté back-end).

## Auteur
Aurelie
