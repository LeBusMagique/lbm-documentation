# lbm-documentation

## Role du projet

Ce dépôt est le point d’entrée documentaire de l’écosystème `LeBusMagique`.
Il centralise les fiches de chaque repository et sert de référence commune pour le run, la maintenance et la roadmap.

## Statut

- **Etat** : Actif
- **Criticité** : Moyenne (support aux équipes, pas de runtime production)
- **Dernière mise à jour attendue** : à chaque changement majeur d’architecture

## Contenu clé

- `README.md` : index global des projets
- `projects/*.md` : une fiche projet par dépôt
- `CONTRIBUTING.md` : règles de mise à jour documentaire

## Convention éditoriale

- Une fiche doit rester orientée exploitation (objectif, stack, run, dépendances, risques).
- Les informations obsolètes doivent être supprimées, pas accumulées.
- Les sections "Actions recommandées" doivent être courtes et actionnables.

## Procédure de mise à jour

```bash
git clone https://github.com/LeBusMagique/lbm-documentation.git
cd lbm-documentation
# Mettre à jour README + fiche(s) projet
git add .
git commit -m "docs: update project documentation"
```

## Actions recommandées

- Ajouter une checklist "Done" pour chaque mise à jour structurante.
- Lier systématiquement les fiches aux issues/projets GitHub concernés.
- Mettre en place une revue documentaire trimestrielle.
