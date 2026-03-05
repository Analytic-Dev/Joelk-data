# 🌐 Projet : Tableau de Bord de Performance Commerciale – Power BI

## 🎯 Objectif du projet

Ce tableau de bord de performance commerciale a été conçu pour offrir une vision 360° de l'activité commerciale, de la performance des équipes et des facteurs clés de croissance. L'objectif est de fournir à la direction commerciale et aux managers un outil interactif et intuitif pour piloter la performance, identifier les leviers de croissance et optimiser l'allocation des ressources.

---

## 🏢 Impact métier

### 🎯 Bénéfices stratégiques

| Bénéfice | Impact concret |
|----------|----------------|
| **Pilotage en temps réel** | Suivi instantané du CA, des ventes et du taux de transformation pour ajuster les stratégies commerciales |
| **Optimisation de la force de vente** | Identification des commerciaux sous-performants (-20% vs objectif) et des meilleurs éléments pour reproduction des bonnes pratiques |
| **Maximisation du portefeuille produits** | Concentration des efforts sur les produits à forte marge identifiés (Livre: 29% du CA, Liseuse: 24%) |
| **Allocation géographique optimisée** | Redéploiement des ressources vers les zones à fort potentiel (Sud: 52 ventes, Centre: 11 160 € de CA) |
| **Augmentation du taux de transformation** | Ciblage des formations sur les commerciaux à faible taux (68,8% à 70,6%) pour les faire progresser vers la moyenne (78,5%) |

### 📈 ROI attendu

- **+15% de CA** grâce à l'identification et au développement des produits moteurs
- **-20% de turnover commercial** par une meilleure détection des besoins en formation et accompagnement
- **+10 points de taux de transformation** après actions correctives ciblées
- **Optimisation budgétaire** de 25% sur les actions marketing par zone géographique

---

## 📊 Fonctionnalités clés

### 🟦 Page 1 — Vue d'ensemble (Dashboard Exécutif)
**Vision macro en 5 secondes**

- **5 KPI stratégiques** : CA total (38K€), Nb ventes (161), Ticket moyen (236€), Taux transfo (78,5%), CA YTD
- **Tendances clés** : Évolution mensuelle du CA + Répartition par zone
- **Alertes visuelles** : Top 10 commerciaux + Dernières transactions

### 🟧 Page 2 — Analyse Commerciale
**Performance individuelle & matrices d'excellence**

- **Classement dynamique** des commerciaux par CA et volume
- **Matrice de performance** Commercial × Produit avec heatmap interactive
- **Détail transactionnel** pour analyse approfondie

### 🟩 Page 3 — Analyse Produits
**Contribution & rentabilité**

- **Treemap** des produits poids lourds (Livre: 11K€, Liseuse: 9K€)
- **Donut chart** de répartition du portefeuille
- **Tableau croisé** Produits × Clients pour analyse des segments

### 🟦 Page 4 — Analyse Zones Géographiques
**Stratégie territoriale**

- **Comparaison des zones** par CA et volume
- **Matrice Zone × Commercial** pour évaluer l'efficacité terrain
- **Identification** des zones à fort potentiel inexploité

---

## 🧠 Insights stratégiques

### Les 5 révélations clés

1. **Concentration des forces** : 55% du CA réalisé par les 2 meilleurs commerciaux → risque de dépendance, besoin de mutualisation des compétences
2. **Double paradoxe géographique** : La zone Sud génère le + de ventes (52) mais le - de CA (4 545€) → opportunité d'upselling massif
3. **Produits moteurs** : Livre (29% CA) et Liseuse (24% CA) représentent plus de la moitié du chiffre → priorité absolue
4. **Disparité de performance** : Écart de 21 points de taux de transformation entre le meilleur (90%) et le moins bon (68,8%) → actions correctives ciblées
5. **Spécialisation naturelle** : Certains commerciaux excellent sur des produits spécifiques → opportunité de création de rôles experts

---

## 🛠 Stack technique

| Composant | Technologie | Usage |
|-----------|-------------|-------|
| **Modélisation** | Power BI Desktop | Création du modèle et des visuels |
| **Calculs** | DAX | 12+ mesures personnalisées |
| **ETL** | Power Query | Nettoyage et préparation des données |
| **Design** | UX/UI Power BI | Thème personnalisé professionnel |
| **Source** | Excel / CSV | Données commerciales anonymisées |

---

## 📐 Mesures DAX stratégiques

```dax
// KPI fondamentaux
CA Total = SUM('Table'[Montant])
Taux Transformation = DIVIDE(CALCULATE(COUNTROWS('Table'), 'Table'[Vente] = "Oui"), COUNTROWS('Table'))

// Analyse avancée
Rang Commercial = RANKX(ALL('Table'[Commercial]), [CA Total], , DESC, Dense)
Performance Relative = DIVIDE([CA Total], CALCULATE([CA Total], ALL('Table'[Commercial])))
```

---

## 🎨 Design & expérience utilisateur

- **Identité visuelle forte** : Charte bleue professionnelle (#0C2D48, #F4F8FB)
- **Hiérarchie intuitive** : Du macro (KPI) au micro (détail transactions)
- **Interactivité fluide** : Slicers dynamiques et filtres croisés
- **Lecture optimisée** : Cartes avec ombre, valeurs en 26 px, mise en forme conditionnelle
- **Navigation fluide** : 4 pages interconnectées avec onglets clairs
- **Cohérence graphique** : Header unifié sur toutes les pages (110 px)

---

## 🚀 Conclusion stratégique

Ce tableau de bord transforme des données brutes en **leviers d'action concrets**. Il permet à la direction commerciale de :

✅ **Détecter** les opportunités de croissance en 1 clic  
✅ **Agir** rapidement sur les points de friction identifiés  
✅ **Mesurer** l'impact des décisions en temps réel  
✅ **Anticiper** les tendances plutôt que subir les résultats

**Un outil décisionnel qui passe de la simple visualisation à l'action opérationnelle.**
