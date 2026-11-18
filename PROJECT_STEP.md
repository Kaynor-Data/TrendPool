# PROJECT_STEPS — TrendPool

> Feuille de route du projet d'analyse des données de vente **TrendPool**.
> Ce document suit la méthodologie classique : **Problème Business → Données → Analyse → Visualisation → Recommandations**.

---

## 🎯 Étape 1 — Poser le cadre (Le "Pourquoi")

- [ ] Définir le problème business principal
- [ ] Lister les 4-5 questions clés auxquelles l'analyse doit répondre
- [ ] Identifier les KPIs à calculer (CA total, panier moyen, quantité vendue…)
- [ ] Rédiger une courte "problem statement" dans le README

**Livrable** : une section "Problème business & questions clés" dans le README.

---

## 🧹 Étape 2 — Préparer les données (Le "Comment")

- [ ] Télécharger / placer le dataset dans `data/raw/`
- [ ] Inspecter les colonnes, types et dimensions (`df.info()`, `df.describe()`)
- [ ] Vérifier et supprimer les doublons
- [ ] Gérer les valeurs manquantes
- [ ] Convertir les types (`Order Date` → datetime, `Price Each` → float…)
- [ ] Créer des colonnes dérivées : `Month`, `Year`, `Hour`, `City`, `Revenue = Quantity × Price`
- [ ] Sauvegarder le dataset nettoyé dans `data/processed/`

**Livrable** : `notebooks/01_exploration_ventes.ipynb` + `src/data_preparation.py`

---

## 📊 Étape 3 — Analyser (Le "Quoi")

- [ ] Calculer les KPIs globaux (CA total, quantité totale, panier moyen)
- [ ] Analyser l'évolution mensuelle du CA
- [ ] Identifier les Top 10 produits par revenu et par quantité
- [ ] Analyser la répartition par ville / région
- [ ] Analyser les créneaux horaires de vente
- [ ] Croiser produit × mois pour repérer les produits saisonniers

**Livrable** : section "Analyse" du notebook + premières figures dans `reports/figures/`

---

## 📈 Étape 4 — Visualiser

- [ ] Créer les graphiques clés (courbe temporelle, bar chart top produits, pie chart catégories)
- [ ] Construire le dashboard Power BI (`dashboards/trendpool_dashboard.pbix`)
  - [ ] Carte KPI : CA total
  - [ ] Graphique ligne : évolution mensuelle
  - [ ] Bar chart : Top produits
  - [ ] Slicers : ville / mois / catégorie
- [ ] Exporter une capture du dashboard pour le README

**Livrable** : dashboard Power BI + `reports/figures/dashboard_preview.png`

---

## 💡 Étape 5 — Insights & Recommandations (Le "Et alors ?")

- [ ] Rédiger 3-5 insights clés (ex : "Le produit X = 40% du CA mais en baisse depuis 3 mois")
- [ ] Formuler 2-3 recommandations concrètes et actionnables
- [ ] Ajouter ces insights dans le README
- [ ] (Optionnel) Rédiger un mini rapport PDF dans `reports/`

**Livrable** : sections "Résultats & insights clés" et "Recommandations" du README.

---

## 🚀 Étape 6 — Finalisation du dépôt

- [ ] Rédiger le README complet
- [ ] Ajouter `requirements.txt`
- [ ] Vérifier le `.gitignore` (données brutes exclues)
- [ ] Nettoyer les notebooks (`Kernel > Restart & Clear Output` avant commit)
- [ ] Ajouter les topics GitHub (`data-analysis`, `sales-analytics`, `python`, `power-bi`…)
- [ ] Publier sur LinkedIn avec un lien vers le repo

---

## 📅 Journal de progression

| Date | Étape | Statut | Notes |
|------|-------|--------|-------|
| AAAA-MM-JJ | Cadrage | ✅ | Problème et questions définis |
| AAAA-MM-JJ | Nettoyage | 🟡 | Doublons supprimés, nulls à traiter |
|  |  |  |  |

**Légende** : ✅ terminé · 🟡 en cours · ⬜ à faire
