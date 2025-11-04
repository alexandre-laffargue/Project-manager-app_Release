# Release – Project Manager App v1.0

## Informations générales
**Version :** v1.0  
**Date de release :** 3 décembre 2025  
**Nom du projet :** Project Manager App  
**Équipe :**  
- **Jeremy** – Backend & Tests  
- **Alexandre** – Frontend & Intégration  
- **Anis** – Frontend & Intégration  

---

## Objectif de la release
Livrer la première version **fonctionnelle, stable et documentée** de l’application web de gestion de projet inspirée de Jira et Trello.  
L’application intègre toutes les fonctionnalités principales : backlog, tableau Kanban, gestion des sprints, chronologie et automatisation CI/CD.

---

## Fonctionnalités principales

### Authentification
- Inscription et connexion sécurisées via JWT.  
- Gestion de la session utilisateur et redirection automatique.  

### Kanban
- Création, modification et suppression de cartes et colonnes.  
- Drag & drop fluide entre colonnes.  
- Sauvegarde persistante dans MongoDB.  

### Backlog
- Vue backlog avec liste des issues.  
- Création et tri des issues.  
- Planification des issues dans un sprint.  

###  Sprints
- Création, démarrage et clôture d’un sprint.  
- Gestion du statut (`planned`, `active`, `closed`).  
- Récapitulatif des issues terminées et reportées.  

### Chronologie (Gantt)
- Visualisation temporelle des issues par sprint.  
- Modification directe des dates par drag & drop.  
- Synchronisation automatique avec la base de données.  

### Pipeline CI/CD
- Exécution automatique des tests (Vitest) et lint à chaque push.  
- Build du front et du back sur GitHub Actions.  
- Badges de statut intégrés dans le README.  

### UI/UX
- Interface claire et cohérente.  
- Navigation fluide entre les vues principales (Backlog, Board, Chronologie).  
- Responsive sur desktop et mobile.  

---

##  Tests & Qualité


---

##  Correctifs notables


---

## 📦 Contenu du dépôt release
