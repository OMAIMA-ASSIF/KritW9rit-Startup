# KritW9rit — Plateforme dédiée aux étudiants marocains 🇲🇦

KritW9rit est une plateforme web moderne conçue pour faciliter la vie des étudiants marocains, en leur offrant un espace unique pour **trouver un logement**, **chercher une colocation**, **découvrir des activités**, et **communiquer facilement** avec d’autres utilisateurs via un système de messagerie intégré.

L’objectif principal est de centraliser plusieurs besoins essentiels des étudiants dans une seule application fiable, sécurisée et simple d’utilisation.

---

## 🎯 Objectif du projet

De nombreux étudiants rencontrent des difficultés pour :
- trouver un logement adapté et fiable,
- trouver des colocataires sérieux,
- rester informés sur les opportunités et activités étudiantes,
- communiquer rapidement avec les propriétaires ou autres étudiants,
- éviter les arnaques et annonces frauduleuses.

**KritW9rit** répond à ces problèmes en proposant une solution complète et structurée.

---

## 🚀 Fonctionnalités principales

### 🏠 Gestion des annonces (Housing / Colocation / Activities)
- Publication d’annonces de logement
- Publication d’annonces de colocation
- Publication d’annonces d’activités
- Consultation des annonces (liste + détails)
- Formulaires dédiés pour créer/modifier une annonce

---

### ⭐ Système de favoris
- Enregistrer des annonces intéressantes
- Accéder rapidement à sa liste personnelle de favoris

---

### 💬 Messagerie instantanée
- Communication directe entre utilisateurs
- Envoi et réception de messages
- Gestion des conversations

---

### 🔔 Notifications
- Notifications automatiques pour rester informé des nouveautés
- Alertes liées aux messages ou actions importantes

---

### ⭐ Reviews (Avis & évaluations)
- Possibilité de laisser un avis sur une annonce ou une expérience
- Amélioration de la confiance entre les utilisateurs

---

### 🚨 Signalements (Reports)
- Les utilisateurs peuvent signaler une annonce ou un comportement suspect
- Renforcement de la sécurité de la communauté

---

### 👤 Gestion des comptes utilisateurs
- Inscription et connexion sécurisée
- Vérification d’email
- Mot de passe oublié / reset password
- Gestion du profil utilisateur

---

### 🛠️ Espace Administrateur
Un module complet pour la modération :
- Gestion des utilisateurs
- Gestion des annonces
- Consultation des signalements
- Modération des avis
- Dashboard centralisé

---

## 🔐 Sécurité et authentification

Le projet intègre plusieurs mécanismes pour garantir la sécurité :
- Authentification via **JWT**
- Protection des routes sensibles via middleware
- Guards Angular côté frontend (auth, guest, role)
- Gestion des rôles (**User / Admin**)

---

## 🏗️ Architecture du projet

Le projet suit une architecture **Full Stack** divisée en deux parties :

- **Backend (API REST)** : Node.js / Express
- **Frontend (Client Web)** : Angular

---

## ⚙️ Backend (Node.js + Express)

Le backend représente le cœur logique du projet :  
il gère les utilisateurs, les annonces, les messages, les favoris, les notifications et la modération.

### 📌 Structure principale

- `config/` : configuration et connexion base de données
- `middleware/` : middleware d’authentification JWT
- `models/` : modèles MongoDB (User, Listings, Messages, etc.)
- `routes/` : routes API organisées par module
- `uploads/` : stockage des fichiers (avatars, images annonces)
- `utils/` : services utilitaires (ex: email)

### 📌 Modèles de données (models)

Le backend contient plusieurs modèles essentiels :
- `User` : utilisateurs et rôles
- `HousingListing` : annonces de logements
- `ColocationListing` : annonces de colocation
- `ActivityListing` : annonces d’activités
- `Favorite` : favoris utilisateurs
- `Message` : messages privés
- `Notification` : notifications
- `Review` : avis et évaluations
- `Report` : signalements

---

## 🎨 Frontend (Angular)

Le frontend représente l’interface utilisateur de KritW9rit.  
Il propose une navigation simple et fluide entre les différentes fonctionnalités.

### 📌 Pages principales

- Authentification : login, register, verify email, reset password
- Housing : list / detail / form
- Colocation : list / detail / form
- Activities : list / detail / form
- Favorites : annonces sauvegardées
- Messages : interface de chat
- Profile : gestion du profil
- Admin : dashboard complet (users, listings, reports, reviews)

### 📌 Services Angular

Les services permettent la communication avec le backend :
- `auth.service.ts`
- `housing.service.ts`
- `chat.service.ts`
- `translation.service.ts`
- `theme.service.ts`

### 📌 Sécurité Frontend

- Guards : `auth.guard`, `guest.guard`, `role.guard`
- Interceptor : `auth.interceptor` (injection automatique du token JWT)

---

## 🔄 Communication Frontend ↔ Backend

Le frontend Angular communique avec le backend via une API REST :

- Authentification (login/register/reset)
- Consultation et gestion des annonces
- Ajout aux favoris
- Messagerie et notifications
- Gestion du profil
- Administration et modération

---

## 🧩 Modules API disponibles

Le backend expose plusieurs modules structurés :

- `/auth` : inscription, connexion, reset password, verify email
- `/housing` : annonces logement
- `/colocation` : annonces colocation
- `/activity` : annonces activités
- `/favorite` : favoris
- `/message` : messagerie
- `/notification` : notifications
- `/review` : avis
- `/report` : signalements
- `/admin` : routes admin
- `/profile` : gestion profil

---

## 🖼️ Gestion des fichiers uploadés

Les images sont stockées côté serveur dans :
- `uploads/avatars/` : avatars utilisateurs
- `uploads/housing/` : images des logements

---

## 🛠️ Technologies utilisées

### Backend
- Node.js
- Express.js
- MongoDB / Mongoose
- JWT Authentication
- Email Service (Verification / Reset)
- Upload de fichiers (images)

### Frontend
- Angular
- TypeScript
- Guards & Interceptors
- Services HTTP
- Routing

---

## 🌍 Vision du projet

KritW9rit vise à devenir une référence au Maroc pour les étudiants en proposant :
- un accès rapide à des annonces fiables,
- une communauté active,
- un système sécurisé et modéré,
- une expérience utilisateur moderne.

---

## 📌 Statut du projet

🚧 Projet en développement actif (Startup)  
📍 Ciblage actuel : **Étudiants marocains**

---

## 👩‍💻 Équipe

Ce projet est développé dans le cadre d’une startup.  
Je suis **cofondatrice** du projet **KritW9rit**.

---

## 📬 Contact

Pour toute collaboration, partenariat ou question :

📧 Email : [your_email]  
🔗 LinkedIn : [your_linkedin]  
🌐 Website : [your_website_if_exists]

---
