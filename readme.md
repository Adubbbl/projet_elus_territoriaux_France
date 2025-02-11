# Analyse et Fusion de Jeux de Données Open Data

## Description du Projet

Ce projet vise à fusionner et analyser plusieurs jeux de données, portant sur les élus territoriaux en France, issus de la plateforme [data.gouv.fr](https://www.data.gouv.fr). L'objectif est d'identifier les colonnes communes, explorer et évaluer la qualité des données, identifier des axes d'analyses et les mettre en place.

## Données Utilisées

Les fichiers analysés proviennent des URLs suivantes :

- [Élus conseillers d'arrondissements](https://www.data.gouv.fr/fr/datasets/r/3b6b2281-b9d9-4959-ae9d-c2c166dff118)
- [Élus conseillers municipaux](https://www.data.gouv.fr/fr/datasets/r/d5f400de-ae3f-4966-8cb6-a85c70c6c24a)
- [Élus conseillers communautaires](https://www.data.gouv.fr/fr/datasets/r/41d95d7d-b172-4636-ac44-32656367cdc7)
- [Élus conseillers départementaux](https://www.data.gouv.fr/fr/datasets/r/601ef073-d986-4582-8e1a-ed14dc857fba)
- [Élus conseillers régionaux](https://www.data.gouv.fr/fr/datasets/r/430e13f9-834b-4411-a1a8-da0b4b6e715c)

## Installation et Prérequis

### Environnement requis

- Python 3.x
- Jupyter Notebook
- Bibliothèques Python :
  - pandas
  - numpy
  - requests

### Installation

Clonez ce projet et installez les dépendances :

```bash
git clone https://github.com/Adubbbl/projet_elus_territoriaux_France.git
cd projet_elus_territoriaux_France
pip install -r requirements.txt
```

## Structure du Projet

- `main.ipynb` : Contient l'ensemble des analyses et transformations appliquées aux données.
- `data/` : Dossier contenant les fichiers de données.
- `README.md` : Documentation du projet.

## Workflow du Projet

1. **Lecture des fichiers**
   - Chargement des jeux de données dans des DataFrames pandas.
   - Association de noms lisibles aux URLs.
2. **Identification des colonnes communes**
   - Analyse de la fréquence des colonnes présentes dans les différents fichiers.
   - Production d'un DataFrame listant chaque colonne et son occurrence.
3. **Fusion des fichiers**
   - Regroupement des données avec `pandas.concat`.
   - Harmonisation des structures de données.
4. **Évaluation de la qualité des données**
   - Calcul du nombre de lignes contenant des valeurs manquantes (NaN).
5. **Pistes d'analyse**
   - Identification des colonnes à conserver ou à supprimer.
   - Proposition de méthodes pour traiter les valeurs manquantes.
   - Idées d'axes d'analyses exploitables avec les données disponibles.
6. **Analyse exploratoire des colonnes**
    - Visualisation univariées, bivariées et multivariées des colonnes
7. **Mise en place des axes d'analyses**
   - Création d'un tableau de bord avec shinny

## Résultats Attendus

- Un jeu de données unifié et nettoyé.
- Un rapport d'analyse des colonnes disponibles.
- Une stratégie de nettoyage et de traitement des valeurs manquantes.
- Des axes d'analyses pour exploiter au mieux les données fusionnées.

## Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

## Auteur

[Aduni LAWANI](https://adunilawani.com/) - Data analyst

