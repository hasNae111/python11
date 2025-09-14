Challenge 1 : Création d’une Base de Données
Objectif : Apprendre à créer une base de données et préparer sa structure.
Travail à faire :
Créez une base de données nommée store_db.
Sélectionnez cette base pour y créer les tables suivantes : customers, orders, products, et order_items.


Challenge 2 : Création de Tables
Objectif : Définir les schémas de tables avec les bonnes clés.
Travail à faire :
Créez la table customers avec :
customer_id (clé primaire, auto-incrémentée)
first_name, last_name, email, phone_number
Créez la table products avec :
product_id, name, price, category
Créez la table orders avec :
order_id, customer_id (clé étrangère), order_date, total_amount
Créez la table order_items avec : 
item_id, order_id, product_id, quantity
                5. Ajoutez les clés étrangères nécessaires (orders.customer_id,                   order_items.order_id, order_items.product_id).

Challenge 3 : Insertion de Données
Objectif : Remplir les tables avec des données fictives.
Travail à faire :
Insérez au moins 5 clients, 5 produits.
Insérez plusieurs commandes passées par ces clients.
Associez les commandes aux produits via la table order_items.


Challenge 4 : Requêtes de Sélection Simples
Objectif : Interroger les tables individuellement.
Travail à faire :
Sélectionnez tous les clients.
Sélectionnez les commandes passées après le 1er janvier 2024.
Sélectionnez le nom et l’e-mail des clients ayant passé une commande.


Challenge 5 : Clauses WHERE
Objectif : Filtrer les résultats de requêtes.
Travail à faire :
Sélectionnez les clients dont le prénom est "John".
Sélectionnez les commandes dont le montant est supérieur à 100 €.
Sélectionnez les clients dont le nom commence par "D".

Challenge 6 : Mise à Jour de Données
Objectif : Modifier les enregistrements existants.
Travail à faire :
Mettez à jour le numéro de téléphone d’un client.
Augmentez le total_amount de toutes les commandes de 10%.
Corrigez une adresse e-mail incorrecte.


Challenge 7 : Suppression de Données
Objectif : Supprimer proprement des données liées.
Travail à faire :
Supprimez les commandes antérieures à 2023.
Supprimez un client et toutes ses commandes associées (ON DELETE CASCADE).
Supprimez toutes les commandes d’un client spécifique.
Table customers
customer_id	first_name	last_name	email	phone_number
1	John	Doe	john.doe@gmail.com	0612345678
2	Alice	Smith	alice.smith@yahoo.com	0623456789
3	David	Dubois	david.dubois@live.com	0634567890
4	Maria	Gonzalez	maria.gon@gmail.com	0645678901
5	Karim	Dali	karim.dali@outlook.com	0656789012

Table products

product_id	name	price (€)	category
1	Laptop	899.99	Electronics
2	Smartphone	599.50	Electronics
3	Office Chair	149.90	Furniture
4	Coffee Maker	79.99	Appliances
5	USB-C Cable	15.00	Accessories

Table orders
order_id	customer_id	order_date	total_amount (€)
1	1	2024-01-15	914.99
2	3	2024-03-02	78.99
3	2	2023-12-30	149.90
4	1	2024-04-18	614.50
5	5	2022-11-01	79.99

Table order_items
item_id	order_id	product_id	quantity
1	1	1	1
2	1	5	1
3	2	4	1
4	3	3	1
5	4	2	1
6	5	4	1
