# Manuel de Simulation — ARIANE

> Ce document résume les règles et mécanismes de la simulation de gestion d'entreprise ARIANE utilisée dans le cadre du projet pédagogique.

---

## Présentation générale

La simulation **ARIANE** est un jeu de gestion d'entreprise pédagogique dans lequel plusieurs équipes s'affrontent sur un marché fictif. Chaque équipe dirige une entreprise qui produit et commercialise un produit unique sur un marché concurrentiel.

La simulation se déroule sur **plusieurs cycles**, chacun représentant une période de gestion (trimestre ou semestre selon la configuration). À chaque cycle, les équipes soumettent leurs décisions et reçoivent les résultats sous forme de rapports financiers et commerciaux.

---

## Structure d'un cycle

Chaque cycle comprend les étapes suivantes :

1. **Analyse des résultats du cycle précédent** (comptes de résultat, bilan, parts de marché).
2. **Prise de décisions** dans les quatre domaines (production, marketing, finance, trésorerie).
3. **Soumission des décisions** à l'animateur de la simulation.
4. **Traitement** par le moteur de simulation.
5. **Publication des résultats** et préparation du cycle suivant.

---

## Les quatre domaines de décision

### 1. Production

| Paramètre                  | Description                                                        |
|----------------------------|--------------------------------------------------------------------|
| Volume de production       | Nombre d'unités à fabriquer durant le cycle                        |
| Investissement en machines | Montant investi pour augmenter la capacité de production           |
| Taux d'utilisation         | Pourcentage d'utilisation de la capacité totale installée          |

**Règles importantes :**
- On ne peut pas produire au-delà de la capacité installée.
- Les unités non vendues sont mises en stock et génèrent des coûts de stockage.
- Un investissement en machine augmente la capacité mais implique un amortissement sur plusieurs cycles.

### 2. Commercialisation

| Paramètre              | Description                                                        |
|------------------------|--------------------------------------------------------------------|
| Prix de vente unitaire | Prix auquel l'entreprise vend son produit sur le marché            |
| Budget marketing       | Montant alloué à la publicité et à la promotion                    |

**Règles importantes :**
- Le prix de vente et le budget marketing influencent la demande et les parts de marché.
- Un prix trop élevé réduit les ventes ; un prix trop bas réduit la marge.
- L'effet du marketing est partiellement différé (impact sur les cycles suivants).

### 3. Finance

| Paramètre              | Description                                                        |
|------------------------|--------------------------------------------------------------------|
| Emprunt court terme    | Emprunt remboursable sur 1 cycle pour couvrir des besoins immédiats|
| Emprunt long terme     | Emprunt remboursable sur plusieurs cycles pour financer un investissement |

**Règles importantes :**
- Les emprunts génèrent des frais financiers (intérêts).
- Un taux d'endettement trop élevé peut déclencher des pénalités ou des contraintes de financement.

### 4. Trésorerie

La trésorerie est le résultat de tous les flux financiers du cycle :
- **Encaissements** : ventes, emprunts reçus.
- **Décaissements** : achats de matières premières, salaires, loyers, remboursements, impôts.

**Règle critique :** Si la trésorerie devient négative, l'entreprise est en cessation de paiement et subit des pénalités importantes.

---

## Les rapports fournis après chaque cycle

1. **Compte de résultat** : chiffre d'affaires, coûts, marge, résultat net.
2. **Bilan** : actif (immobilisations, stocks, créances, trésorerie) et passif (capitaux propres, dettes).
3. **Tableau de trésorerie** : détail des flux d'encaissements et de décaissements.
4. **Rapport de marché** : parts de marché de chaque équipe, prix moyen du marché, demande globale.

---

## Indicateurs de performance évalués

| Indicateur                | Formule                                           |
|---------------------------|---------------------------------------------------|
| Marge brute               | CA − Coût de production                           |
| Résultat net              | Marge brute − Charges fixes − Charges financières |
| Part de marché            | Ventes entreprise / Ventes totales marché × 100   |
| Cash-flow                 | Résultat net + Amortissements                     |
| Taux d'endettement        | Dettes totales / Capitaux propres × 100           |
| ROI                       | Résultat net / Capitaux investis × 100            |

---

## Conseils généraux pour réussir la simulation

1. **Lisez attentivement les rapports** après chaque cycle avant de décider.
2. **Calibrez la production** à la demande estimée, avec une marge de sécurité modérée.
3. **Investissez en marketing** de manière progressive et continue.
4. **Anticipez la trésorerie** : simulez les flux avant de valider vos décisions.
5. **Surveillez la concurrence** : adaptez votre prix et votre marketing en fonction des autres équipes.
6. **Ne sur-investissez pas** sans avoir une demande suffisante pour justifier l'augmentation de capacité.

---

*Pour la présentation du projet, voir [`presentation.md`](./presentation.md).*
