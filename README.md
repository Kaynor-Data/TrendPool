# TrendPool — Projet d'analyse des données de vente
Sales data analysis project: trends, top-selling products and revenue metrics for business decision-making. Python, Pandas, Power BI.

## 📌 Aperçu du projet

**TrendPool** est un projet d'analyse de données de vente dont l'objectif est d'identifier les **tendances**, les **produits les plus vendus** et les **métriques de revenus clés** afin d'éclairer la prise de décision business. Ce projet a été réalisé dans le cadre du programme proposé par **MeriSKILL**, pour développer des compétences concrètes sur un cas réel d'analyse de données.

## ❓ Problème business & questions clés

- **Problème** : Comment les ventes évoluent-elles dans le temps, et où se trouvent les opportunités d'optimisation des revenus ?
- **Questions** :
  1. Quel est le chiffre d'affaires total et son évolution mensuelle ?
  2. Quels sont les produits qui génèrent le plus de revenus ?
  3. Quelles sont les villes / catégories les plus performantes ?
  4. Quels créneaux horaires concentrent le plus de ventes ?

## 📊 Données

- **Source** : Dataset fourni par MeriSKILL (simulation de ventes d'un détaillant en électronique).
- **Taille** : ~186 000 lignes.
- **Colonnes clés** : `Order ID`, `Product`, `Quantity Ordered`, `Price Each`, `Order Date`, `Purchase Address`.

> ⚠️ Les données brutes ne sont pas versionnées dans ce dépôt (voir `.gitignore`). Un échantillon est disponible dans `data/sample/`.

## 🛠️ Outils & technologies

- **Langage** : Python 3.x
- **Librairies** : Pandas, NumPy, Matplotlib, Seaborn
- **Visualisation** : Power BI (dashboard interactif)
- **Versioning** : Git / GitHub

## 🔍 Méthodologie

1. **Nettoyage & préparation** : suppression des doublons, gestion des valeurs manquantes, conversion des dates, extraction du mois, de l'heure et de la ville.
2. **Analyse exploratoire (EDA)** : calcul des KPIs (CA total, panier moyen, quantité vendue), analyse des tendances temporelles et géographiques.
3. **Visualisation** : création d'un tableau de bord interactif (Power BI) pour explorer les performances par produit, ville et période.
4. **Insights & recommandations** : synthèse des résultats et propositions d'actions concrètes.

## 💡 Résultats & insights clés

- **Tendance** : pic de ventes en **décembre**, avec une croissance de **X %** par rapport au trimestre précédent.
- **Top produit** : le produit **[Nom]** représente **Y %** du chiffre d'affaires total.
- **Géographie** : la ville de **[Ville]** concentre **Z %** des ventes.
- **Recommandation** : renforcer les stocks de **[Catégorie]** avant la période de pointe et lancer une campagne ciblée sur **[Ville]**.

_(À compléter au fur et à mesure de l'analyse.)_

## 🚀 Comment exécuter ce projet

```bash
# 1. Cloner le dépôt
git clone https://github.com/<ton-username>/TrendPool.git
cd TrendPool

# 2. Créer un environnement virtuel
python -m venv .venv
source .venv/bin/activate      # Linux / macOS
.venv\Scripts\activate         # Windows

# 3. Installer les dépendances
pip install -r requirements.txt

# 4. Placer le fichier de données original dans data/raw/

# 5. Lancer les notebooks
jupyter notebook
```

## 📁 Structure du projet

```text
TrendPool/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   ├── raw/              # données brutes (non versionnées)
│   └── processed/        # données nettoyées
├── notebooks/
│   └── 01_exploration_ventes.ipynb
├── src/
│   ├── data_preparation.py
│   └── analysis.py
├── dashboards/
│   └── trendpool_dashboard.pbix
├── reports/
│   └── figures/
└── sql/
    └── analyses_cles.sql
```

## 👤 Auteur

**[Ton Nom]** — [LinkedIn](https://linkedin.com/in/ton-profil) — [Portfolio](https://ton-portfolio.com)

## 📄 Licence

Ce projet est sous licence **MIT**. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
