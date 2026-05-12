<div align="center">

# 🌍 FEVEO Backend Demo

### Plateforme de gestion des GIE — Groupements d'Intérêt Économique

*Backend API démo pour la souveraineté économique des femmes au Sénégal* 🇸🇳

</div>

---

<div align="center">

[![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square)](https://github.com/alpha-do-code/feveo-backend-demo)
[![License](https://img.shields.io/badge/license-MIT-yellow?style=flat-square)](LICENSE)
[![Node.js](https://img.shields.io/badge/Node.js-18.x-green?style=flat-square&logo=node.js)](https://nodejs.org)
[![Made for](https://img.shields.io/badge/Made_for-FEVEO_2050-red?style=flat-square)](https://feveo2050.sn)

![Last Commit](https://img.shields.io/github/last-commit/alpha-do-code/feveo-backend-demo?style=flat-square)
![Repo Size](https://img.shields.io/github/repo-size/alpha-do-code/feveo-backend-demo?style=flat-square)
![Stars](https://img.shields.io/github/stars/alpha-do-code/feveo-backend-demo?style=social)

</div>

---

## 📖 À propos

**FEVEO Backend Demo** est une API REST de démonstration pour la gestion des **Groupements d'Intérêt Économique (GIE)** au Sénégal. Conçue dans le cadre de la mission de **FEVEO 2050** pour la souveraineté économique et l'autonomisation des femmes, cette API permet d'enregistrer les GIE, gérer leurs bureaux (présidente, secrétaire, trésorière), suivre les cotisations et automatiser les opérations administratives.

Ce projet sert également de **terrain de pratique DevOps** pour explorer les workflows Git/GitHub professionnels (Conventional Commits, Pull Requests, CI/CD).

---

## ✨ Fonctionnalités

### 🏢 Gestion des GIE

- 📝 **Enregistrer un GIE** avec ses informations complètes (nom, région, commune, secteur d'activité)
- 👥 **Gérer le bureau** : présidente, secrétaire, trésorière (avec validation des rôles)
- 🔄 **Modifier ou supprimer** un GIE existant
- 📋 **Lister les GIE** avec filtres par région, arrondissement, statut

### 💰 Suivi financier

- 💵 **Enregistrer les cotisations** mensuelles des membres
- 📊 **Tableau de bord** des contributions par GIE et par période
- 🧾 **Générer des reçus PDF** automatiquement (intégration n8n/WeasyPrint)

### 🔐 Sécurité & Authentification

- 🗝️ **Authentification JWT** avec gestion de rôles (admin, présidente, membre)
- 🛡️ **Validation des données** avec Joi sur tous les endpoints
- 🚨 **Rate limiting** pour prévenir les abus d'API

### 🌍 Multi-localisation

- 📍 **Hiérarchie administrative** : région → département → arrondissement → commune
- 🇸🇳 **Couverture nationale** : 14 régions du Sénégal préchargées

---

## 🛠️ Tech Stack

<div align="center">

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

</div>

### 📦 Détail des technologies

| Catégorie | Technologie | Rôle |
|-----------|-------------|------|
| **Runtime** | [Node.js 18.x](https://nodejs.org/) | Environnement d'exécution JavaScript côté serveur |
| **Framework** | [Express.js](https://expressjs.com/) | Framework web minimaliste pour construire l'API REST |
| **Base de données** | [MongoDB](https://www.mongodb.com/) + [Mongoose](https://mongoosejs.com/) | Stockage NoSQL flexible pour les GIE et utilisateurs |
| **Authentification** | [JSON Web Tokens](https://jwt.io/) | Authentification stateless avec tokens signés |
| **Validation** | [Joi](https://joi.dev/) | Validation des données entrantes (body, query, params) |
| **Tests** | [Jest](https://jestjs.io/) + [Supertest](https://github.com/ladjs/supertest) | Tests unitaires et d'intégration de l'API |
| **Conteneurisation** | [Docker](https://www.docker.com/) | Empaquetage de l'application pour le déploiement |
| **CI/CD** | [GitHub Actions](https://github.com/features/actions) | Pipeline d'intégration et déploiement continu |
| **Automation** | [n8n](https://n8n.io/) | Génération de PDF (lettres de cotisation, reçus) |

### 🏗️ Architecture

```
feveo-backend-demo/
├── src/
│   ├── controllers/   # Logique métier des endpoints
│   ├── models/        # Schémas Mongoose
│   ├── routes/        # Définition des routes API
│   ├── middlewares/   # Auth, validation, error handling
│   ├── services/      # Logique réutilisable
│   └── utils/         # Helpers, constantes
├── tests/             # Tests Jest
├── .github/
│   └── workflows/     # GitHub Actions
├── Dockerfile         # Image Docker
└── docker-compose.yml # Stack locale complète

```

---

## 📜 License

Ce projet est distribué sous la **License MIT** — voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

---

## 👤 Auteur

<div align="center">

### **Alpha (Mamadou Alpha BALDE)**

*Développeur en reconversion DevOps · FEVEO 2050 SAS · Keur Massar, Dakar, Sénégal* 🇸🇳

[![GitHub](https://img.shields.io/badge/GitHub-alpha--do--code-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/alpha-do-code)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:alphab045@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)

</div>

---

## 🙏 Remerciements

- **FEVEO 2050 SAS** — Pour l'inspiration et le contexte métier
- **GitHub Student Developer Pack** — Pour les outils qui financent ce parcours d'apprentissage
- **Diilaye** — Mentor et partenaire de code

---

<div align="center">

**⭐ Si ce projet t'a aidé ou inspiré, n'hésite pas à mettre une étoile !**

*Made with ❤️ in Dakar*

</div>