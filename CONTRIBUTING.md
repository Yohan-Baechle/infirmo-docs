# Contribuer au projet INFIRMO

Ce document décrit les conventions de code, les règles Git et le workflow de
gestion des tickets adoptés par l'équipe. Il vise à faciliter l'intégration de
tout nouveau membre et à garantir la cohérence du projet.

> Référence : section 11 (Plan de qualité) du cahier des charges.

---

## 1. Conventions de code

- **Nommage** : `camelCase` (Dart), `lower_snake_case` (base de données).
- **Formatage automatique** :
  - Python (backend / IA) : **Black** + **Ruff**
  - Dart (mobile) : **`dart format`** / `flutter analyze`
- **Documentation** : un `README` par module, documentation d'API
  (Swagger / OpenAPI).
- **Sécurité** : aucun secret en clair dans le code (utiliser les variables
  d'environnement), validation systématique des entrées.
- **Versions** : tags sémantiques `vX.Y.Z` sur `main` après validation en
  staging.

---

## 2. Conventions Git

### Branches

Modèle **Git Flow** : `main` (production), `develop` (intégration),
`feature/*` (développement).

Les branches doivent suivre l'un des formats suivants (vérifié automatiquement
par la CI) :

```
feature/<desc>   bugfix/<desc>   hotfix/<desc>   docs/<desc>
ci/<desc>        test/<desc>     refactor/<desc>  dev/<desc>
```

- `main` et `develop` sont **protégées** : toute modification passe par une
  Pull Request validée par au moins un relecteur.
- **Merge** : *squash merge* sur `develop`, *merge commit* sur `main`.

### Commits

Les messages de commit respectent la convention **Conventional Commits** :

```
feat   fix   docs   style   refactor   test   chore   ci   perf   build
```

Exemple : `feat(auth): add JWT cookie login`

- Pour être guidé lors de la rédaction d'un commit : `npx git-cz`.
- Les releases sont générées automatiquement avec **semantic-release**
  (`npx semantic-release`), selon la configuration `release.config.js`.

---

## 3. Gestion des tickets

- **Outil** : GitHub Projects.
- **Workflow** : `To Do` → `In Progress` → `In Review` → `Done`.
- **Labels** : `bug`, `feature`, `improvement`, `documentation`, `urgent`.
- **Attribution** : chaque ticket est assigné à un responsable et rattaché à un
  sprint.

---

## 4. Definition of Done

Une contribution n'est considérée comme terminée que lorsque **tous** les
critères suivants sont satisfaits :

- [ ] Code développé et relu (revue de code, fusionné sur la branche d'intégration)
- [ ] Critères d'acceptation validés (tests et/ou démonstration)
- [ ] Tests automatisés au vert (unitaires, intégration, E2E si applicable)
- [ ] Aucune régression critique (build CI vert)
- [ ] Sécurité vérifiée (authentification, autorisations, aucun secret en clair)
- [ ] Documentation à jour (README, endpoints API, notes de release)
- [ ] Déployé et validé en environnement de recette (staging)

> Référence : section 12 (Definition of Done) du cahier des charges.
