# Sprint 1 – Authentification & Kanban statique

## Période
Du **23 octobre au 5 novembre**

---

## Objectif principal
Mettre en place la **première version fonctionnelle** de l’application avec :
- un système **d’authentification utilisateur** (inscription / connexion) ;
- la **structure du tableau Kanban** avec colonnes statiques ;
- une **navigation de base** entre les vues principales ;
- une **première version du pipeline CI**.

Ce sprint vise à obtenir un MVP stable pour poursuivre le développement des fonctionnalités cœur au sprint suivant.

---

## User Stories incluses

| ID | Description | Priorité | Estimation |
|----|--------------|-----------|-------------|
| **US1.1** | En tant que visiteur, je veux m’inscrire avec un email et un mot de passe pour créer un compte. | Must | 5 |
| **US1.2** | En tant qu’utilisateur, je veux me connecter à mon compte pour accéder à mes données. | Must | 5 |
| **US2.1** | En tant qu’utilisateur, je veux voir mon tableau principal avec des colonnes statiques (To Do, In Progress, Done). | Must | 5 |
| **US2.2** | En tant qu’utilisateur, je veux pouvoir ajouter, renommer ou supprimer une colonne. | Must | 5 |
| **US7.2** | En tant qu’utilisateur, je veux naviguer simplement entre les vues principales. | Must | 4 |
| **US6.2 (partiel)** | Mettre en place une première version du pipeline CI. | Should | 3 |

**Total estimé : 27 points**

---

## Plan de travail (Sprint backlog)

### Backend – A
- Créer les routes **/auth/register** et **/auth/login**
- Gérer les tokens **JWT**
- Configurer la base **MongoDB** (collection `users`)
- Préparer la structure backend pour le **module Kanban**

### Frontend – B & C
- Pages **Login** et **Register**
- Page **Kanban statique** avec colonnes “To Do / In Progress / Done”
- Composants Vue.js pour les colonnes et les cartes
- Navigation basique entre **Login**, **Kanban**, et **Accueil**
- Configuration **Prettier + ESLint**
- Début de pipeline CI (GitHub Actions – build & test simple)

---

## Avancement prévu
- Authentification complète (register / login)
- Tableau Kanban visible et interactif (structure de base)
- Navigation fluide entre les vues principales
- CI minimale en place (test du build et du lint)

---

## Difficultés anticipées
- Gestion sécurisée du token JWT côté frontend
- Configuration du pipeline (GitHub Actions, Vitest)
- Organisation du code Vue.js pour préparer le Kanban dynamique

---

## Résultats attendus
À la fin du sprint :
- L’utilisateur peut **s’inscrire et se connecter**.
- Le tableau Kanban s’affiche avec **colonnes statiques**.
- La base du projet (front/back) est stable et prête pour évolution.
- Une **pipeline CI de base** fonctionne sur GitHub (lint + build + test).

---

## Rétrospective *(à compléter en fin de sprint)*
| Points positifs | Axes d’amélioration |
|--------------------|------------------------|

---

## Objectifs pour le Sprint 2
- Rendre le **Kanban dynamique** (cartes et colonnes persistantes)
- Créer le **backlog produit**
- Ajouter la **gestion des sprints**
- Écrire les **premiers tests unitaires**
- Finaliser la **pipeline CI complète**
