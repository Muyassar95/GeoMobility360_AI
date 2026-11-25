# Journal de progression — GeoMobility360 AI

---

## J05 — Consolidation démographique et SQL

**Objectifs :** consolider POP1/POP2, découvrir DuckDB et préparer les indicateurs communaux.

**Travaux vérifiés :**
- Premières requêtes SQL avec `SELECT`, `WHERE`, `GROUP BY`.
- Débogage de l'affichage des cartes Plotly : WebGL réactivé dans Edge.

**Tâches validées :** complétude des indicateurs, jointures et sauvegardes finales.

**Compétences :** SQL, diagnostic technique, cartographie interactive.


---

## J06 — Exploration statistique et analyse territoriale

**Objectif :** explorer les disparités démographiques entre les communes franciliennes.

**Travaux réalisés :**
- Statistiques descriptives et quantiles.
- Détection des communes atypiques.
- Corrélations et visualisations Plotly.
- Analyses SQL et cartes territoriales.

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
- Nombre de communes contrôlées : 1266.
- Nombre d'anomalies détectées : 0.
- Résultats des jointures POP1/POP2 : Validé.
- Typologie et carte interactive : Oui.

### Tâches validées
- Cohérence finale des données et des dénominateurs.
- Compatibilité des millésimes géographiques.
- Sauvegarde et relecture des fichiers produits.

### Preuves
- `notebooks/J07_validation_territoriale.ipynb`
- `data/processed/J07_controles_qualite.csv`
- `reports/figures/J07_typologie_demographique.html`

---

## J08 — Activité, emploi et chômage par âge et sexe

**Projet :** GeoMobility360 AI  
**Date :** 22 novembre 2026  
**Thématique :** Socioeconomic Intelligence, Data Engineering & SQL Analytics

### Travaux

- Exploration des données INSEE ACT1 — Recensement 2023 sur l'activité, l'emploi et le chômage.
- Extraction des observations communales par sexe, âge détaillé et statut d'activité avec DuckDB/SQL.
- Préparation des effectifs d'actifs, de chômeurs et de personnes en emploi.
- Identification de doublons lors de la transformation avec `pivot()`.
- Diagnostic des clés statistiques et des modalités géographiques pour éviter les doubles comptes.
- Préparation des regroupements d'âge : 15–24, 25–39, 40–54 et 55–64 ans.
- Préparation des indicateurs communaux et de leur intégration géographique.

### Résultats vérifiés

- Lecture et interrogation des données ACT1 avec DuckDB : réalisées.
- Extraction des observations par âge, sexe et statut : réalisée.
- Doublons empêchant le pivot : identifiés.
- Nombre de communes exploitables : 1266.
- Cohérence des effectifs actifs = emplois + chômeurs : Oui.
- Cartes interactives des taux d'activité, d'emploi et de chômage : Oui.

### Tâches validées

- Résolution des doublons ACT1 sans perte ni double comptage.
- Complétude des âges et des catégories d'activité.
- Calcul et validation des trois taux avec les dénominateurs appropriés.
- Harmonisation des codes INSEE, notamment Paris.
- Jointure ACT1/POP1 et intégration dans la base géodémographique.
- Sauvegarde et relecture des fichiers Parquet et GeoPackage.

### Preuves

- `notebooks/J08_activite_emploi_chomage.ipynb`
- `sql/J08_extraction_ACT1.sql`
- `data/processed/J08_emploi_tranches_age_2023.parquet`
- `data/processed/J08_indicateurs_emploi_communaux_2023.parquet`
- `reports/figures/J08_taux_chomage_15_64.html`

---

## J09 — Analyse territoriale de l'activité, de l'emploi et du chômage

**Projet :** GeoMobility360 AI  
**Date :** 23 novembre 2026  
**Thématique :** Socioeconomic Intelligence, SQL & GeoAnalytics

### Travaux

- Préparation des données ACT1 par commune, sexe et âge.
- Segmentation en trois classes : 15–24, 25–54 et 55–64 ans.
- Construction de neuf indicateurs : taux d'activité, d'emploi et de chômage par classe d'âge.
- Comparaison des disparités femmes-hommes.
- Analyses territoriales avec DuckDB et SQL.
- Statistiques descriptives et visualisations interactives Plotly.
- Préparation des cartes choroplèthes par âge et indicateur.

### Résultats vérifiés

- Communes étudiées : 1266
- Contrôles des doublons et des effectifs : Oui
- Couverture des trois groupes d'âge : Oui
- Écarts femmes-hommes : Oui
- Principales disparités territoriales : Oui
- Cartes produites : Oui

### Tâches validées

- Cohérence ACT1/POP1 et traitement de Paris.
- Comparaison des taux avec les indicateurs INSEE publiés.
- Prudence concernant les faibles effectifs.
- Sauvegarde et relecture des fichiers produits.

### Preuves

- `notebooks/J09_analyse_emploi_age_sexe.ipynb`
- `data/processed/J09_emploi_sexe_age_2023.parquet`
- `data/processed/J09_neuf_indicateurs_emploi_2023.parquet`
- `reports/figures/J09_comparaison_taux_age.html`
- `reports/figures/J09_carte_chomage_jeunes.html`

