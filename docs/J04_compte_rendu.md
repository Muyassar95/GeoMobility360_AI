# J04 — Démographie avancée : POP1 et POP2

**Projet :** GeoMobility360 AI  
**Date :** 7 novembre 2026  
**Thématique :** Territorial Intelligence & Demographic Data Engineering

## 1. Objectif

Enrichir la base démographique des communes d'Île-de-France avec les populations légales, les répartitions par sexe et âge, ainsi que les catégories de résidence.

## 2. Données utilisées

- **INSEE — Populations de référence 2023 :** population municipale (PMUN), comptée à part (PCAP) et totale (PTOT).
- **INSEE — POP1 :** population selon le sexe et l'âge détaillé (0 à 100 ans ou plus).
- **INSEE — POP2 :** population selon le sexe, les classes d'âge et les catégories de résidence.
- **GeoPandas :** contours communaux et superficies issus des journées précédentes.

## 3. Méthodologie

- Conservation des trois populations légales et vérification de leur cohérence.
- Nettoyage et harmonisation des codes INSEE.
- Transformation de POP1 et POP2 avec `melt()`.
- Agrégation des effectifs avec `groupby()`.
- Calcul des proportions par sexe et catégorie de résidence.
- Regroupement des âges pour faciliter les comparaisons territoriales.
- Restructuration des catégories avec `pivot()`.
- Création d'une pyramide des âges interactive avec Plotly.
- Préparation des données pour les jointures géographiques.

## 4. Résultats et contrôles qualité

- **Communes étudiées :** 1266
- **Âges POP1 :** 0 à 100 ans ou plus, par sexe.
- **Groupes d'âge POP2 :** 0–14, 15–24, 25–54, 55–64 et 65 ans ou plus.
- **Catégories de résidence :** catégories détaillées conservées.
- **Doublons :** Non
- **Valeurs manquantes :** Non
- **Cohérence PMUN + PCAP = PTOT :** Oui
- **Jointures géographiques non résolues :** Non

## 5. Difficultés rencontrées

La principale difficulté a été de traiter des données démographiques présentées sous des formats complexes, notamment les nombreuses colonnes d'âge et de sexe de POP1 et les catégories de résidence de POP2.

L'utilisation de `melt()`, `groupby()` et `pivot()` a permis de mieux structurer les données. Une attention particulière reste nécessaire pour éviter les doubles comptes et harmoniser les unités géographiques, notamment les arrondissements de Paris.

## 6. Interprétation des résultats

Les données POP1 permettent d'étudier la structure démographique des communes selon le sexe et l'âge. La pyramide des âges facilite la visualisation des différences entre générations.

Les données POP2 apportent une dimension supplémentaire en distinguant les catégories de résidence. Elles permettront de comparer les profils résidentiels et démographiques des territoires franciliens.

Ces analyses doivent tenir compte des différences de millésimes géographiques et des méthodes statistiques de l'INSEE.

## 7. Compétences développées

- Traitement de données INSEE multidimensionnelles.
- Manipulation avancée de DataFrames avec Pandas.
- Agrégation et transformation de données.
- Construction d'indicateurs démographiques.
- Visualisation interactive avec Plotly.
- Préparation de bases réutilisables pour les analyses spatiales.

## 8. Prochaine étape — J05

Approfondir l'analyse territoriale des données POP1 et POP2, vérifier les jointures communales et produire des comparaisons interactives entre communes.

Préparer progressivement les indicateurs démographiques destinés aux futures analyses de mobilité, de géomarketing et de Machine Learning.
