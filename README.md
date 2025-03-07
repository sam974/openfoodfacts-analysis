# Projet : Système de Nettoyage et Exploration des Données Open Food Facts

Ce projet se concentre sur le nettoyage et l'exploration du jeu de données Open Food Facts de plus 800 Mo via l'écosystème [pandas](https://pandas.pydata.org/).
Il s'agit ensuite d'évaluer la faisabilité d'une solution sur base d'un système de suggestion et d'auto-complétion.

---

## Objectifs du projet

Le projet répond à plusieurs objectifs clés :

- **Nettoyage des données** : Identifier et traiter les valeurs manquantes et aberrantes dans le jeu de données Open Food Facts.
- **Exploration des données** : Produire des visualisations pour comprendre les variables pertinentes et leur comportement.
- **Automatisation** : Développer un système robuste capable de gérer les modifications légères du jeu de données (ajout ou suppression d'entrées).
- **Analyse multivariée** : Sélectionner ou créer des variables pertinentes pour améliorer la qualité des suggestions.

---

## Fonctionnalités principales

### 1. Traitement des données

- Identification des variables pertinentes pour les analyses.
- Nettoyage des valeurs manquantes avec au moins trois méthodes adaptées :
    - Imputation par médiane
    - Suppression conditionnelle des entrées non exploitables.
    - Détection et gestion des valeurs aberrantes via :
- Analyse statistique (écarts-types, quartiles).
    - Visualisations (boxplots, histogrammes).
- Automatisation du traitement pour garantir une compatibilité avec les modifications du jeu de données.


### 2. Visualisation des données

- Analyse univariée pour chaque variable pertinente :
    - Histogrammes pour les distributions.
    - Diagrammes circulaires pour les catégories.
    - Nuages de points pour les corrélations.
- Création de graphiques lisibles et variés adaptés à un public néophyte.


### 3. Analyse multivariée

- Sélection ou création de nouvelles variables basées sur les corrélations entre les données.
- Tests statistiques pour vérifier la significativité des résultats.

---

## Installation

1. Installez les dépendances nécessaires :

```bash
pip install -r requirements.txt
```

2. Téléchargez le jeu de données Open Food Facts depuis [le site officiel](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/parcours-data-scientist/P2/fr.openfoodfacts.org.products.csv.zip) et placez-le dans le répertoire `data/`.

---

## Utilisation

### Étape 1 : Nettoyage des données

### Étape 2 : Analyse univariée et bivariée

### Étape 3 : Analyse multivariée (ACP & ANOVA)


---

## Structure du projet

```
├── data/                                               # Répertoire contenant les jeux de données
│   └── fr.openfoodfacts.org.products.cleaned.csv       # Sample généré suite à l'analyse
├── notebooks/                                          # Notebooks Jupyter pour analyses exploratoires
├── README.md                                           # Documentation du projet
└── requirements.txt                                    # Dépendances Python nécessaires au projet
```

---

## Résultats attendus

1. Un jeu de données nettoyé, prêt à être utilisé pour développer un système de suggestion.
2. Des visualisations claires illustrant la structure et le comportement des variables.
3. Une analyse multivariée permettant d'identifier les variables clés pour la suggestion automatique.

---