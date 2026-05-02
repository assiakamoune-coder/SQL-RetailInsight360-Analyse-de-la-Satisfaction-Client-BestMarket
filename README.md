# SQL-RetailInsight360-Analyse-de-la-Satisfaction-Client-BestMarket
RetailInsight360 est un projet d'analyse de données visant à évaluer la satisfaction des clients de l'enseigne BestMarket. L'objectif est d'exploiter les retours multicanaux (emails, téléphone, réseaux sociaux) pour piloter la qualité du réseau de magasins et renforcer la fidélisation via une vision à 360° de l'expérience client.

---

## 📌 Contexte du projet
BestMarket souhaite exploiter les données issues des retours clients (email, téléphone, réseaux sociaux…) afin d’évaluer la satisfaction de sa clientèle sur l’ensemble de son réseau de magasins.

Les données collectées couvrent différents aspects : cle_retour_client, note, Clé_produit, ref_magasin, date_achat, libelle_source, libelle_categorie, recommandation, cle_produit , titre_produit,, typologie_produit.

L’enjeu est de disposer d’une vision à 360° de l’expérience client, pour améliorer les processus internes et renforcer la fidélisation.

L’objectif est d’exploiter des retours multicanaux (emails, téléphone, réseaux sociaux) afin de :
- piloter la qualité du réseau de magasins  
- améliorer la satisfaction client  
- renforcer la fidélisation  
- obtenir une vision à 360° de l’expérience client  

---


## 🏗️ Architecture technique

### 1. Modélisation des données

Le projet repose sur un **schéma en étoile** :

- **Table de faits : `retour_client`**
  - notes (0–10)
  - dates d’achat
  - canaux (email, téléphone, réseaux sociaux)
  - catégories de retour

- **Dimension produit : `produit`**
  - titre produit
  - typologie (High-Tech, Alimentaire, Loisirs, Maison)

- **Dimension magasin : `ref_magasin`**
  - localisation
  - données démographiques

---

### 2. Stack technologique

- **SGBD :** SQLite  
- **Outil :** DB Browser for SQLite  
- **Reporting :** Markdown  
- **Langage :** SQL  

---

## 📊 Structure de la base de données

La base de données `feedback.db` contient :

- `retour_client` → interactions clients & notes
- `produit` → typologie des produits
- `ref_magasin` → informations magasins

---

## 📈 Indicateurs clés (KPIs)

Le projet répond à **17 analyses business**, dont :

### 📊 Performance globale
- **Net Promoter Score (NPS)** global et par canal  
- segmentation clients (promoteurs / passifs / détracteurs)

### 🏆 Performance produit
- Catégorie la plus performante : **Loisirs (8.51/10)**

### 📉 Analyse temporelle
- évolution de la satisfaction (T1 vs T2 2021)
- pic critique en **octobre**

### ⚠️ Performance magasins
- identification des magasins sous-performants
- notes inférieures à 5

---
## 🔒 Bonnes pratiques

- 💾 Sauvegardes régulières sur cloud (OneDrive / SharePoint)
- 🔐 Gestion des accès (lecture seule / écriture restreinte)
- 🧼 Contrôle qualité des données et des jointures SQL
- 🧩 Gestion des doublons et données manquantes
- ⚙️ Installation & utilisation

---

## 📌 Prérequis
DB Browser for SQLite (ou autre outil SQL)

---

## ▶️ Étapes
- Cloner le dépôt
- Ouvrir feedback.db
- Exécuter analyses.sql
- Explorer les résultats


--- 

## 💡 Gouvernance & maintenance
- Contrôle qualité des jointures SQL (INNER JOIN optimisés)
- Sécurisation des accès via RBAC
- Architecture évolutive (fidélité, panier moyen, nouveaux KPIs)

---

## 🚀 Objectif métier
Transformer les retours clients en insights exploitables pour :
- améliorer l’expérience client
- optimiser les magasins
- piloter la stratégie commerciale

---

## 📂 Livrables du projet

📄[**Expression des besoins(PDF)**](./Kamoune_Assia_expression_besoin_112025.pdf) | Cahier des charges et KPIs |

📄 [**Requêtes SQL (PPT)**](./Kamoune_Assia_presentation_112025.pptx) | 17 analyses business |



