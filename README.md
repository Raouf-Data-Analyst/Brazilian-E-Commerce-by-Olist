# 🛒 Projet Data Warehouse – E-commerce Brésilien (Olist)

Bienvenue dans ce projet complet de **Data Warehouse et Analytique** basé sur un jeu de données réel issu de la marketplace brésilienne **Olist**. Ce projet met en pratique les meilleures pratiques en ingénierie des données, nettoyage, modélisation en étoile et analyse SQL, dans un cadre inspiré du monde professionnel.

---

## 🧱 Architecture des données – Medallion Architecture

Ce projet utilise l'architecture en couches **Bronze**, **Silver** et **Gold** pour construire un data warehouse moderne :

1. **Bronze Layer** : Ingestion brute des fichiers CSV (données ERP et CRM anonymisées).
2. **Silver Layer** : Nettoyage des données, standardisation, transformation (jointures, filtrages, gestion des anomalies).
3. **Gold Layer** : Modélisation analytique en schéma en étoile avec tables de faits et dimensions prêtes pour l’analyse.

---

## 📦 Données utilisées

Les données proviennent du dataset [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).  
Ce jeu de données contient environ **100 000 commandes** passées entre 2016 et 2018 sur différentes marketplaces au Brésil.

### Tables principales :
- `customers` : informations clients (ID, ville, état)
- `orders` : statut, date de commande, livraison
- `order_items` : produits, vendeurs, prix, frais de port
- `products` : catégorie, nom, poids, dimensions
- `sellers` : localisation des vendeurs
- `order_reviews` : notes et commentaires clients
- `geolocation` : code postal → latitude/longitude

> 💡 Les noms des vendeurs et entreprises ont été remplacés par des noms issus de **Game of Thrones** pour anonymiser les données.

---

## 🎯 Objectifs du projet

- **Créer un Data Warehouse complet** à partir de données brutes
- **Nettoyer et transformer** les données multi-sources
- **Modéliser un schéma en étoile** pour les analyses métier
- **Réaliser des requêtes analytiques** : comportement client, performance produit, retards de livraison, etc.
- **Détecter les anomalies** dans les livraisons et retours

---

## 🧰 Outils & Technologies

- **SQL Server** : Base de données relationnelle
- **T-SQL** : Scripts ETL et transformations
- **Draw.io** : Documentation d'architecture
- **Power BI / Excel (optionnel)** : Visualisation des KPI
```
---

## 📁 Structure du répertoire

olist-data-warehouse/  
│
├── datasets/ # Données brutes issues de Olist
│
├── docs/ # Diagrammes d’architecture
│ ├── data_flow.drawio # Diagramme du flux de données
│ ├── data_model_star.drawio # Schéma en étoile final
│ ├── data_catalog.md # Dictionnaire des tables et colonnes
│
├── scripts/
│ ├── bronze/ # Scripts d’importation brute
│ ├── silver/ # Scripts de nettoyage et jointure
│ ├── gold/ # Scripts de création de tables de faits/dimensions
│
├── README.md # Ce fichier
├── .gitignore # Fichiers ignorés par Git
├── LICENSE # Licence du projet
└── requirements.txt # Dépendances éventuelles
```
---

## 🔍 Analyses réalisées

- 🌎 Répartition géographique des clients et vendeurs
- 📦 Produits les plus vendus par catégorie
- 🕒 Délais moyens de livraison vs prévision
- 📈 Évolution des ventes mensuelles
- ⭐ Notes moyennes par catégorie produit

---

## 🌟 À propos de moi

Salut ! Je suis **Abderaouf Larouci**, passionné de Data et spécialisé dans la transformation de données brutes en insights exploitables. Ce projet reflète ma volonté de reproduire des situations réelles rencontrées en entreprise, en appliquant des standards professionnels.

---

## 📌 Inspirations

- Kaggle Dataset: [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- Projet inspiré par la formation "DataWithBaraa"


