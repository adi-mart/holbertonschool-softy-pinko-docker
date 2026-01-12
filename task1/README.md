docker build -t softy-pinko:task0 .
docker run -it --rm --name softy-pinko-task0 softy-pinko:task0

# Softy Pinko - Task 1

Ce projet montre comment créer une API Flask dans un conteneur Docker basé sur Ubuntu.

## Fichiers
- **Dockerfile** : Définit l'image Docker, installe Python3, pip3 et Flask, et lance l'API.
- **api.py** : Script Python qui expose un endpoint `/api/hello` retournant "Hello, World!".
- **README.md** : Ce fichier d'explication.

## Instructions

### 1. Construction de l'image
Dans le dossier `task1`, exécutez :
```bash
docker build -t softy-pinko:task1 .
```

### 2. Exécution du conteneur
```bash
docker run -p 5252:5252 -it --rm --name softy-pinko-task1 softy-pinko:task1
```

### 3. Test de l'API
Dans votre navigateur ou avec curl, accédez à :
```
http://localhost:5252/api/hello
```
Vous devez obtenir :
```
Hello, World!
```

## Explications
- L'image utilise Ubuntu latest.
- Installe Python3, pip3 et Flask.
- Supprime la restriction EXTERNALLY-MANAGED si nécessaire.
- Copie le script api.py et lance le serveur Flask sur le port 5252.

## Auteur
Aurelie
