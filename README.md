# Backlog – Project Manager App

## Objectif du projet
Développer une application web de gestion de projet inspirée de Trello et Jira.  
L’application permet la gestion complète des tâches à travers trois vues principales :
- **Backlog** : liste des issues à planifier  
- **Tableau (Kanban)** : suivi des tâches par statut  
- **Chronologie (Gantt)** : visualisation temporelle des issues  

---

## Technologies utilisées
| Composant | Outil / Framework | Rôle |
|------------|------------------|------|
| Frontend | **Vue.js** | Interface utilisateur réactive et modulaire |
| Backend | **Node.js (Express)** | API REST performante |
| Base de données | **MongoDB** | Gestion flexible des tâches et utilisateurs |
| Authentification | **JWT (JSON Web Tokens)** | Sécurisation de l’accès utilisateur |
| Tests | **Vitest** / **Selenium** | Tests unitaires et end-to-end |
| DevOps | **Docker**, **GitHub Actions** | Conteneurisation & CI/CD |

---

## Équipe & rôles
| Membre | Rôle principal |
|---------|----------------|
| **A** | Backend & Tests |
| **B** | Frontend & Intégration |
| **C** | Frontend & Intégration |

---

## Modules principaux
- Gestion des utilisateurs (comptes, rôles, authentification)
- Gestion des issues (bugs, problèmes)
- Gestion des tâches (création, édition, suivi)
- Gestion des releases (versions logicielles)
- Gestion des tests (qualité, vérification)
- Documentation technique et utilisateur

---

## Planning des sprints

| Sprint | Dates | Objectif principal |
|---------|--------|-------------------|
| Sprint 0 | 15 oct – 22 oct | Mise en place et cadrage |
| Sprint 1 | 23 oct – 5 nov | MVP du tableau Kanban |
| Sprint 2 | 6 nov – 19 nov | Gestion du backlog et des sprints |
| Sprint 3 | 20 nov – 3 déc | Chronologie et finitions |

---

## Backlog (User Stories par Epic)

### **EPIC 0 – Infrastructure et mise en place**
| ID | User Story | Priorité | Sprint | Estimation |
|----|-------------|-----------|----------|-------------|
| US0.1 | Initialiser le dépôt GitHub (front + back). | Must | 0 | 2 |
| US0.2 | Mettre en place le Project Board et les labels. | Must | 0 | 2 |
| US0.3 | Configurer lint + prettier pour la qualité du code. | Must | 1 | 3 |
| US0.4 | Ajouter un README clair avec instructions de lancement. | Must | 1 | 2 |

---

### **EPIC 1 – Authentification et utilisateurs**
| ID | User Story | Priorité | Sprint | Estimation |
|----|-------------|-----------|----------|-------------|
| US1.1 | Inscription avec email et mot de passe. | Must | 1 | 5 |
| US1.2 | Connexion utilisateur. | Must | 1 | 5 |

---

### **EPIC 2 – Tableau (vue Kanban)**
| ID | User Story | Priorité | Sprint | Estimation |
|----|-------------|-----------|----------|-------------|
| US2.1 | Voir le tableau principal avec colonnes et cartes. | Must | 1 | 5 |
| US2.2 | Ajouter, renommer ou supprimer une colonne. | Must | 1 | 5 |
| US2.3 | Ajouter, modifier ou supprimer une carte. | Must | 1 | 5 |
| US2.4 | Déplacer une carte entre colonnes (drag & drop). | Must | 1 | 8 |
| US2.5 | Sauvegarder colonnes et cartes dans la base. | Must | 1 | 6 |

---

### **EPIC 3 – Backlog**
| ID | User Story | Priorité | Sprint | Estimation |
|----|-------------|-----------|----------|-------------|
| US3.1 | Voir toutes les issues dans un backlog unique. | Must | 2 | 5 |
| US3.2 | Créer une issue avec titre, description, priorité, type. | Must | 2 | 6 |
| US3.3 | Réordonner les issues dans le backlog. | Should | 2 | 5 |
| US3.4 | Planifier une issue dans un sprint. | Should | 2 | 7 |

---

### **EPIC 4 – Sprints**
| ID | User Story | Priorité | Sprint | Estimation |
|----|-------------|-----------|----------|-------------|
| US4.1 | Créer un sprint (nom, dates début/fin). | Must | 2 | 5 |
| US4.2 | Démarrer un sprint planifié. | Must | 2 | 5 |
| US4.3 | Clôturer un sprint et voir les issues terminées. | Should | 3 | 6 |

---

### **EPIC 5 – Chronologie (vue Gantt)**
| ID | User Story | Priorité | Sprint | Estimation |
|----|-------------|-----------|----------|-------------|
| US5.1 | Voir les issues sous forme de barres temporelles. | Must | 3 | 7 |
| US5.2 | Déplacer/redimensionner une barre pour ajuster les dates. | Should | 3 | 8 |

---

### **EPIC 6 – Tests et intégration**
| ID | User Story | Priorité | Sprint | Estimation |
|----|-------------|-----------|----------|-------------|
| US6.1 | Écrire des tests unitaires pour les fonctions critiques. | Must | 2 | 5 |
| US6.2 | Pipeline GitHub Actions pour exécuter les tests. | Should | 2 | 4 |

---

### **EPIC 7 – Améliorations UX/UI**
| ID | User Story | Priorité | Sprint | Estimation |
|----|-------------|-----------|----------|-------------|
| US7.1 | Interface claire et cohérente. | Could | 3 | 4 |
| US7.2 | Navigation fluide entre Backlog, Tableau et Chronologie. | Must | 2 | 4 |

---

## Synthèse par sprint

| Sprint | Objectif principal | US clés | Estimation totale |
|---------|--------------------|---------|-------------------|
| **Sprint 0** | Préparation du cadre projet | US0.1, US0.2 | 4 |
| **Sprint 1** | MVP du tableau Kanban | US1.1 → US2.5 | 34 |
| **Sprint 2** | Backlog + sprints + tests unitaires | US3.1 → US4.2, US6.1, US6.2, US7.2 | 46 |
| **Sprint 3** | Chronologie et finitions | US4.3, US5.1, US5.2, US7.1 | 25 |

---

## Synthèse des priorités
**Must have**
- Authentification  
- Tableau Kanban (CRUD + drag & drop)  
- Backlog produit (vue liste)  
- Gestion des sprints  
- Tests unitaires simples (Vitest)  
- Pipeline GitHub Actions  
- Navigation entre vues  

**Should have**
- Filtrage, réorganisation du backlog  
- Chronologie simplifiée  
- Interface plus fluide  

**Could have**
- Amélioration visuelle  
- Filtres/recherche avancée  
- Thème clair/sombre (bonus)
