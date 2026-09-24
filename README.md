# MarieTeam - Projet AP 3-4 (2SLAM 2026-2027)

Projet réalisé dans le cadre de l'AP (Accompagnement Personnalisé) pour la compagnie de transport maritime **MarieTeam**, en collaboration avec l'ESN **VDEV**.

## Sommaire

- [Contexte](#contexte)
- [Réalisations professionnelles](#réalisations-professionnelles)
- [Répartition des tâches (2 personnes)](#répartition-des-tâches-2-personnes)
- [Planning prévisionnel](#planning-prévisionnel-20-semaines)
- [Environnement de travail](#environnement-de-travail)
- [Suivi d'avancement](#suivi-davancement)

---

## Contexte

MarieTeam assure la desserte maritime d'îles du littoral français (Belle-Île, Houat, Groix, Ouessant, etc.). Le projet couvre deux activités :

- **Transport de voyageurs** (réservation en ligne, tarifs, horaires)
- **Fret** (évolution future)

VDEV est l'ESN chargée de développer les outils pour MarieTeam.

## Réalisations professionnelles

| # | Réalisation | Type |
|---|---|---|
| RP1 | Application web de gestion de transport voyageur | Client léger (Web) |
| RP2 | Client lourd - édition de brochures PDF | Application objet |
| RP3 | Application mobile native (capitaines) | Mobile |
| RPT | Gestion des incidents (GLPI) | Transversale |

Base de données à implémenter sur **Windows/MySQL** et **Linux/PostgreSQL** (environnement virtualisé).

---

## Répartition des tâches (2 personnes)


### Personne A — Côté "Données + Web (RP1)"

- [ ] Dictionnaire de données détaillé
- [ ] MCD (Merise 2) + MLD
- [ ] Script de création BDD + jeu d'essai (MySQL sous Windows)
- [ ] Diagramme de cas d'utilisation - RP1 (site web)
- [ ] Description textuelle des cas d'utilisation - RP1
- [ ] Maquettage IHM (composants nommés) - RP1
- [ ] Développement RP1 : consultation liaisons / tarifs / horaires
- [ ] Développement RP1 : réservation en ligne + fidélisation (bonus 25 pts / ristourne 100 pts)
- [ ] Authentification gestionnaire + sécurité du site
- [ ] Statistiques gestionnaire (CA, passagers transportés, par catégorie)
- [ ] Rapport de tests RP1

### Personne B — Côté "Client lourd (RP2) + Mobile (RP3) + Incidents"

- [ ] Implémentation BDD miroir (PostgreSQL sous Linux/Ubuntu virtualisé)
- [ ] Diagramme de classes UML (Bateau / BateauVoyageur / BateauFret / Equipement)
- [ ] Développement classes techniques `Passerelle`, `JeuEnregistrement`, `PDF`
- [ ] Procédure `BrochurePDF` (génération BateauVoyageur.pdf)
- [ ] Diagramme + description des cas d'utilisation - RP2
- [ ] Maquettage IHM - RP2 (interfaces gestionnaire)
- [ ] Tests unitaires + rapport de tests RP2
- [ ] RP3 : choix smartphone, schéma BDD SQLite locale + code de sauvegarde
- [ ] RP3 : synchronisation local ↔ serveur
- [ ] RP3 : consultation BDD serveur depuis mobile
- [ ] Paramétrage GLPI (droits par client / par technicien / responsable)
- [ ] Tests de validation du paramétrage GLPI

### Tâches communes (à faire à deux, ou en alternance)

- [ ] Veille technologique (stratégie de recherche, sources, synthèse)
- [ ] Étude d'une technologie/outil/méthode (potentiel et limites)
- [ ] Choix des architectures logicielles (documenté et justifié)
- [ ] Charte graphique commune
- [ ] Règles de nommage des variables (respect notation Pascal/Camel imposée)
- [ ] Documentation technique HTML (RP2)
- [ ] Portefeuille de compétences (à jour régulièrement, **pas à la dernière minute**)
- [ ] Planning de projet (Gantt) tenu à jour
*-----------

## Planning prévisionnel (20 semaines)

| Semaines | Étape |
|---|---|
| S1-S2 | Analyse du cahier des charges, choix techno, MCD/MLD |
| S3-S5 | Dictionnaire de données, scripts BDD (MySQL + PostgreSQL), spécifications |
| S6-S10 | Développement RP1 (web) |
| S11-S14 | Développement RP2 (client lourd, brochure PDF) |
| S15-S17 | Développement RP3 (mobile) |
| S18 | Paramétrage GLPI + tests |
| S19 | Tests globaux, rapports de tests |
| S20 | Finalisation documentation, portefeuille de compétences |

---

## Environnement de travail

- **Gestion de version** : Git / GitHub (ce dépôt)
- **Documents collaboratifs** : Google Drive / Office 365
- **Suivi de projet** : GLPI (RPT) + outil de planning (GanttProject, Trello, etc.)

### Structure de dépôt suggérée

```
marieteam-projet/
├── README.md
├── rp1-web/
├── rp2-client-lourd/
├── rp3-mobile/
├── bdd/
│   ├── mcd-mld/
│   ├── scripts-mysql/
│   └── scripts-postgresql/
├── documentation/
│   ├── cas-utilisation/
│   ├── maquettes-ihm/
│   └── charte-graphique/
├── glpi/
└── tests/
```

---

## Suivi d'avancement

| Date | Auteur | Avancement |
|---|---|---|
| | | |

[lien d'un exemplaire qu'on va se baser sur ](https://mairie-team.lovable.app/)
