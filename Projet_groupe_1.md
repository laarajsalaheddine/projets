# 🎯 CAHIER DES TÂCHES — PROJET FLOWERS

# 🏪 1️⃣ ESPACE PUBLIC (Boutique)

## 🔹 1.1 Catalogue Produits

L’application doit permettre :

* Affichage des produits sous forme de grille élégante
* Affichage : image, nom, prix
* Filtrage par catégorie
* Gestion pagination

---

## 🔹 1.2 Fiche Produit

Chaque produit doit avoir :

* Page détaillée
* Image principale
* Description
* Prix
* Indication stock
* Bouton ajouter au panier

---

## 🔹 1.3 Gestion Panier

Le système doit permettre :

* Ajouter un produit
* Modifier quantité
* Supprimer produit
* Calcul automatique du total
* Conserver panier pendant la session

---

## 🔹 1.4 Processus de Commande (Checkout)

L’utilisateur doit pouvoir :

* Saisir ses informations (nom, email, adresse…)
* Valider la commande
* Recevoir une confirmation
* Voir un résumé commande

---

## 🔹 1.5 Confirmation de commande

Après validation :

* Afficher numéro de référence
* Résumé produits
* Total final

# 📊 2️⃣ DASHBOARD ADMIN (Espace privé)

# 🔐 2.1 Authentification & Rôles

Le système doit intégrer :

* Authentification admin
* Protection des routes privées
* Gestion des rôles (admin / gestionnaire)
* Interdiction d’accès au public non autorisé

---

# 📦 2.2 Gestion Produits

Le dashboard doit permettre :

* Créer produit
* Modifier produit
* Supprimer produit
* Activer / Désactiver produit
* Gérer stock
* Upload image

---

# 🏷 2.3 Gestion Catégories

Le dashboard doit permettre :

* Ajouter catégorie
* Modifier catégorie
* Supprimer catégorie
* Empêcher suppression si produits liés

---

# 🛒 2.4 Gestion Commandes

Le dashboard doit permettre :

* Voir liste des commandes
* Voir détail commande
* Modifier statut (en attente, validée, expédiée…)
* Visualiser produits commandés
* Visualiser informations client

---

# 📈 2.5 Vue d’ensemble (Dashboard)

Le tableau de bord doit afficher :

* Nombre total produits
* Nombre total commandes
* Commandes en attente
* Produits en stock faible

---

# 🧾 3️⃣ LOGIQUE MÉTIER À RESPECTER

Les étudiants doivent implémenter :

* Décrémentation du stock après commande
* Blocage si stock insuffisant
* Historisation prix au moment de la commande
* Référence unique pour chaque commande
* Gestion cohérente des statuts

---

# 🎨 4️⃣ EXIGENCES UI

* Design cohérent (luxe / minimal)
* Responsive
* Feedback visuel clair (succès / erreur)
* Navigation fluide entre pages

---

# 🗂 LISTE DES PAGES PRINCIPALES À CRÉER

---

## 🌍 Espace Public

* Page d’accueil
* Page catalogue
* Page produit
* Page panier
* Page checkout
* Page confirmation

---

## 🔐 Espace Admin

* Page login
* Dashboard principal
* Page gestion produits
* Page gestion catégories
* Page gestion commandes
* Page détail commande

---