# 📘 Documentation du Projet – Dashboard Power BI Supply Chain & Business

## 🏷️ Titre du projet
**Dashboard Power BI – Performance Supply Chain, Business & Rentabilité**

---

## 🔍 Contexte & Objectifs

L’entreprise souhaite analyser ses performances à partir d’un ensemble de données contenant les commandes, les produits, les clients et les informations logistiques.  
L’objectif est de concevoir un dashboard Power BI complet permettant :

- une vision globale des performances (CA, profit, OTD, retards)
- une analyse approfondie par segment, produit, pays et période
- une exploration libre grâce à des filtres avancés
- une amélioration du pilotage et de la prise de décision

Ce projet valorise les compétences en **modélisation, DAX, UX/UI** et **analyse supply chain**.

---

## 📦 Jeu de données

Le dataset comprend **51 colonnes**, organisées en 4 grands axes :

| Axe | Description |
|:---|:---|
| **Commandes** | ID commande, Date de commande / Date d'expédition, Quantité commandée, Mode d'expédition, Ventes (CA), Profit, Catégorie / Sous-catégorie produit, Pays / Région / Ville de commande |
| **Clients** | ID client, Prénom, nom, email, Segment client, Localisation (pays, ville…) |
| **Produits** | Nom produit, Catégorie, Prix, Description |
| **Logistique & Délais** | Jours d'expédition réel, Jours d'expédition planifié, Risque de retard livraison |

---

## 🧩 Modèle de données

Le modèle repose sur :

- **Une table de faits :** Orders
- **Une table de dates :** Calendrier
    - Année
    - Mois
    - Année-Mois
    - Jour

**Relations utilisées :**

- **Active :** Calendrier[Date] → Orders[Date de commande]
- **Inactive** pour analyses logistiques : Calendrier[Date] → Orders[Date d'expédition] (activée via `USERELATIONSHIP`)

**Avantages :**

✔ gestion propre des analyses temporelles  
✔ séparation business vs logistique  
✔ modèle clair, lisible et performant

---

## 📐 Principales mesures DAX

| Catégorie | Mesures |
|:---|:---|
| **Business** | CA Total, CA N-1, Profit Total, Profit N-1, Marge (%), Quantité totale vendue, Profit moyen par commande, Panier moyen |
| **Time Intelligence** | Quantité Vendue Année N, Quantité Vendue Année N-1, Croissance N vs N-1, CA & Profit par mois |
| **Logistique** | Nombre de commandes livrées à temps, Nombre de commandes en retard, OTD (%) – On-Time Delivery, Taux de retard (%), Délai réel / planifié moyen |

---

## 🖥️ Structure du Dashboard (3 pages)

### 🟦 PAGE 1 — Vue d'ensemble / Performances Globales

**🎯 Objectif :** Vision synthétique des performances Business & Supply Chain.

**📊 Contenu :**
- 6 KPI clés : CA, Profit, OTD (%), Retards, Quantité vendue, Clients uniques
- Graphique combiné : CA & Profit par mois
- Carte de forme : CA par pays
- Analyse CA par segment client
- Top 10 pays en CA

**🎛️ Segments :**
- Année, Segment client, Pays

---

### 🟩 PAGE 2 — Analyse Business : CA, Profit & Rentabilité

**🎯 Objectif :** Analyser les performances commerciales et les produits.

**📊 Contenu :**
- 4 KPI Business : CA, Profit, Profit moyen, Panier moyen
- CA & Profit par mois
- CA par segment client
- CA par catégorie produit
- Scatter plot : Quantité vs Profit (taille = CA)
- Tableau détaillé produit : CA, quantité, profit, marge (%)

**🎛️ Segments :**
- Année, Catégorie produit, Segment client, Pays

---

### 🟧 PAGE 3 — Exploration libre / Self-Service BI

**🎯 Objectif :** Permettre une analyse dynamique et flexible.

**📊 Contenu :**
- **Slicers :** Année, Mois, Pays, Région de commande, Ville de commande, Segment client, Catégorie, Produit, Mode d'expédition
- Graphique dynamique : CA & Profit selon les filtres
- Tableau détaillé : commandes, dates, produit, CA, profit, quantité, segment, pays

**📝 Particularité :**
→ Pas de KPI pour laisser toute la place à l'exploration.

---

## 🎨 Design & Thème UI/UX

Le rapport utilise un **thème personnalisé moderne** :

**Palette principale**
- Bleu KPI : `#1A73E8`
- Vert profit : `#34A853`
- Rouge retards : `#EA4335`
- Fond visuels : `#FFFFFF`
- Fond canevas : `#F7F9FC`
- Bordure visuels : `#D2D2D2`

**Style**
- Interface épurée et professionnelle
- Icônes modernes
- Slicers horizontaux et verticaux pour une navigation fluide
- Mise en avant des KPI via codes couleur

---

## 🚀 Impact métier

Ce dashboard fournit :

✔ Une vision consolidée du CA, du profit et des performances logistiques  
✔ Une meilleure identification des zones à optimiser (produits, pays, segments)  
✔ Un suivi précis du taux de livraison à temps (OTD) et des retards  
✔ Une réduction du temps d'analyse grâce à l'automatisation Power BI  
✔ Une meilleure collaboration entre Supply Chain, Commerce et Finance  

> *En résumé, c’est un véritable outil de pilotage stratégique et un accélérateur de performance business.*

---

## 📝 Conclusion du projet

Ce projet démontre :

- la maîtrise de **Power BI** (modélisation, relations, DAX, UX/UI)
- la capacité à traduire des besoins métier en indicateurs pertinents
- une vision complète combinant **Supply Chain** et **Business**
- la création de dashboards interactifs à forte valeur ajoutée

Le rapport apporte des réponses rapides, visuelles et fiables aux problématiques de performance globale de l'entreprise.
