

# Softy Pinko - Back-end (Task 6)


Ce dossier contient le back-end de l'application Softy Pinko, développé avec Flask (et flask-cors) et conteneurisé avec Docker.

## Fichiers
- **Dockerfile** : Image Docker basée sur Ubuntu, installe Python, Flask, flask-cors et lance l'API.
- **api.py** : Application Flask exposant un endpoint simple `/api/hello` (CORS activé).
- **README.md** : Ce fichier d'explication.

## Instructions

### 1. Lancer avec docker-compose
Dans le dossier parent, exécutez :
```bash
docker-compose up --build --scale back-end=2
```

### 2. Accès à l'API
Ouvrez votre navigateur ou utilisez `curl` pour accéder à :
```
http://localhost:5252/api/hello
```
Vous devriez obtenir :
```
Hello, World!
```

## Explications
- L'image utilise Ubuntu latest.
- Installe Python 3, pip, Flask et flask-cors.
- Active CORS pour permettre les requêtes du front-end.
- Copie le code de l'API dans le conteneur.
- Expose le port 5252 pour accéder à l'API Flask.

## Auteur
Aurelie
