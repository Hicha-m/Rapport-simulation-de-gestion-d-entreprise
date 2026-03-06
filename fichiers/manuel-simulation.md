# Manuel de Simulation — ARIANE II

> Ce document résume les règles et mécanismes de la simulation de gestion d'entreprise ARIANE II (Gambini Raymond & Tixier Daniel), tels qu'ils ont été appliqués dans le cadre du projet.

---

## Présentation générale

La simulation **ARIANE II** est un jeu de gestion d'entreprise pédagogique dans lequel plusieurs équipes s'affrontent sur un marché du matériel de sports d'hiver. Chaque équipe dirige une entreprise industrielle qui fabrique et commercialise jusqu'à trois produits.

La simulation se déroule sur **6 périodes** (trimestres), représentant chacune un trimestre de gestion. À chaque période, les équipes soumettent une trentaine de décisions et reçoivent des rapports financiers et commerciaux détaillés.

---

## Les produits

### Ski Élite
- Produit haut de gamme existant au début du jeu.
- Matières premières : 80% Fibre + 20% Résine.
- Saisonnalité : T1=20%, T2=40%, T3=25%, T4=15% des ventes annuelles.
- Prix initial de référence : 200 €/unité.
- Machines nécessaires : **MX**.

### Ski 2000
- Nouveau produit bas de gamme pouvant être lancé à tout moment.
- Matières premières : toute combinaison Fibre/Résine (flexible).
- Même saisonnalité que Ski Élite.
- **Règle de lancement** : les ventes atteignent seulement 50% la première période, puis 100% dès la période suivante.
- Machines nécessaires : **MX** (identiques à Ski Élite).

### Raquette+
- Nouveau produit contre-saisonnier (tennis).
- Matières premières : Fibre + Résine.
- Saisonnalité inversée par rapport aux skis : T1=15%, T2=20%, T3=40%, T4=25%.
- **Règle de lancement** : même règle des 50% que Ski 2000.
- Machines nécessaires : **MY** (machines spécifiques, à acheter obligatoirement).

---

## Marketing et distribution

### Force de vente
- 50 vendeurs au démarrage (12 500 €/vendeur/trimestre en salaires + charges).
- Frais de déplacement : 10 000 €/vendeur/trimestre.
- Encadrement fixe : 375 000 €/trimestre.
- Délai d'efficacité des nouveaux vendeurs : 1 trimestre à 50%, puis 100%.
- Coût d'embauche : 5 000 €/vendeur. Coût de licenciement : 50 000 €/vendeur.

### Publicité
- Budget publicité distinct par produit, décidé chaque période.
- Publicité plus efficace pour les produits bas de gamme (Ski 2000).
- Budget de référence en P0 : 600 000 €.

### Délai client
- Tous les clients exigent un **crédit de 90 jours** (1 trimestre).
- Conséquence : les encaissements du CA d'une période arrivent la période suivante.
- Possibilité d'**escompter** une partie du CA pour obtenir des liquidités immédiates (avec un coût).

---

## Production

### Matières premières
| Matière | Prix contractuel (P1-P2) | Prix spot (P3+) | Prix recyclée (P1) |
|---------|--------------------------|-----------------|---------------------|
| Fibre   | 5,00 €/u                 | Variable         | 6,00 €/u (+20%)    |
| Résine  | 1,25 €/u                 | Variable         | 1,625 €/u (+30%)   |

**Évolution des prix contractuels par période :**
| Période | Fibre (contractuel) | Résine (contractuel) |
|---------|---------------------|----------------------|
| P1-P2   | 5,00 €              | 1,25 €               |
| P3      | 5,00 €              | 1,25 €               |
| P4      | 5,00 €              | 1,25 €               |
| P5      | 6,25 €              | 2,25 €               |
| P6      | 5,00 €              | 1,25 €               |

Prix spot P4 : Fibre=10 €, Résine=3 €. Prix spot P5 : Fibre=12 €, Résine=5 €. Prix spot P6 : Fibre=10 €, Résine=3 €.

### Machines

| Type | Usage    | Coût d'achat | Capacité | Amortissement |
|------|----------|--------------|----------|---------------|
| MX   | Ski Élite + Ski 2000 | 1 250 K€ | ~75 000 u/an | 5% / période |
| MY   | Raquette+ uniquement | 1 900 K€ | à définir | 5% / période |

### Personnel
- Ouvriers permanents : 7 500 K€/trimestre (au départ).
- Heures supplémentaires : coût plus élevé qu'un ouvrier permanent à long terme.
- Agents de maîtrise : 1 750 K€/trimestre (fixe).
- R&D : réduit les coûts variables de production.

---

## Finance

### Emprunts
- **Court terme** : remboursé à la période suivante.
- **Long terme** : remboursé sur plusieurs périodes.
- En P5, les emprunts LT sont gelés (contexte économique difficile, voir newsletter P5).

### Effet escompté
- Permet d'encaisser une partie du CA de la période courante sans attendre 90 jours.
- Décision : pourcentage du CA à escompter.
- Coût : taux d'escompte appliqué (P1-P3 : 2,25%, P4 : 2,70%, P5 : 5,40%, P6 : 2,70%).

### Taux d'intérêt par période
| Période | CT   | LT   | Découvert | Escompte |
|---------|------|------|-----------|----------|
| P1      | 2,5% | 2,5% | 5,0%      | 2,25%    |
| P2      | 2,5% | 2,5% | 5,0%      | 2,25%    |
| P3      | 3,0% | 3,0% | 6,0%      | 2,70%    |
| P4      | 3,0% | 3,0% | 6,0%      | 2,70%    |
| P5      | 6,0% | N/A  | 12,0%     | 5,40%    |
| P6      | 3,0% | 3,0% | 6,0%      | 2,70%    |

---

## RSE — Responsabilité Sociétale de l'Entreprise

Disponible à partir de la **période 2**.

### Les 3 axes d'investissement
1. **Production Éco-responsable** : investissement minimum recommandé de 2 000 K€/période.
   - Réduit les émissions, améliore le recyclage des déchets.
2. **Matières Premières Recyclées** : surcoût de 20% pour la Fibre et 30% pour la Résine.
   - Contribue à la note RSE et ouvre un segment de clientèle "vert".
3. **Qualité de Vie au Travail (QVT)** : investissement minimum recommandé de 2 000 K€/période.
   - Réduit l'absentéisme et les coûts variables de production.

### Certification ISO 14001
- **Disponible à partir de P4**.
- Condition : **Note RSE Global ≥ 0,50**.
- Coût de la demande : 1 500 K€ (si note ≥ 0,5) ou 250 K€ forfaitaire (si note < 0,5).
- Coût de maintien : 1 500 K€/période.
- La certification peut être **perdue** si la note repasse sous 0,5.
- Bénéfice : accès à un nouveau segment de clientèle sensible à l'environnement.

---

## Rapports fournis après chaque période

1. **Compte de résultat** : chiffre d'affaires, coûts, marge brute, résultat net.
2. **Bilan** : actif (machines, stocks MP et PF, créances, trésorerie) et passif (capitaux propres, dettes).
3. **Tableau de trésorerie** : détail des encaissements et décaissements.
4. **Rapport de marché** : ventes par produit, stocks, indicateurs RSE.
5. **Newsletter de conjoncture** : informations sur l'économie générale et les taux.

---

## Indicateurs clés utilisés

| Indicateur            | Formule                                               |
|-----------------------|-------------------------------------------------------|
| Marge brute           | CA − Coût de production des produits vendus           |
| Résultat net          | Marge brute − Charges commerciales − Charges admin    |
| ROE                   | Résultat net / Capitaux propres × 100                 |
| Fonds de roulement    | Capitaux permanents − Actif immobilisé                |
| BFR                   | Stocks + Créances clients − Dettes fournisseurs       |
| Note RSE Global       | Moyenne pondérée des 4 notes RSE                      |

---

*Pour la présentation du projet, voir [`presentation.md`](./presentation.md).*
