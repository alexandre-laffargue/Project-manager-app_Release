# Project Manager App

Bienvenue sur **Project Manager App**, votre solution complète de gestion de projet agile. Cette application web moderne, inspirée des standards de l'industrie comme Jira et Trello, vous permet de piloter vos projets de A à Z grâce à une interface intuitive et des fonctionnalités puissantes.

## Fonctionnalités Principales

L'application s'articule autour de trois modules clés pour couvrir l'ensemble du cycle de vie de développement :

*   **Tableau Kanban** : Visualisez et gérez vos tâches quotidiennes avec un système de colonnes et de cartes en glisser-déposer.
*   **Backlog & Sprints** : Planifiez vos itérations, priorisez vos tickets (User Stories, Bugs) et organisez vos sprints.
*   **Chronologie (Gantt)** : Suivez l'avancement global de vos projets sur une ligne de temps interactive.

## Documentation

Nous avons mis à votre disposition une documentation complète pour chaque type d'utilisateur :

*   **[Guide Utilisateur](USER_GUIDE.md)** : Apprenez à utiliser l'application, gérer vos tâches et collaborer avec votre équipe.
*   **[Guide Administrateur](ADMIN_GUIDE.md)** : Instructions détaillées pour l'installation, le déploiement (Docker), la configuration et la maintenance du serveur.
*   **[Architecture Technique](ARCHITECTURE.md)** : Plongez dans les détails techniques de l'application (Vue.js, Node.js, MongoDB, Docker).
*   **Documentation API** : Une fois l'application lancée, la documentation Swagger est disponible sur `http://localhost:3000/api-docs`.

## Stack Technique

Ce projet repose sur une stack moderne et performante :

*   **Frontend** : Vue.js 3, Vite, TailwindCSS.
*   **Backend** : Node.js, Express.js.
*   **Base de données** : MongoDB.
*   **DevOps** : Docker, Docker Compose.
*   **Qualité** : ESLint, Prettier.

## Tests et Qualité

La qualité du code est assurée par une suite de tests automatisés utilisant **Vitest**.

### Lancer les tests Backend
Le backend dispose de tests unitaires et d'intégration (API, Base de données).
```bash
cd backend
npm install
npm test
```

### Lancer les tests Frontend
Le frontend est testé via des tests unitaires de composants et de logique (Stores, Composables).
```bash
cd frontend
npm install
npm test
```

## Installation Rapide

Pour démarrer l'application en quelques secondes avec Docker :

1.  Assurez-vous d'avoir Docker et Docker Compose installés.
2.  Clonez ce dépôt.
3.  Lancez la commande :
    ```bash
    docker compose up --build -d
    ```
4.  Accédez à l'application sur [http://localhost](http://localhost).

*Pour plus de détails, consultez le [Guide Administrateur](ADMIN_GUIDE.md).*

---
*Développé dans le cadre du Master Conduite de Projet - 2025/2026*
