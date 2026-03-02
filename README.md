# Rapport — Simulation de Gestion d'Entreprise ARIANE

> Journal de bord et documentation complète de notre simulation de gestion d'entreprise réalisée en groupe.

---

## 📋 Objectif du projet

L'objectif de ce projet est de gérer une entreprise virtuelle — **ARIANE** — sur plusieurs cycles de simulation. Chaque cycle représente une période décisionnelle au cours de laquelle l'équipe doit prendre des décisions stratégiques portant sur :

- La **production** (volumes, capacités, investissements),
- La **commercialisation** (prix de vente, budget marketing, canaux de distribution),
- La **finance** (financement, emprunts, remboursements),
- La **trésorerie** (gestion des flux de trésorerie, équilibres budgétaires).

L'enjeu est d'optimiser la performance globale de l'entreprise face à des concurrents simulés, en maximisant la rentabilité, les parts de marché et la santé financière.

---

## 👥 Rôles dans l'équipe

| Membre         | Rôle principal                          | Responsabilités                                              |
|----------------|-----------------------------------------|--------------------------------------------------------------|
| Membre 1       | Directeur Général / Coordinateur        | Supervision des décisions, arbitrages finaux, synthèse       |
| Membre 2       | Directeur de Production                 | Volumes de production, gestion des capacités, investissements|
| Membre 3       | Directeur Commercial / Marketing        | Prix de vente, budget pub, parts de marché                   |
| Membre 4       | Directeur Financier                     | Trésorerie, emprunts, remboursements, bilan                  |
| Membre 5       | Analyste / Contrôleur de Gestion        | Indicateurs de performance, rapports, analyses               |

---

## 🎯 Décisions prises

Les décisions ont été prises cycle par cycle. Le détail complet se trouve dans le dossier [`/decisions/`](./decisions/).

### Domaines de décision

- **Production** : volume produit, taux d'utilisation des capacités, investissements machines.
- **Prix** : positionnement tarifaire par rapport à la concurrence.
- **Marketing** : budget publicitaire et promotionnel alloué.
- **Finance** : choix de financement (autofinancement, emprunts court/long terme).
- **Trésorerie** : anticipation des besoins en fonds de roulement, gestion des décalages.

---

## 📊 Indicateurs suivis

| Indicateur                  | Description                                                       |
|-----------------------------|-------------------------------------------------------------------|
| **Marge brute**             | Chiffre d'affaires − Coût de production                          |
| **Résultat net**            | Bénéfice ou perte après charges et impôts                        |
| **Parts de marché**         | % des ventes de l'entreprise sur le marché total                 |
| **Cash-flow**               | Flux de trésorerie nets générés sur chaque période               |
| **Trésorerie nette**        | Solde de trésorerie disponible en fin de cycle                   |
| **Taux d'endettement**      | Ratio dettes / capitaux propres                                  |
| **Taux de rotation stocks** | Efficacité de la gestion des stocks                              |
| **Rentabilité (ROE/ROI)**   | Retour sur capitaux propres / Retour sur investissement          |

Les analyses détaillées se trouvent dans le dossier [`/analyses/`](./analyses/).

---

## 🏆 Résultats

### Ce qui a marché ✅

- Ajustement du prix de vente en fonction du positionnement concurrentiel dès le cycle 2.
- Augmentation progressive du budget marketing qui a permis de gagner des parts de marché.
- Anticipation des besoins de trésorerie grâce à des emprunts à court terme ciblés.
- Investissement en capacité de production au bon moment pour répondre à la demande.

### Ce qui a échoué ❌

- Sous-estimation des coûts fixes lors des premiers cycles, entraînant un résultat net négatif au cycle 1.
- Sur-production au cycle 3 ayant généré des stocks excessifs et alourdi la trésorerie.
- Retard dans la décision d'emprunt long terme, limitant les investissements.

### Ce que nous avons appris 💡

- L'importance de l'anticipation et de la cohérence entre décisions commerciales et capacité de production.
- La nécessité de surveiller simultanément la rentabilité et la liquidité.
- La valeur du travail d'équipe dans les arbitrages stratégiques.

Le bilan complet se trouve dans [`/conclusions/`](./conclusions/).

---

## 🧠 Compétences développées

- **Analyse financière** : lecture de bilans, comptes de résultat, tableaux de flux.
- **Stratégie d'entreprise** : positionnement prix, arbitrage production/marketing.
- **Gestion financière** : gestion de la trésorerie, financement, ratios.
- **Travail en équipe** : prise de décision collective, délégation, communication.
- **Résolution de problèmes** : adaptation aux résultats inattendus, ajustement de stratégie.
- **Utilisation d'outils de gestion** : tableaux de bord, indicateurs clés de performance (KPI).

---

## 📁 Structure du dépôt

```
📦 Rapport-simulation-de-gestion-d-entreprise
├── README.md                        ← Résumé du projet (ce fichier)
├── journal-de-bord.md               ← Suivi chronologique cycle par cycle
├── decisions/
│   ├── cycle-1.md                   ← Décisions du cycle 1
│   ├── cycle-2.md                   ← Décisions du cycle 2
│   ├── cycle-3.md                   ← Décisions du cycle 3
│   └── cycle-4.md                   ← Décisions du cycle 4
├── analyses/
│   ├── analyse-cycle-1.md           ← Analyse des résultats cycle 1
│   ├── analyse-cycle-2.md           ← Analyse des résultats cycle 2
│   ├── analyse-cycle-3.md           ← Analyse des résultats cycle 3
│   ├── analyse-cycle-4.md           ← Analyse des résultats cycle 4
│   └── synthese-globale.md          ← Synthèse générale des performances
├── conclusions/
│   ├── bilan-strategique.md         ← Bilan stratégique global
│   └── competences-developpees.md   ← Compétences acquises
└── fichiers/
    ├── manuel-simulation.md         ← Manuel et règles de la simulation
    └── presentation.md              ← Présentation du projet
```

---

## 🔗 Navigation rapide

- 📅 [Journal de bord](./journal-de-bord.md)
- 📂 [Décisions par cycle](./decisions/)
- 📈 [Analyses des résultats](./analyses/)
- 🏁 [Conclusions et bilan](./conclusions/)
- 📎 [Fichiers et ressources](./fichiers/)
