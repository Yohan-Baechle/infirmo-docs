# INFIRMO — T-ESP-800 (Epitech Nancy, MSC 2027)

**Le réseau professionnel des infirmiers libéraux**

Application mobile sécurisée de mise en relation pour les remplacements et
collaborations entre cabinets d'infirmiers titulaires et infirmiers remplaçants.

> Ce dépôt regroupe l'ensemble des **livrables de la phase _Project_** (cadrage &
> documentation) du projet INFIRMO. Le code de l'application sera développé dans
> un dépôt dédié lors de la phase de réalisation (à partir du jalon M2).

---

## Sommaire

- [Contexte](#contexte)
- [Structure du dépôt](#structure-du-dépôt)
- [Livrables](#livrables)
- [Maquettes](#maquettes)
- [Méthodologie & organisation](#méthodologie--organisation)
- [Contribuer](#contribuer)
- [Équipe](#équipe)

---

## Contexte

En France, plus de 100 000 infirmiers libéraux sont légalement tenus de garantir
la continuité des soins. Aujourd'hui, la recherche de remplaçants repose sur des
canaux informels (groupes Facebook, WhatsApp, bouche-à-oreille) : lents, non
structurés et non conformes au RGPD. INFIRMO comble ce vide avec une plateforme
mobile sécurisée, conforme et spécialisée.

---

## Structure du dépôt

```
.
├── README.md                      # Ce fichier
├── CONTRIBUTING.md                # Conventions de code, Git et tickets
├── docs/
│   ├── T-ESP-800-Deliveries-consignes.pdf
│   ├── livrables/
│   │   ├── INFIRMO_Cahier_des_Charges_v3-1.pdf
│   │   └── AJOUT-CDC_Revue_Conformite_RGPD.md
│   └── presentation/
│       └── PROMPT-slidesgpt-pitch-investisseur.md
└── INFIRMO_Pitch_Investisseur.pptx  # Support de soutenance (pitch investisseur)
```

---

## Livrables

| Livrable                       | Emplacement                                                            | Échéance   |
| ------------------------------ | --------------------------------------------------------------------- | ---------- |
| Cahier des charges complet     | [`docs/livrables/`](docs/livrables/INFIRMO_Cahier_des_Charges_v3-1.pdf) | Juin 2026  |
| Revue de conformité RGPD       | [`docs/livrables/`](docs/livrables/AJOUT-CDC_Revue_Conformite_RGPD.md)  | Juin 2026  |
| Pitch investisseur (slides)    | [`INFIRMO_Pitch_Investisseur.pptx`](INFIRMO_Pitch_Investisseur.pptx)   | Juin 2026  |
| Application mobile (MVP)       | _dépôt de code (M2 → M6)_                                              | Avril 2027 |
| Backend API + Module IA        | _dépôt de code (M2 → M6)_                                              | Avril 2027 |

Le cahier des charges contient notamment : PBS, WBS, OBS (matrice RACI), backlog
chiffré, plan de qualité, Definition of Done, analyse des risques, architecture
et estimation des coûts.

---

## Maquettes

Les maquettes UI/UX servent de référence visuelle pour comprendre rapidement les
fonctionnalités du produit.

- **Figma** : _<!-- Ajouter ici le lien de partage Figma -->_

---

## Méthodologie & organisation

- **Méthode** : Scrumban (sprints courts, backlog priorisé, daily, review,
  rétrospective).
- **Pilotage** : GitHub Projects (backlog, sprints, attribution des tâches,
  suivi des livrables).
- **Gestion du code** : Git Flow (`main` = production, `develop` = intégration,
  `feature/*` = développement), Pull Requests obligatoires avec relecture.
- **Environnement** : Docker (lancement local en une commande) — dans le dépôt
  de code à partir de M2.

---

## Contribuer

Les conventions de code, les règles Git (branches, commits) et le workflow de
gestion des tickets sont décrits dans [`CONTRIBUTING.md`](CONTRIBUTING.md).

---

## Équipe

| Membre                          | Rôle                     |
| ------------------------------- | ------------------------ |
| Tetiana Lombardi                | Cheffe de projet / UI-UX |
| Maxence Noizet                  | Dev Mobile (Flutter)     |
| Yohan Baechlé                   | Dev Fullstack            |
| Louis Chenot                    | Dev Backend              |
| Ziad Tiarimti                   | Dev Backend / IA         |
| Pierre-Arthur Toutouom Yountebo | Dev IA                   |
| Lazaro Marrero Rousse           | DevOps                   |
