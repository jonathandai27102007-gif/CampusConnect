# CampusConnect

> Plateforme permettant aux étudiants de **découvrir les événements universitaires** et de **s'y inscrire**.

![Statut](https://img.shields.io/badge/statut-conception-orange)

## Présentation et objectifs
Les événements de l'université (conférences, ateliers, soirées associatives, forums) sont aujourd'hui annoncés sur des canaux dispersés. CampusConnect vise à :
- **centraliser** les événements universitaires en un seul endroit ;
- **simplifier l'inscription** des étudiants ;
- donner aux **organisateurs** une visibilité sur le nombre de participants.

## État réel du projet
🟠 **Phase de conception.** Aucune fonctionnalité n'est développée à ce jour et aucune version installable n'existe.

Travaux réalisés :
- Product Backlog et Sprint 1 dans Jira (projet `CC`) ;
- spécification fonctionnelle de l'inscription (SPEC-01, User Story CC-8) ;
- diagrammes UML de conception (cas d'utilisation, classes, séquence).

Les instructions d'installation seront ajoutées lorsque le premier incrément sera développé.

## Fonctionnalités envisagées
| Fonctionnalité | Description | Jira | État |
|----------------|-------------|------|------|
| Consulter | Liste des événements à venir et fiche détaillée | CC-5, CC-7 | Envisagée |
| Rechercher | Recherche par mot-clé, date ou catégorie | CC-6 | Envisagée |
| S'inscrire | Inscription à un événement, gestion « complet » et « déjà inscrit » ; annulation ; « Mes inscriptions » | CC-8, CC-9, CC-10 | Spécifiée (SPEC-01) |
| Gérer les événements | Création, modification, annulation, liste des inscrits (organisateur) | CC-11, CC-12, CC-13 | Envisagée |
| Se connecter | Authentification (mode à confirmer avec le PO) | CC-14 | Envisagée |

## Outils
| Outil | Usage |
|-------|-------|
| **Jira** | Product Backlog, User Stories, Sprints — projet `CC` : <https://erwanfantonimartinet.atlassian.net/jira/software/projects/CC/boards/35> |
| **Confluence** | Documentation fonctionnelle, technique, agile et guide utilisateur — espace *CampusConnect* : `<lien de l'espace Confluence>` |
| **GitHub** | Versionnement de la documentation, des sources UML et, plus tard, du code |
| **draw.io** | Diagrammes UML (fichiers sources `.drawio`) |

## Documentation
- 📘 Espace Confluence CampusConnect : `<lien de l'espace Confluence>`
  - 01 — Présentation du projet · 02 — Documentation fonctionnelle (SPEC-01) · 03 — Documentation technique · 04 — Gestion Agile · 05 — Guide utilisateur
- 📐 Diagrammes UML (sources éditables avec <https://app.diagrams.net/>) :
  - [Cas d'utilisation](docs/uml/CampusConnect_01_cas_utilisation.drawio)
  - [Classes](docs/uml/CampusConnect_02_classes.drawio)
  - [Séquence — inscription](docs/uml/CampusConnect_03_sequence_inscription.drawio)
  - [Fichier regroupant les 3 diagrammes](docs/uml/CampusConnect_UML.drawio)

## Structure du dépôt
```
.
├── README.md
└── docs/
    └── uml/        sources draw.io des diagrammes UML
```

## Consignes de contribution
1. **Partir d'un ticket Jira** : tout changement correspond à un ticket `CC-x`.
2. **Créer une branche** nommée `CC-x-description-courte` (ex. `CC-8-spec-inscription`).
3. **Messages de commit** préfixés par la clé Jira : `CC-8 : ajoute le critère CA4`.
4. **Pull Request** obligatoire, relue par au moins un autre membre de l'équipe avant fusion dans `main`.
5. **Diagrammes** : modifier le fichier `.drawio` source (jamais seulement l'image) et mettre à jour la page Confluence 03.
6. **Règles métier** : ne pas introduire de règle non validée ; la marquer « À confirmer PO » et ouvrir une question dans Jira.
7. **Cohérence** : toute modification d'une User Story est répercutée dans Jira, Confluence et ce README.

## Équipe
Équipe Scrum CampusConnect — Product Owner, Scrum Master et équipe de développement (voir Confluence › 01 — Présentation du projet).
