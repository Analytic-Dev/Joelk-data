# 📊 Tableau de bord des ventes — Café & Thé  
### *Projet Data Analytics – Looker Studio*

---

## 📅 Période analysée  
**1er janvier 2023 — 31 décembre 2024**

## 📂 Source de données  
**Google Sheets lié — Table_ventes_café_thé.xlsx**

---

# 1. 🎯 Contexte et Objectifs du Projet

## 1.1 Contexte  
Ce projet s'inscrit dans un portfolio Data Analytics visant à démontrer des compétences en :

- Visualisation de données  
- Analyse commerciale  
- Construction de tableaux de bord  
- Data storytelling  

Le dashboard analyse les performances d’une enseigne fictive de distribution de café et de thé opérant aux États-Unis (2023–2024).  
**962 transactions**, **6 produits**, **10 États**, **2 catégories**, pour un **CA total de 8 127,30 €**.

## 1.2 Objectifs

- **Pilotage opérationnel** : KPIs dynamiques et visualisations clés.  
- **Analyse produit & géographique** : identifier les produits/États performants.  
- **Saisonnalité** : détecter pics et creux d'activité.  
- **Comparaison N vs N-1** : mesure de croissance.  
- **Valorisation portfolio** : démontrer maîtrise de Looker Studio et narration analytique.

---

# 2. 📘 Source de Données

## 2.1 Description du jeu de données  
Structure de la base : **962 lignes** (2023–2024)

| Champ | Description |
|-------|-------------|
| **Order ID** | Identifiant unique |
| **Date** | Date de transaction |
| **Product** | 6 références produits |
| **Category** | Coffee / Tea |
| **State** | 10 États US |
| **Units Sold** | Quantité vendue |
| **Unit Price** | Prix unitaire (€) |
| **Sales** | Units × Price |

## 2.2 Périmètre des données  
- **962 commandes**  
- **6 produits** : Espresso Energizer, Zen Green Tea, Velvety Vanilla Latte, Bold Brewed Mocha, Mystic Oolong, Bold Black Tea  
- **2 catégories** : Coffee (47,4%) — Tea (52,6%)  
- **10 États US**  
- **Période** : janv. 2023 → déc. 2024  

---

# 3. 🧱 Architecture du Tableau de Bord

## 3.1 Outil : Looker Studio  
Looker Studio a été choisi pour :

- ses connecteurs variés  
- ses filtres interactifs  
- ses visualisations natives  
- son partage simple (lien public)

## 3.2 Structure et composants  
Le dashboard est organisé en **4 zones principales** :

| Zone | Contenu | Visualisation |
|------|---------|----------------|
| **KPIs globaux** | CA, commandes, unités, AOV + delta | Scorecards |
| **Ventes par catégorie** | Coffee vs Tea | Donut |
| **Ventes par produit** | Classement des 6 produits | Barres horizontales |
| **Ventes par localisation** | Top 10 États | Barres horizontales |
| **Évolution mensuelle** | Tendance Coffee vs Tea | Histogramme empilé |

## 3.3 Filtres interactifs  
- Période  
- Produit  
- Catégorie  
- État  

---

# 4. 📈 Résultats Clés & Insights

## 4.1 KPIs 2024 — Vue d’ensemble

| Indicateur | Valeur | Variation |
|------------|--------|-----------|
| **CA 2024** | **3 585,90 €** | **-21%** |
| **Commandes** | 441 | -15,4% |
| **Quantités** | 1 036 unités | -20,4% |
| **Panier moyen** | 8,13 € | -6,7% |
| **CA total (2 ans)** | 8 127,30 € | — |

---

## 4.2 Analyse par produit  
- ⭐ **Top produits** : *Mystic Oolong* (688 €) & *Zen Green Tea* (661,50 €)  
- ☕ **Meilleur Coffee** : *Bold Brewed Mocha* (646,80 €)  
- 🔻 **Produit le moins performant** : *Espresso Energizer* (475 €)

---

## 4.3 Analyse géographique  
- 🥇 **Texas** (467,10 €) & **New York** (431,90 €) = principaux contributeurs  
- 🌎 **Répartition homogène** entre les 10 États  
- 📉 **Ohio** (309,80 €) = marché le moins actif

---

## 4.4 Saisonnalité  
- ❄️ **Pic Coffee en décembre** (356,20 €)  
- ☀️ **Creux estival en juillet** (71,10 €)  
- 🍵 **Tea stable** toute l'année (89 à 229 €)

---

# 5. 🚀 Impact Business & Valeur Métier

## 5.1 Aide à la décision  
Le dashboard répond à des questions clés :

| Question | Insight |
|----------|---------|
| Quels produits génèrent le plus de CA ? | Classement dynamique |
| L’activité est-elle en croissance ? | Comparaison N vs N-1 |
| Quels États prioriser ? | Classement + carte géographique |
| Quand lancer des promotions ? | Analyse saisonnière |
| Le panier moyen évolue-t-il ? | KPI + delta |

---

## 5.2 Bénéfices  
- **Gain de temps** : reporting automatisé  
- **Accessibilité** : partage via lien  
- **Personnalisation** : filtres utilisateurs  
- **MAJ automatique** via la source Excel  

---

## 5.3 Recommandations  
- 🔦 **Stratégie saisonnière** : maximiser Coffee en hiver  
- 📉 **Analyser la baisse de 21% en 2024**  
- 🗺️ **Développer Ohio et North Carolina**  
- 🔧 **Optimiser Espresso Energizer** via promotions ou repositionnement

---

# 6. 🎓 Compétences Démontrées

| Domaine | Compétences |
|---------|-------------|
| **Data Viz** | Conception dashboards, hiérarchie visuelle |
| **Looker Studio** | Connexions, calculs, filtres |
| **Analyse commerciale** | KPIs, saisonnalité, benchmarks |
| **Gestion données** | Nettoyage, structuration, modèles |
| **Data storytelling** | Mise en page, narration, insights |

---

# 7. 🏁 Conclusion

Ce projet illustre la capacité à transformer des données brutes en un outil de pilotage complet, visuel et orienté business.  
La combinaison entre :

- analyse produit  
- analyse géographique  
- saisonnalité  
- KPIs dynamiques  

… permet d’offrir un tableau de bord clair, actionnable et aligné sur les besoins métier.

---

# 📁 Mots-clés  
`Looker Studio` · `Data Analytics` · `Dashboard` · `Data Storytelling` · `KPIs` · `Business Analysis`
