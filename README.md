# Brazilian-E-Commerce-by-Olist
📦 # Projet Data Warehouse - Olist (E-Commerce Brésilien)

🛍️ Contexte
Ce projet repose sur un jeu de données réel et anonymisé fourni par Olist, une plateforme e-commerce brésilienne. Il contient plus de 100 000 commandes réalisées entre 2016 et 2018 sur plusieurs marketplaces au Brésil. Ces données reflètent des processus réels de vente en ligne, depuis la commande jusqu’à la livraison, en passant par les paiements, les avis clients, les retours et la logistique.

📚 Objectif du projet
Créer un Data Warehouse complet en SQL Server (ou autre SGBD) à partir de données brutes, en appliquant les concepts suivants :

Modèle bronze / silver / gold pour l’architecture des données

Nettoyage et enrichissement des données (data cleansing & wrangling)

Modélisation dimensionnelle (star schema)

Création de vues métiers pour les analyses (vente, logistique, satisfaction, etc.)

🧾 Description du dataset
Le dataset est composé de plusieurs fichiers représentant les différentes entités du processus e-commerce :

Fichier	Description
olist_orders_dataset.csv	Commandes passées (statut, dates, ID client)
olist_order_items_dataset.csv	Détails de chaque article commandé
olist_products_dataset.csv	Produits (nom, catégorie, poids, etc.)
olist_customers_dataset.csv	Clients (localisation, ID anonymisé)
olist_order_reviews_dataset.csv	Avis et notes clients
olist_sellers_dataset.csv	Vendeurs (ID et localisation)
olist_order_payments_dataset.csv	Détail des paiements (montant, type)
product_category_name_translation.csv	Traduction des catégories produits
geolocation_dataset.csv	Coordonnées géographiques des codes postaux brésiliens

🔍 Analyse: 
Nettoyage de données (data cleansing) : gestion des données manquantes, incohérentes, doublons, etc.

Qualité produit & satisfaction client : quels produits ou catégories génèrent le plus d’insatisfaction ?

Performance logistique : délais réels vs prévus, retards, zones géographiques problématiques

Prévision de ventes : création de variables temporelles et prévision par série temporelle

Segmentation client : analyse RFM ou clustering client

Analyse marketing (si vous ajoutez le funnel marketing)

🧰 Outils recommandés
SQL Server 
Power BI 

🌍 Source des données
Les données sont disponibles gratuitement sur Kaggle.
