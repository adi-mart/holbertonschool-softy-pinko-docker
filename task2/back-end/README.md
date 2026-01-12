
# Softy Pinko - Back-end (Task 2)

Ce dossier contient le back-end de l'application Softy Pinko, développé avec Flask et conteneurisé avec Docker.

## Fichiers
- **Dockerfile** : Image Docker basée sur Ubuntu, installe Python, Flask et lance l'API.
- **api.py** : Application Flask exposant un endpoint simple `/api/hello`.
- **README.md** : Ce fichier d'explication.

## Instructions

### 1. Construction de l'image
Dans ce dossier (`task2/back-end`), exécutez :
```bash
docker build -t softy-pinko-back-end:task2 .
```

### 2. Exécution du conteneur
```bash
docker run -it --rm -p 5252:5252 --name softy-pinko-back-end softy-pinko-back-end:task2
```

### 3. Accès à l'API
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
- Installe Python 3, pip et Flask.
- Copie le code de l'API dans le conteneur.
- Expose le port 5252 pour accéder à l'API Flask.

## Auteur
Aurelie
