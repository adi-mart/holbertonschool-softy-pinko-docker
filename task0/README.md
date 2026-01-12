# Softy Pinko - Task 0

Ce projet contient un exemple simple d'utilisation de Docker avec Ubuntu.

## Fichiers
- **Dockerfile** : Définit l'image Docker basée sur Ubuntu et affiche "Hello, World!" à l'exécution.
- **README.md** : Ce fichier d'explication.

## Instructions

### 1. Construction de l'image
Dans le dossier `task0`, exécutez :
```bash
docker build -t softy-pinko:task0 .
```

### 2. Exécution du conteneur
```bash
docker run -it --rm --name softy-pinko-task0 softy-pinko:task0
```

### 3. Résultat attendu
Le conteneur affichera :
```
Hello, World!
```

## Explications
- L'image utilise Ubuntu latest.
- Met à jour le système.
- Affiche un message simple à l'exécution.

## Auteur
Aurelie
