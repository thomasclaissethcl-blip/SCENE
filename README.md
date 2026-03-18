# SCENE : Système de Création d’Expériences Narratives à Embranchements

SCENE est un outil web permettant de concevoir des parcours interactifs de type *livre dont vous êtes le héros*, notamment pour des usages pédagogiques, des simulations professionnelles et des serious games.

Le projet fournit une chaîne complète de conception :

- génération d’une structure narrative
- édition détaillée des scènes
- définition de la logique décisionnelle
- export d’une expérience interactive autonome

L’objectif est de permettre à un concepteur pédagogique ou à un formateur de produire rapidement des scénarios interactifs structurés sans dépendre d’un framework complexe.

---

# Principe général

Un parcours SCENE fonctionne comme une histoire interactive composée de scènes reliées par des choix.

Chaque scène :
- présente une situation
- fournit du contexte narratif
- propose des décisions

Chaque choix :
- modifie l’état du parcours
- influence les scènes accessibles
- produit des conséquences visibles ou invisibles

Le système repose sur trois composants :

- les **scènes** (structure narrative)
- les **choix** (navigation)
- les **variables** (mémoire du parcours)

Logique simplifiée :
`Scène → Choix → Modification de l’état → Nouvelle scène`

Cette approche permet de construire des simulations pédagogiques où les conséquences dépendent de l’ensemble des décisions prises.

---

# Structure du projet

Le projet est organisé autour de trois interfaces principales.

## 1. Page d’accueil

**index.html**

Rôle :

- expliquer le principe narratif
- présenter la logique des embranchements
- décrire le workflow
- accès au générateur de templates et au builder

Objectif :

Servir de point d’entrée pédagogique pour comprendre le système.

---

## 2. Générateur de templates

**templateGenerator.html**

Cet outil permet de générer une architecture de scénario à partir de paramètres :

- type de parcours :
  - prise de décision
  - gestion de crise
  - apprentissage progressif

- contexte
- complexité
- logique pédagogique

Production :

- structure de scènes
- fonctions narratives
- types de décisions
- JSON exploitable

Objectif :

Accélérer la phase de conception initiale.

---

## 3. Builder (éditeur de projet interactif)

**gameDesigner.html**

Outil principal de conception.

Fonctionnalités :

### Création du projet

- titre
- auteur
- scène de départ
- nombre d’étapes

### Conception des scènes

- contenu narratif
- dialogues
- images
- transitions

### Logique du parcours

- variables
- règles conditionnelles
- effets des choix

### Analyse structurelle

- visualisation JSON
- diagnostics
- cohérence logique

### Export

- sauvegarde projet (JSON)
- export HTML autonome

Le builder constitue le cœur fonctionnel du système.

---

# Workflow recommandé

Le projet suit une logique progressive.

## Étape 1 / Générer une structure

Utiliser le générateur de templates.

Objectif :

Obtenir une base narrative cohérente.

## Étape 2 / Structurer le projet

Importer ou créer le projet dans le builder.

Définir :

- métadonnées
- progression
- structure générale

## Étape 3 / Concevoir les scènes dans le builder

Créer :

- situations
- décisions
- conséquences

Objectif :

Construire la narration interactive.

## Étape 4 / Définir la logique

Configurer :

- variables
- règles
- conditions

Objectif :

Donner du sens aux décisions.

## Étape 5 / Exporter

Générer un HTML autonome utilisable :

- en formation
- en LMS
- en démonstration
- en prototype

---

# Technologies utilisées

Architecture volontairement simple :

- HTML
- CSS
- JavaScript vanilla

Aucune dépendance externe.

Objectifs :

- portabilité
- simplicité
- lisibilité
- modification facile

---

# Installation

Aucune installation nécessaire.

Télécharger le dépôt puis ouvrir :
`index.html`
dans un navigateur.

---

# Utilisation rapide

Workflow minimal :
1. ouvrir templateGenerator.html
2. générer une structure
3. ouvrir gameDesigner.html
4. construire les scènes
5. exporter en HTML


---

# Cas d’usage

## Formation

- mises en situation professionnelles
- entraînement décisionnel
- simulations managériales

## Pédagogie

- apprentissage par scénario
- évaluation formative
- parcours adaptatifs

## Prototype

- serious games
- design narratif
- démonstrateurs pédagogiques

---

# Philosophie du projet

Principes :

**Simplicité technique**

Pas de dépendances lourdes.

**Lisibilité**

Code compréhensible.

**Pédagogie**

Pensé pour les concepteurs pédagogiques.

---

# Fonctionnalités actuelles

- génération de structure narrative
- éditeur de scènes
- gestion des variables
- règles conditionnelles
- diagnostics structurels
- export HTML autonome
- import/export JSON

---

# Améliorations possibles

Extensions envisagées :

- visualisation graphique des embranchements
- éditeur avancé des variables
- bibliothèque de templates

---

# Roadmap

- [x] Générateur de structure
- [x] Éditeur narratif
- [x] Export HTML
- [ ] Visualisation graphique des branches
- [ ] Validation logique automatique
- [ ] Export SCORM

---

# Contribution

Projet actuellement expérimental et entièrement personnel.

Contributions possibles :

- amélioration UI
- optimisation code
- nouvelles mécaniques narratives
- documentation

---

# Licence
MIT  

---

# Auteur

Thomas Claisse
thomasclaisse.thcl@gmail.com

---

# État du projet

Prototype fonctionnel en évolution.

Utilisable pour :

- prototypage pédagogique
- démonstrateurs
- conception de scénarios interactifs

---
