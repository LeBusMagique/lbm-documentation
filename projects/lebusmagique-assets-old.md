# lebusmagique-assets-old

## Role du projet

Ancienne base d’assets front-end du Bus Magique (Grunt/SCSS/JS).
Le dépôt est historique et remplacé fonctionnellement par `lebusmagique-assets`.

## Statut

- **Etat** : A archiver
- **Stack** : Grunt, JavaScript, SCSS
- **Contexte** : legacy, à conserver uniquement comme source de récupération

## Ce que contient le dépôt

- Outils front historiques (timers, embeds, composants d’époque).
- Documentation HTML locale sous `documentation/`.
- Configuration déploiement héritée (`netlify.toml`).

## Risques / dette identifiés

- Stack obsolète, coût de maintenance élevé.
- Confusion possible entre version legacy et version actuelle des assets.
- Dépendances non alignées avec la chaîne moderne Vue/Vite.

## Plan recommandé

- Vérifier qu’aucune page en production ne dépend encore de ces assets.
- Migrer les éléments encore utiles vers `lebusmagique-assets`.
- Archiver le dépôt sur GitHub après validation opérationnelle.
