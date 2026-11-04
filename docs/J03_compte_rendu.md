# J03 — Population et densité démographique

**Projet :** GeoMobility360 AI  
**Date :** 4 novembre 2026  
**Thématique :** Territorial Intelligence & Geospatial Data Engineering

## 1. Objectif

Intégrer les populations municipales INSEE aux contours communaux d'Île-de-France, construire un indicateur de densité et réaliser une cartographie interactive.

## 2. Données utilisées

- INSEE : populations de référence 2023, géographie au 1er janvier 2025.
- Contours communaux : données géographiques du J1/J2.
- Clé de jointure : code INSEE communal.

## 3. Méthodologie

- Acquisition et exploration du CSV INSEE.
- Filtrage des communes franciliennes.
- Normalisation des codes INSEE.
- Jointure géographique avec Pandas.
- Contrôles qualité.
- Calcul de la densité en habitants/km².
- Visualisation interactive avec Plotly.

## 4. Résultats

- Communes géographiques : 1266
- Communes associées : 0
- Jointures non résolues : 0
- Population municipale totale : 12 463 067 habitants (Région Ile-de-France)
- Commune la plus peuplée : Paris (2 103 778 habitants)
- Commune la plus dense : Levallois-Perret (28 167 hab/km²)

## 5. Difficultés rencontrées

- J'ai rencontré des difficultés lors de l'agrégation des populations des 20 arrondissements de Paris. Les données INSEE étant présentées à l'échelle des arrondissements, j'ai dû regrouper leurs populations sous le code communal 75056 pour assurer leur compatibilité avec les données géographiques.
- Cette difficulté m'a permis de mieux comprendre l'importance de l'harmonisation des échelles géographiques avant une jointure.

## 6. Interprétation

- L'analyse géographique suggère que les communes présentant les densités de population les plus élevées se concentrent notamment à Paris et en petite couronne.
- Cette répartition peut s'expliquer par une urbanisation plus dense et une concentration importante des logements et des habitants.
- Toutefois, la densité dépend à la fois du nombre d'habitants et de la superficie communale. Une commune très peuplée n'est donc pas nécessairement la plus dense.

## 7. Compétences développées

- Manipulation de données INSEE.
- Fusion de DataFrames.
- Nettoyage des identifiants.
- Calcul d'indicateurs territoriaux.
- Contrôles statistiques.
- Cartographie choroplèthe interactive.

## 8. Prochaine étape — J04

Analyse statistique des populations et des densités : distributions, valeurs extrêmes, comparaisons territoriales et visualisations avancées.
