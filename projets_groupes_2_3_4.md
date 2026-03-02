# Projet : Plateforme E-commerce B2C

# I. Sujet

Il s’agit de réaliser une **plateforme E-commerce B2C** permettant la vente de produits en ligne.

La plateforme devra comporter :

* Un **espace public** accessible à tous
* Un **espace privé (Dashboard)** accessible uniquement aux utilisateurs connectés

Le projet doit être développé en **Laravel (MVC)** avec gestion des rôles et authentification sécurisée.

---

# II. Travail demandé

La plateforme est constituée de deux espaces distincts :

---

# 1️⃣ L’espace public contient les fonctionnalités suivantes :

* Page d’accueil (présentation du site)
* Liste des produits
* Filtrage par catégorie
* Page détail d’un produit
* Affichage des avis clients
* Inscription d’un nouvel utilisateur
* Connexion d’un utilisateur existant
* Nombre total de produits
* Derniers produits ajoutés

---

# 2️⃣ L’espace privé (Dashboard)

Accessible uniquement après authentification.

Deux profils sont autorisés :

* **Admin**
* **Client (Customer)**

---

# III. Gestion des utilisateurs

## 1. Inscription

Un utilisateur qui clique sur “Inscription” doit saisir les informations suivantes :

### Informations obligatoires :

* Nom
* Prénom
* Email
* Mot de passe
* Confirmation mot de passe

### Informations optionnelles :

* Téléphone
* Adresse
* Photo de profil

Les mots de passe doivent être **hashés**.

---

## 2. Connexion

La connexion se fait avec :

* Email
* Mot de passe

L’accès aux routes doit être protégé par **middleware**.

---

## 3. Gestion des rôles

Le système doit intégrer :

* Table `users`
* Table `roles`
* Table pivot `role_user`
* (Optionnel) Table `permissions`

Un administrateur peut :

* Voir la liste des utilisateurs
* Modifier les rôles
* Suspendre un compte

---

# IV. Organisation du projet (Travail en groupes)

La classe est divisée en **3 groupes**.

Chaque groupe doit :

* Implémenter la partie **Authentification + Rôles**
* Implémenter le CRUD complet de **3 entités métier maximum**

---

# 🟦 GROUPE 2 — Catalogue Produits

## Entités :

* Product
* Category
* ProductImage

## Fonctionnalités :

### Public :

* Voir les produits
* Filtrer par catégorie
* Voir détail produit

### Dashboard (Admin) :

* CRUD produits
* CRUD catégories
* Upload images
* Gestion du stock

---

# 🟩 GROUPE 3 — Panier & Commandes

## Entités :

* Cart
* Order
* OrderItem

## Fonctionnalités :

### Client :

* Ajouter au panier
* Modifier quantité
* Supprimer produit
* Valider commande
* Voir historique commandes

### Admin :

* Voir commandes
* Modifier statut (pending → shipped → delivered)

---

# 🟥 GROUPE 4 — Paiement & Gestion Client

## Entités :

* Payment
* Address
* Review

## Fonctionnalités :

### Client :

* Ajouter / modifier adresse
* Laisser un avis
* Effectuer paiement (simulation)

### Admin :

* Voir paiements
* Modérer avis
* Supprimer avis inapproprié

---

# V. Base de Données

Le script de création de la base de données devra contenir :

* Toutes les tables nécessaires
* Les relations (Foreign Keys)
* Les contraintes d’intégrité
* Les timestamps
* Les soft deletes (optionnel)

Il est possible d’ajouter des champs supplémentaires si nécessaire.

---

# VI. Exigences Techniques

Le projet doit obligatoirement inclure :

* Architecture MVC propre
* Migrations Laravel
* Relations Eloquent
* Middleware personnalisé
* Policies
* Validation via FormRequest
* Pagination
* Seeders
* Interface soignée (ergonomie prise en compte)

---

# VII. Sécurité

* Mots de passe hashés
* Protection CSRF
* Protection des routes par rôles
* Validation des formulaires
* Interdiction d’accès direct aux routes sensibles

---

# VIII. Ergonomie

L’ergonomie du site sera prise en compte dans l’évaluation.

Les participants sont invités à :

* Soigner le design
* Organiser clairement la navigation
* Séparer espace public et dashboard
* Ajouter une interface responsive

