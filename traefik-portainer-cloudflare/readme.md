
# Mise en place de Traefik et Portainer pour la gestion de services Docker

Ce guide explique comment déployer Traefik et Portainer pour gérer les services Docker de manière efficace et sécurisée. Nous utiliserons GitHub pour gérer et versionner les fichiers de configuration.

## Prérequis

- Docker et Docker Compose installés sur le serveur.
- Un compte GitHub pour la gestion des configurations.
- Un domaine configuré pour pointer vers votre serveur.
- Ajouter CNAME sur votre domaine sur cloudflare

## Configuration et déploiement

### 1. Cloner le dépôt

Clonez ce dépôt sur votre serveur local ou de production :

```bash
git clone https://github.com/Nasticks/devops-labs.git
cd devops-labs/traefik-portainer-cloudflare
```

### 2. Configuration des fichiers
docker-compose.yml : Ce fichier contient la configuration de tous les services, y compris Traefik et Portainer.

dynamic.yml : Fichier de configuration dynamique pour Traefik.
Assurez-vous de personnaliser ces fichiers selon vos besoins, notamment les paramètres liés aux domaines et aux certificats SSL.

Déployer avec Docker Compose
Exécutez les commandes suivantes pour démarrer tous les services :

```bash
docker-compose up -d
````

### 3. Accéder à Portainer
Une fois les services démarrés, accédez à Portainer en ouvrant votre navigateur à l'adresse suivante :


https://votre-domaine.com
Suivez les instructions pour compléter la configuration de Portainer.

Sécurité
Assurez-vous de configurer les règles de firewall et de sécuriser l'accès aux interfaces web avec HTTPS, si nécessaire.
