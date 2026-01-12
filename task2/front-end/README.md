
# Softy Pinko - Front-end (Task 2)

Ce dossier contient le front-end statique de l'application Softy Pinko, servi par Nginx dans un conteneur Docker.

## Fichiers
- **Dockerfile** : Image Docker basée sur Nginx, copie les fichiers statiques et la configuration personnalisée.
- **softy-pinko-front-end.conf** : Configuration Nginx pour servir le site sur le port 9000.
- **softy-pinko-front-end/** : Répertoire contenant le site web (HTML, CSS, JS, images, etc.).
- **README.md** : Ce fichier d'explication.

## Instructions

### 1. Construction de l'image
Dans ce dossier (`task2/front-end`), exécutez :
```bash
docker build -t softy-pinko-front-end:task2 .
```

### 2. Exécution du conteneur
```bash
docker run -it --rm -p 9000:9000 --name softy-pinko-front-end softy-pinko-front-end:task2
```

### 3. Accès à l'application
Ouvrez votre navigateur à l'adresse :
```
http://localhost:9000/
```
Vous devriez voir la page d'accueil du site Softy Pinko.

## Explications
- L'image utilise Nginx latest.
- Les fichiers statiques sont copiés dans `/var/www/html/softy-pinko-front-end`.
- Le port 9000 est exposé pour accéder au site.
- La configuration Nginx personnalisée permet de servir le front-end.

## Auteur
Aurelie
