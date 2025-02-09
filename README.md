# Microservices

# Registre de Personnes - API Node.js & SQLite

Ce projet est une API REST simple permettant de gérer un registre de personnes à l'aide de Node.js, Express et SQLite.

## 📌 Fonctionnalités

- 📄 **Afficher toutes les personnes** (`GET /personnes`)
- 🔍 **Afficher une personne par ID** (`GET /personnes/:id`)
- ➕ **Ajouter une nouvelle personne** (`POST /personnes`)
- ✏️ **Mettre à jour une personne** (`PUT /personnes/:id`)
- ❌ **Supprimer une personne** (`DELETE /personnes/:id`)

## 🚀 Installation et Exécution

### 1️⃣ Prérequis
- [Node.js](https://nodejs.org/)
- [SQLite3](https://www.sqlite.org/)

### 2️⃣ Installation des dépendances
```sh
npm install
```

### 3️⃣ Exécution du serveur
```sh
node index.js
```
Le serveur démarrera sur `http://localhost:3000`.

## 🛠 Technologies utilisées
- **Node.js** - Environnement d'exécution JavaScript
- **Express.js** - Framework web pour Node.js
- **SQLite** - Base de données légère

## 📁 Structure du projet
```
/compte_rendu_tp2_sqa
│── node_modules/
│── database.js        # Connexion et gestion de la base de données
│── index.js           # Configuration et définition des routes de l'API
│── maBaseDeDonnees.sqlite  # Base de données SQLite
│── package.json       # Fichier de configuration des dépendances
│── README.md          # Documentation du projet
```

## 📝 Exemple d'utilisation avec CURL

### 1️⃣ Récupérer toutes les personnes
```sh
curl -X GET http://localhost:3000/personnes
```

### 2️⃣ Ajouter une personne
```sh
curl -X POST http://localhost:3000/personnes -H "Content-Type: application/json" -d '{"nom":"John Doe","adresse":"123 Rue Principale"}'
```

### 3️⃣ Modifier une personne
```sh
curl -X PUT http://localhost:3000/personnes/1 -H "Content-Type: application/json" -d '{"nom":"Jane Doe","adresse":"456 Avenue Centrale"}'
```

### 4️⃣ Supprimer une personne
```sh
curl -X DELETE http://localhost:3000/personnes/1
```

