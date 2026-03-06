# Rapport — Simulation de Gestion d'Entreprise ARIANE II

> Journal de bord et documentation complète de notre simulation de gestion d'entreprise réalisée en groupe dans le cadre de la formation à Polytech Montpellier (U07 – Promotion 2026).

---

## 📋 Objectif du projet

Ce projet consiste à gérer une entreprise virtuelle dans le cadre de la simulation **ARIANE II**. Chaque période représente un trimestre décisionnel au cours duquel l'équipe prend des décisions stratégiques portant sur :

- La **production** (volumes, capacités machines MX/MY, gestion des stocks, achats de matières premières),
- La **commercialisation** (prix de vente par produit, budget publicité, force de vente),
- La **finance** (emprunts CT/LT, effet escompté, gestion de la trésorerie prévisionnelle),
- La **RSE** (investissements éco-responsables, qualité de vie au travail, matières premières recyclées, certification ISO 14001).

L'enjeu est d'optimiser la performance globale de l'entreprise face à des concurrents simulés (6 firmes au total) sur un marché de matériel de sports d'hiver, en gérant une forte saisonnalité et une diversification produit progressive.

---

## 🏭 Contexte de la simulation

La simulation **ARIANE II** place les équipes à la tête d'entreprises industrielles concurrentes dans le secteur du matériel de sport. Notre entreprise (**Firme 3**) commercialise :

| Produit         | Description                                       | Lancement |
|-----------------|---------------------------------------------------|-----------|
| **Ski Élite**   | Produit haut de gamme — clientèle aisée, saisonnalité hivernale | Déjà existant (P0) |
| **Ski 2000**    | Gamme bas de gamme — marché élargi, même saisonnalité que Ski Élite | Période 1 |
| **Raquette+**   | Raquette de tennis — diversification contre-saisonnière | Période 2 |

La saisonnalité des ventes de skis est : P1=20%, P2=40%, P3=25%, P4=15% (cycle annuel T1-T4).
La saisonnalité des raquettes est inversée : P1=15%, P2=20%, P3=40%, P4=25%.

---

## 👥 Rôles dans l'équipe

| Membre         | Rôle principal                          | Responsabilités                                              |
|----------------|-----------------------------------------|--------------------------------------------------------------|
| Membre 1       | Directeur Général / Coordinateur        | Supervision des décisions, arbitrages finaux, synthèse       |
| Membre 2       | Directeur de Production                 | Volumes de production, gestion des capacités machines, stocks|
| Membre 3       | Directeur Commercial / Marketing        | Prix de vente par produit, budget publicité, parts de marché |
| Membre 4       | Directeur Financier                     | Trésorerie prévisionnelle, emprunts, effet escompté          |
| Membre 5       | Responsable RSE / Analyste              | Programme RSE, certification ISO 14001, indicateurs de performance |

---

## 🎯 Stratégie par période

La simulation s'est déroulée sur **6 périodes** (trimestres). Le détail complet se trouve dans [`/decisions/`](./decisions/).

| Période | Saison | Stratégie principale |
|---------|--------|----------------------|
| **P1** | Basse saison ski | Lancement Ski 2000 + accumulation de stock pour P2 |
| **P2** | Haute saison ski | Lancement Raquette+, start du programme RSE, vente maximale de ski |
| **P3** | Haute saison raquettes | Correction des prix (Raquette: 80€→170€), achats anticipés de MP |
| **P4** | Basse saison | Certification ISO 14001, expansion capacité (machines MY + ouvriers) |
| **P5** | Basse saison ski | Préparation P6, achat machine MX, gestion trésorerie par escompte |
| **P6** | Haute saison ski (finale) | Vente maximale, doublement marketing, clôture de la simulation |

---

## 📊 Résultats financiers par période

| Période | CA (K€) | Marge Brute (K€) | Résultat Net (K€) | Trésorerie (K€) |
|---------|---------|------------------|-------------------|-----------------|
| P1      | 37 820  | 7 258 (19,2%)    | +1 566            | 6 527           |
| P2      | 57 189  | 8 494 (14,8%)    | +738              | 4 419           |
| P3      | 43 450  | 13 529 (31,1%)   | +4 085            | 13 355          |
| P4      | 37 198  | 11 250 (30,2%)   | +1 700            | 2 628           |
| P5      | 38 932  | 10 265 (26,4%)   | +1 793            | 2 428           |
| P6      | 78 817  | 24 950 (31,7%)   | +10 711           | **−12 380 (découvert)** |
| **Total** | **293 406** | — | **+20 593** | — |

> ⚠️ La trésorerie finale est négative en P6 (découvert de 12 380 K€) en raison d'une erreur de calcul sur le pourcentage d'effets escomptés — malgré un résultat net de +10 711 K€ sur la période.

---

## 🏆 Résultats RSE

| Période | Note RSE Global | Certification ISO 14001 |
|---------|----------------|-------------------------|
| P1      | 0,16           | Non demandée            |
| P2      | 0,41           | Non demandée            |
| P3      | **0,52** ✅     | Eligible (≥ 0,5)       |
| P4      | **0,51** ✅     | **Obtenue** (1 500 K€) |
| P5      | 0,49 ⚠️        | Note sous le seuil      |
| P6      | 0,47 ⚠️        | Note sous le seuil      |

---

## ✅ Ce qui a bien fonctionné

- **Diversification réussie** : lancement de Ski 2000 et Raquette+ pour lutter contre la saisonnalité.
- **Anticipation de la haute saison** : constitution de stocks de Ski Élite en P1 pour vendre en P2.
- **Correction rapide de la tarification Raquette** : passage de 80 € à 170 € en P3 après l'erreur de P2.
- **Programme RSE** : obtention de la certification ISO 14001 en P4.
- **Rentabilité constante** : résultat net positif sur les 6 périodes, pour un total de +20 593 K€.
- **Achats anticipés de matières premières** : achat massif de fibres en P3 avant la hausse tarifaire P4 (5 €→10 €).

## ❌ Ce qui aurait pu être amélioré

- **Erreur de prix Raquette en P2** : vente à 80 € pour un coût de production d'environ 113 € → marge négative.
- **Gestion des stocks Ski 2000** : sur-production en P4-P5 → 84 837 unités invendues en fin de simulation.
- **Masse salariale sous-dimensionnée** : heures supplémentaires excessives au lieu d'embaucher des ouvriers plus tôt.
- **Erreur d'escompte en P6** : seulement 6% du CA escompté alors qu'il fallait ~22% pour éviter le découvert.
- **Pas d'emprunt LT en P1** : opportunité manquée de produire plus de skis pour la haute saison P2.

## 💡 Ce que nous avons appris

- L'importance de la **trésorerie prévisionnelle** : différence fondamentale entre rentabilité et liquidité.
- La **lecture attentive des coûts de production** avant de fixer un prix de vente.
- La **saisonnalité** impose une vision à long terme : décisions en P5 conditionnent P6.
- La **RSE** est un investissement stratégique avec des bénéfices commerciaux, mais aussi une contrainte de maintien.
- La **complexité réelle** d'une entreprise industrielle : interactions production / finance / marketing / RH.

Le bilan complet se trouve dans [`/conclusions/`](./conclusions/).

---

## 🧠 Compétences développées

- **Analyse financière** : lecture de bilans, comptes de résultat, tableaux de flux de trésorerie.
- **Stratégie d'entreprise** : positionnement prix, arbitrage production/marketing, gestion de portefeuille produits.
- **Gestion de trésorerie** : trésorerie prévisionnelle, effets escomptés, emprunts CT/LT.
- **RSE** : indicateurs environnementaux, certification ISO 14001, investissements QVT.
- **Travail en équipe** : prise de décision collective, délégation, gestion des désaccords.
- **Résilience** : capacité à analyser les erreurs et corriger la trajectoire rapidement.

---

## 📁 Structure du dépôt

```
📦 Rapport-simulation-de-gestion-d-entreprise
├── README.md                        ← Résumé du projet (ce fichier)
├── journal-de-bord.md               ← Suivi chronologique période par période
├── decisions/
│   ├── cycle-1.md                   ← Décisions de la période 1
│   ├── cycle-2.md                   ← Décisions de la période 2
│   ├── cycle-3.md                   ← Décisions de la période 3
│   ├── cycle-4.md                   ← Décisions de la période 4
│   ├── cycle-5.md                   ← Décisions de la période 5
│   └── cycle-6.md                   ← Décisions de la période 6
├── analyses/
│   ├── analyse-cycle-1.md           ← Analyse des résultats P1
│   ├── analyse-cycle-2.md           ← Analyse des résultats P2
│   ├── analyse-cycle-3.md           ← Analyse des résultats P3
│   ├── analyse-cycle-4.md           ← Analyse des résultats P4
│   ├── analyse-cycle-5.md           ← Analyse des résultats P5
│   ├── analyse-cycle-6.md           ← Analyse des résultats P6
│   └── synthese-globale.md          ← Synthèse générale des performances
├── conclusions/
│   ├── bilan-strategique.md         ← Bilan stratégique global
│   └── competences-developpees.md   ← Compétences acquises
└── fichiers/
    ├── manuel-simulation.md         ← Manuel et règles de la simulation ARIANE II
    └── presentation.md              ← Présentation du projet
```

---

## 🔗 Navigation rapide

- 📅 [Journal de bord](./journal-de-bord.md)
- 📂 [Décisions par période](./decisions/)
- 📈 [Analyses des résultats](./analyses/)
- 🏁 [Conclusions et bilan](./conclusions/)
- 📎 [Fichiers et ressources](./fichiers/)
