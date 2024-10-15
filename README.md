# Docker Ynov : Application Full Stack (Backend Node.js, Frontend React, Base de Données PostgreSQL)

## Description

Ce projet est une application web complète avec un backend, un frontend, et une base de données. Il utilise Docker pour conteneuriser l'application et assurer une bonne gestion des ressources, la persistance des données, ainsi que la mise en réseau des différents composants.

### Structure de l'application :

- **Backend** : API développée en Node.js, qui interagit avec une base de données PostgreSQL.
- **Frontend** : Application web développée avec React, qui consomme l'API backend.
- **Base de données** : PostgreSQL pour la persistance des données.

## Prérequis

Avant de commencer, assurez-vous d'avoir installé les outils suivants :

- Docker : [Guide d'installation](https://docs.docker.com/get-docker/)
- Docker Compose : [Guide d'installation](https://docs.docker.com/compose/install/)

## Installation et configuration

### 1. Cloner le dépôt

Commencez par cloner le dépôt Git contenant le code source de l'application :

```bash
git clone https://github.com/KAlecs12/Docker-Ynov

### 2. Configuration du .env

Fichier .env à ajouter au dossier backend :

```bash
DB_HOST=db
DB_PORT=5432
DB_USER=user
DB_PASSWORD=password
DB_NAME=dockerYnov
NODE_ENV=production

Fichier .env a ajouter au dossier frontend :

```bash
REACT_APP_API_URL=http://localhost:3000

### 3. Lancer l'application avec Docker Compose

Une fois le dépôt cloné et les fichiers .env configurés, lancer l'application avec Docker Compose :

```bash
docker-compose up --build

### 4. Arrêt et suppression des conteneurs

Pour arrêter et supprimer les conteneurs, ainsi que les réseaux et volumes associés, exécuter la commande suivante :

```bash
docker-compose down


