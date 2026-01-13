# Softy Pinko - Projet Docker

Ce dépôt regroupe plusieurs exercices et solutions autour de la conteneurisation d'une application web (Softy Pinko) avec Docker, docker-compose, Nginx, Flask, et la gestion multi-services.

## Structure du projet

Chaque dossier `taskX/` correspond à une étape ou un exercice progressif :

- **task0/** : Premier Dockerfile simple (Hello World)
- **task1/** : API Flask minimaliste dans un conteneur
- **task2/** : Séparation back-end (Flask) et front-end (Nginx)
- **task3/** : Ajout de flask-cors, structure améliorée
- **task4/** : Orchestration avec docker-compose (back + front)
- **task5/** : Ajout d'un proxy (Nginx) devant les services
- **task6/** : Scalabilité du back-end (plusieurs instances), load balancing via proxy

Chaque dossier contient ses propres instructions et fichiers nécessaires (Dockerfile, docker-compose.yml, etc.).

## Lancer la version la plus avancée (task6)

```bash
cd task6
docker-compose up --build --scale back-end=2
```

Accès :
- Front-end : http://localhost:9000/
- API : http://localhost:5252/api/hello

## Prérequis
- Docker
- docker-compose

## Auteur
Aurelie