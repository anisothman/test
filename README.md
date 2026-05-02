# 🎓 QCM — Fondamentaux des Tests Logiciels (ISTQB)

Une application web interactive permettant de s'entraîner aux **fondamentaux du test logiciel (ISTQB Foundation Level)** à travers des QCM générés par IA.

---

## 🚀 Aperçu

Cette application propose :

* 📚 20 questions uniques à chaque session
* 🎯 3 niveaux de difficulté : Facile, Intermédiaire, Difficile
* 🤖 Génération dynamique via API (Anthropic)
* 🔄 Mode fallback avec questions locales
* 📊 Score détaillé + correction complète
* 🎨 Interface moderne et responsive

---

## 🧠 Fonctionnalités principales

### 🔑 Gestion de clé API

* Saisie de la clé API Anthropic
* Stockage sécurisé dans le navigateur (`localStorage`)
* Validation automatique

### 🎯 Choix du niveau

* 🌱 **Facile** → définitions et bases
* ⚡ **Intermédiaire** → principes ISTQB
* 🔥 **Difficile** → analyse avancée

### 🤖 Génération du quiz

* Appel API vers Claude 3.5 Sonnet
* Génération de 20 QCM uniques
* Format JSON strict

### 📝 Quiz interactif

* Affichage question par question
* Feedback immédiat :

  * ✅ bonne réponse
  * ❌ mauvaise réponse
* 💡 Explication affichée

### 📊 Résultats détaillés

* Score en pourcentage (animation circulaire)
* Statistiques :

  * bonnes réponses
  * mauvaises réponses
* 📋 Revue complète des réponses

### 🔄 Mode fallback

Si l’API échoue :

* Utilisation automatique d’un pool local de questions

---

## 🛠️ Technologies utilisées

* HTML5
* CSS3 (animations custom)
* JavaScript Vanilla
* API : Anthropic (Claude 3.5 Sonnet)

---

## 📂 Structure du projet

project/
│
├── index.html   # Application complète (UI + logique JS)
└── README.md    # Documentation

---

## ⚙️ Installation & Utilisation

### 1. Télécharger le projet

* Télécharger le fichier ou cloner le repo

### 2. Ouvrir l’application

* Double-cliquer sur `index.html`

👉 Aucun serveur nécessaire (fonctionne en local)

---

### 3. Ajouter une clé API

1. Aller sur : https://console.anthropic.com
2. Créer une clé API
3. Coller la clé dans l’application

---

## 🔐 Sécurité

* La clé API est :

  * stockée uniquement en local
  * jamais envoyée ailleurs que vers Anthropic

⚠️ Attention : usage côté navigateur (non recommandé en production)

---

## 📈 Améliorations possibles

* Backend pour sécuriser la clé API
* Version mobile optimisée
* Export PDF des résultats
* Leaderboard
* Timer par question
* Support multilingue

---

## 🧑‍💻 Auteur

Anis Othman
📍 Medenine, Tunisie

---

## 📄 Licence

Projet open-source et libre d’utilisation.
