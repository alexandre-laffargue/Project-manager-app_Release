# Sprint 1 – Détail des tâches

## Période
Du **23 octobre au 5 novembre**

---

## Objectif du sprint
Mettre en place la **première version fonctionnelle** du projet :
- Authentification (inscription / connexion)
- Tableau **Kanban statique**
- **Navigation** entre les vues principales
- Pipeline **CI minimale** (lint + test)

---

## Répartition des rôles
| Membre | Rôle principal |
|---------|----------------|
| **A** | Backend & Tests |
| **B-C** | Frontend, Intégration & UI/UX |

---

## User Stories concernées
- **US1.1** : Inscription utilisateur  
- **US1.2** : Connexion utilisateur  
- **US2.1** : Afficher le tableau Kanban (statique)  
- **US2.2** : Gestion basique des colonnes  
- **US7.2** : Navigation entre les vues  
- **US6.2 (partiel)** : Pipeline CI minimale  

---

## Détail des tâches par User Story

### US1.1 – Inscription utilisateur
**A**
- Créer modèle `User` (email, passwordHash, createdAt)
- Créer endpoint `POST /auth/register`
- Hash du mot de passe
- Validation des champs (email, mot de passe)
- Tests unitaires sur la route `/auth/register`

**B-C**
- Créer page `Register.vue`
- Créer formulaire d’inscription (email + mot de passe)
- Appel API `POST /auth/register` via Axios
- Gestion des erreurs et affichage message d’erreur
- Redirection automatique vers `/login`
- Documentation : “Inscription utilisateur”

---

### US1.2 – Connexion utilisateur
**A**
- Créer endpoint `POST /auth/login`
- Génération du token JWT
- Middleware `verifyToken`
- Test unitaire sur la connexion et le JWT

**B-C**
- Créer page `Login.vue`
- Gérer la soumission du formulaire + appel API
- Stockage du token JWT dans `localStorage`
- Redirection vers la page Kanban après connexion
- Tests simples sur la redirection
- Documentation : “Connexion utilisateur”

---

### US2.1 – Afficher le tableau Kanban statique
**A**
- Créer modèle `Board` (title, owner)
- Créer endpoint `GET /boards/me` (mock statique)
- Tests de la route de récupération du board

**B-C**
- Créer page `Board.vue`
- Ajouter 3 colonnes statiques : *To Do / In Progress / Done*
- Créer le store Pinia `board` pour gérer les données
- Afficher cartes statiques avec composants Vue.js
- Tests unitaires sur le store
- Documentation : “Vue Kanban statique”

---

### US2.2 – Gestion basique des colonnes
**A**
- Créer endpoints CRUD (mock) :  
  - `POST /columns`, `PATCH /columns/:id`, `DELETE /columns/:id`
- Tests unitaires backend sur les routes CRUD

**B-C**
- Créer composant `AddColumnForm.vue`
- Gérer l’ajout, la modification et la suppression de colonnes
- Édition inline du titre
- Tests unitaires sur le store `addColumn()`
- Documentation : “Gestion des colonnes Kanban”

---

### US7.2 – Navigation entre les vues
**B-C**
- Créer barre de navigation globale (Header)
- Configurer **Vue Router** (routes : `/login`, `/board`, `/backlog`)
- Ajouter lien actif visuel
- Tests de navigation entre les vues
- Documentation : “Navigation principale”

---

### US6.2 (partiel) – Pipeline CI minimale
**A**
- Créer fichier `.github/workflows/ci.yml`
- Ajouter jobs : test (Vitest)
- Vérifier exécution sur GitHub Actions

**B-C**
- Ajouter badge CI dans le README
- Vérifier exécution du pipeline sur push
- Documentation : “Mise en place pipeline CI/CD”

---

## Récapitulatif par membre

| Membre | Tâches principales | Domaines |
|---------|--------------------|-----------|
| **A** | Auth backend, JWT, MongoDB, CI | Backend & Tests |
| **B-C** | Login/Register UI, Kanban statique, Navigation | Frontend, Intégration, UI/UX |

---

## Livrables attendus
- Authentification complète (register + login)
- Kanban statique avec 3 colonnes fixes
- Navigation entre vues principales fonctionnelle
- Pipeline CI minimale fonctionnelle
- Documentation utilisateur et technique à jour
