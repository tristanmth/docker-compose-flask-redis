# Docker Compose Flask Redis

Application web simple utilisant Flask, Redis et Docker Compose.

## 📌 Description

Ce projet met en place une application web Python utilisant Flask.  
Elle affiche un compteur de visites stocké dans Redis.

Le projet sert d’exemple pour comprendre :
- Docker
- Docker Compose
- Communication entre conteneurs
- Persistance des données avec volumes
- Développement avec Compose Watch

---

## 🚀 Technologies utilisées

- Python 3.12
- Flask
- Redis
- Docker
- Docker Compose

---

## ⚙️ Installation et exécution

### 1. Cloner le projet
```bash
git clone <URL_DU_REPO>
cd docker-compose-flask-redis
````

### 2. Lancer l’application

```bash
docker compose up --watch
```

### 3. Accéder à l’application

```
http://localhost:8000
```

---

## 📁 Structure du projet

```
.
├── app.py
├── requirements.txt
├── Dockerfile
├── compose.yaml
├── infra.yaml
├── .env
└── .dockerignore
```

---

## 🔧 Fonctionnement

* Flask expose une route `/`
* Redis stocke le compteur de visites
* Docker Compose orchestre les services
* Un volume permet de conserver les données Redis
* Compose Watch permet le rechargement automatique du code

---

## 🧹 Reset des données

Pour supprimer les données Redis :

```bash
docker compose down -v
```

---

## 👨‍💻 Auteur

Projet réalisé dans le cadre d’un TP Docker / Docker Compose.
