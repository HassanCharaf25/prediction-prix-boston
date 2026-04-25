# Projet de Régression — Prédiction des Prix Immobiliers

## Description du projet

Ce projet d'analyse de données et de modélisation statistique a pour objectif de prédire le prix médian des logements à Boston (`MEDV`). À l'aide de techniques de régression et de réduction de dimensionnalité, nous cherchons à identifier les variables socio-économiques les plus influentes et à comparer la précision de différents modèles prédictifs.

## Jeu de données

Le projet utilise le célèbre dataset **Boston Housing** (`housing.csv`). Le jeu de données comprend 14 variables, dont les plus significatives pour notre étude sont :
* **LSTAT** : Pourcentage de la population de statut socio-économique inférieur.
* **RM** : Nombre moyen de pièces par logement.
* **PTRATIO** : Ratio élèves-enseignants par ville.
* **MEDV** : Valeur médiane des logements occupés par leurs propriétaires (variable cible).

## Méthodologie

Le projet suit une démarche de Data Science structurée :
1. **Exploration & Analyse Descriptive (EDA)** : Nettoyage des données, calcul des intervalles de confiance à 95 % et tests de normalité (Shapiro-Wilk) pour comprendre la distribution des variables.
2. **Prétraitement** : Standardisation des données (`StandardScaler`) pour assurer une convergence optimale des modèles.
3. **Régression Linéaire Classique** : Modélisation basée sur les variables clés identifiées lors de l'EDA pour garantir une interprétabilité maximale.
4. **Réduction de dimensionnalité (PCR)** : Application de l'Analyse en Composantes Principales (ACP) combinée à une régression pour traiter la multicolinéarité et améliorer la robustesse.
5. **Évaluation & Validation** : Comparaison des modèles via les métriques $R^2$ et RMSE (Root Mean Square Error) sur des jeux d'entraînement et de test distincts.

## Installation & Exécution
Pour exécuter ce notebook en local :

1. Clonez ce dépôt :
```bash
git clone https://github.com/HassanCharaf25/prediction-prix-boston
```
2. Installer les dépendances nécessaires :
```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn statsmodels
```
3. Ouvrir le fichier `boston_housing.ipynb` avec un editeur de texte :
```bash
code boston_housing.ipynb
```
## Auteur :
* **CHARAF Hassan**
