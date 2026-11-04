
# J02 — Qualité et analyse géographique

**Projet :** GeoMobility360 AI  
**Date :** 3 novembre 2026  
**Thématique :** Territorial Intelligence & Geospatial Data Engineering

## 1. Objectif
Contrôler les données communales et calculer les superficies.

## 2. Données
- Source : GeoAPI
- Format : GEOJSON
- Projection initiale : 4326
- Projection finale : 2154 (Lambert-93)

## 3. Résultats
- Nombre de communes : 1266
- Doublons : 0
- Valeurs manquantes : 0
- Géométries invalides : 0
- Superficie minimale : 0,09 km²
- Superficie maximale : 172,28 km²

## 4. Travaux réalisés
- Contrôle qualité : x
- Reprojection : x
- Calcul des superficies : x
- Cartographie : x

## 5. Difficultés rencontrées
- Distinction entre les valeurs manquantes (isna()) et les géométries invalides (is_valid).

- Compréhension des opérations booléennes (~, &) pour contrôler la qualité géographique.

- Sélection simultanée des noms des communes et de leurs superficies avec nlargest().

- Compréhension de la reprojection géographique et du calcul des superficies en km².

## 6. Interprétation
- Les superficies communales présentent des différences importantes entre les territoires franciliens.

- La reprojection en Lambert-93 (EPSG:2154) permet d'effectuer des calculs de superficies en unités métriques.

- Les contrôles qualité permettent d'identifier les anomalies susceptibles de fausser les analyses géospatiales.

- La superficie seule ne permet pas d'évaluer la densité démographique, l'accessibilité ou le potentiel économique d'un territoire.

## 7. Compétences acquises
- Manipulation de GeoDataFrames avec GeoPandas.

- Contrôle des doublons, des valeurs manquantes et des géométries invalides.

- Utilisation des systèmes de coordonnées EPSG:4326 et EPSG:2154.

- Calcul des superficies communales avec .area.

- Classement des communes avec .nlargest() et .sort_values().

- Initiation à la cartographie choroplèthe avec Matplotlib et GeoPandas.
