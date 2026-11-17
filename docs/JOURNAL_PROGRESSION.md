# Journal de progression — GeoMobility360 AI

---

## J05 — Consolidation démographique et SQL

**Objectifs :** consolider POP1/POP2, découvrir DuckDB et préparer les indicateurs communaux.

**Travaux vérifiés :**
- Premières requêtes SQL avec `SELECT`, `WHERE`, `GROUP BY`.
- Débogage de l'affichage des cartes Plotly : WebGL réactivé dans Edge.

**À vérifier :** complétude des indicateurs, jointures et sauvegardes finales.

**Compétences :** SQL, diagnostic technique, cartographie interactive.


---

## J06 — Exploration statistique et analyse territoriale

**Objectif :** explorer les disparités démographiques entre les communes franciliennes.

**Travaux réalisés :**
- À compléter : statistiques descriptives et quantiles.
- À compléter : détection des communes atypiques.
- À compléter : corrélations et visualisations Plotly.
- À compléter : analyses SQL et cartes territoriales.

**Résultat principal :** à renseigner avec une observation chiffrée.

**Difficulté rencontrée / solution :** à compléter.

**Compétences travaillées :** Pandas, statistiques descriptives, SQL, GeoPandas et Plotly.

---

## J07 — Consolidation et validation territoriale

**Projet :** GeoMobility360 AI  
**Date :** 17 novembre 2026  
**Thématique :** Data Quality, SQL & GeoAnalytics

### Travaux
- Audit des données communales POP1/POP2 : doublons, valeurs manquantes et cohérence des effectifs.
- Consolidation des indicateurs de vieillissement et de dépendance démographique.
- Analyses comparatives entre communes et départements avec DuckDB/SQL.
- Construction d'une typologie démographique fondée sur les quartiles.
- Préparation d'une carte interactive Plotly et des exports Parquet/GeoPackage.

### Résultats vérifiés
- Nombre de communes contrôlées : à compléter.
- Nombre d'anomalies détectées : à compléter.
- Résultats des jointures POP1/POP2 : à compléter.
- Typologie et carte interactive : à confirmer après exécution.

### À valider
- Cohérence finale des données et des dénominateurs.
- Compatibilité des millésimes géographiques.
- Sauvegarde et relecture des fichiers produits.

### Preuves
- `notebooks/J07_validation_territoriale.ipynb`
- `data/processed/J07_controles_qualite.csv`
- `reports/figures/J07_typologie_demographique.html`
