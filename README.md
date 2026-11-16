# 📊 Impact des IDE Industriels sur les Métiers Mondiaux du Maroc (2014–2025)

## 🎯 Objectif du Projet
Cette étude analyse l'effet d'entraînement des **Investissements Directs Étrangers (IDE) manufacturiers** sur la performance à l'export des **Métiers Mondiaux du Maroc** (Automobile et Aéronautique) entre **2014 et 2025**, tout en évaluant l'évolution de la dépendance aux importations d'intrants (biens d'équipement et demi-produits).

---

## 📂 Source & Périmètre des Données
- **Source officielle :** Office des Changes (Maroc) — Statistiques des Échanges Extérieurs et des IDE par secteurs (Nomenclature NMA).
- **Période :** 2014 – 2025 (données annuelles harmonisées en **Millions de Dirhams - MDH**).
- **Variables analysées :**
  - `IDE_Recettes_Ind` & `IDE_Nets_Ind` : Flux d'IDE dans les industries manufacturières.
  - `Exp_Automobile` & `Exp_Aeronautique` : Exportations FAB des secteurs automobile et aéronautique.
  - `Imp_Equipement` & `Imp_DemiProduits` : Importations CAF d'intrants industriels.

---

## 🛠️ Stack Technique & Méthodologie
1. **ETL & Data Cleaning (Python - `pandas`) :** Extraction automatisée, harmonisation des unités (MAD → MDH) et structuration de la base finale (`Data_Final.xlsx`).
2. **Modélisation Économétrique (Python - `statsmodels`) :** Analyse des décalages temporels (*Lag Analysis*), corrélations croisées et estimation de l'élasticité IDE → Exportations.
3. **Business Intelligence (Power BI) :** Conception d'un tableau de bord interactif suivant le taux de couverture sectoriel et la dynamique commerciale.

---

## 📁 Architecture du Repository
```text
├── data_clean/       # Base de données nettoyée et harmonisée (Data_Final.xlsx)
├── scripts/          # Scripts Python (ETL, nettoyage et tests économétriques)
├── powerbi/          # Fichier source du Dashboard interactif (.pbix) et export PDF
└── README.md         # Documentation du projet
