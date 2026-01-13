

# Softy Pinko - Task 5


Ce dossier contient la solution Dockerisée de l'application Softy Pinko, composée d'un back-end (API Flask avec flask-cors), d'un front-end statique (servi par Nginx) et d'une orchestration via docker-compose et un proxy.

## Structure du dossier
- **back-end/** : Contient l'API Flask et son Dockerfile
- **front-end/** : Contient le site statique, la configuration Nginx et son Dockerfile
- **README.md** : Ce fichier d'explication global


## Démarrage rapide

### 1. Lancer l'application avec docker-compose
Dans ce dossier, exécutez :
```bash
docker-compose up --build
```

### 2. Accès
- API : http://localhost:5252/api/hello
- Site : http://localhost:9000/

### 3. Détails
Consultez les README dans `back-end/`, `front-end/` et `proxy/` pour plus d'informations sur chaque service (notamment l'utilisation de flask-cors côté back-end).

## Auteur
Aurelie
