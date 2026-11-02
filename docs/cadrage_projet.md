# Cadrage du projet GeoMobility360 AI

**Nom :** GeoMobility360 AI — Geospatial Intelligence, Smart Mobility & Urban Analytics

**Date de lancement :** 02 novembre 2026  
**Durée du MVP :** 60 jours (30 à 45 minutes/jour)  
**Périmètre initial :** Île-de-France — communes et IRIS

## 1. Présentation et objectifs

GeoMobility360 AI est un projet de Data Science et d'intelligence géospatiale visant à analyser les territoires, les mobilités, les dynamiques socio-économiques et les opportunités d'implantation commerciale.

**Deux objectifs :**
- **Court terme :** développer un portfolio Data Scientist professionnel sur GitHub et LinkedIn.
- **Long terme :** créer une plateforme SaaS B2B/B2G destinée aux entreprises, collectivités et acteurs de la mobilité, extensible à l'international.

## 2. Domaines d'analyse

- **Territorial Intelligence :** population, revenus, emploi, chômage, logement et inégalités.
- **Smart Mobility :** réseaux de transport, gares, arrêts et accessibilité.
- **GeoMarketing :** équipements, commerces, concurrence et potentiel d'implantation.
- **Smart Cities :** mobilité durable, accès aux services et aménagement territorial.

## 3. Données prioritaires

| Source | Données |
|---|---|
| INSEE | Population, emploi, revenus, pauvreté |
| IGN | Contours communaux et IRIS |
| INSEE BPE | Commerces, équipements et services |
| Île-de-France Mobilités | Arrêts, gares et réseaux de transport |
| OpenStreetMap | Réseaux et données géographiques complémentaires |

## 4. Technologies

**Data :** Python, Pandas, NumPy, SQL, DuckDB, Parquet.

**SIG :** GeoPandas, Shapely, QGIS, Folium.

**Machine Learning :** Scikit-learn, KMeans, évaluation des clusters.

**Visualisation :** Streamlit et Power BI.

**Extensions futures :** PostgreSQL/PostGIS, PyTorch, Deep Learning, Big Data et Cloud.

**Contraintes :** ordinateur Windows, 16 Go de RAM, calcul principalement sur CPU.

## 5. Méthodologie et MVP

Chaîne de traitement :

Acquisition → Nettoyage → Jointures géographiques → Analyse statistique → Machine Learning → Cartographie → Dashboard.

**Plan des 60 jours :**

- **J0–J15 :** cadrage, collecte, nettoyage et préparation des données.
- **J16–J25 :** analyses statistiques et cartographies territoriales.
- **J26–J35 :** clustering KMeans et segmentation des communes.
- **J36–J45 :** analyse de l'accessibilité et scoring géomarketing.
- **J46–J55 :** développement du dashboard Streamlit.
- **J56–J60 :** documentation, GitHub et présentation professionnelle.

## 6. Livrables attendus

1. Dépôt GitHub structuré et documenté.
2. Notebooks Python et requêtes SQL reproductibles.
3. Base territoriale communale et prototype IRIS.
4. Cartes et indicateurs socio-économiques.
5. Modèle de clustering évalué.
6. Score d'implantation transparent.
7. Dashboard interactif Streamlit.

## 7. Vision internationale

Après validation du MVP en Île-de-France, GeoMobility360 AI pourra être étendu aux métropoles européennes, puis aux mégalopoles internationales.

L'architecture devra prendre en charge les différentes unités géographiques, les systèmes de coordonnées, les millésimes et les définitions statistiques propres à chaque pays.

**Finalité :** développer progressivement une plateforme internationale d'intelligence territoriale, de mobilité et de géomarketing destinée aux professionnels.

## 8. Prochaine étape — J01

Récupérer les contours officiels des communes d'Île-de-France, les importer dans Jupyter avec GeoPandas, vérifier les codes géographiques et réaliser une première carte.
