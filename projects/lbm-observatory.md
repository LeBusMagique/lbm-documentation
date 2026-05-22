# lbm-observatory

## Role du projet

Application web de suivi de progression des quêtes Guild Wars 2.
Permet une lecture par timeline, personnage et indicateurs de progression.

## Statut

- **Etat** : Actif
- **Stack** : React 16, Webpack 5, JavaScript
- **Licence** : MIT
- **Enjeu 2025-2026** : modernisation React 18 + migration Vite

## Démarrage rapide

```bash
git clone https://github.com/LeBusMagique/lbm-observatory.git
cd lbm-observatory
npm install
npm run dev
```

## Scripts principaux

```bash
npm run dev
npm run build
npm run lint
npm run format
npm run serve:dist
```

## Fonctionnalités centrales

- Vue chronologique complète des arcs narratifs GW2.
- Vue par personnage avec filtres et recherche.
- Statistiques globales de complétion.
- Export des données (JSON/CSV).
- Cache local pour améliorer les performances.

## Dépendances externes

- API officielle GW2 (`account`, `characters`, `progression`, `pvp`).
- Données et mapping internes (`quests_line`, `tuto_line`).

## Risques / dette identifiés

- Stack front vieillissante (React 16 / Router 5).
- Couplage historique à certains patterns Webpack legacy.
- Maintenance long terme plus coûteuse sans migration.

## Actions recommandées

- Migrer progressivement vers React 18 et React Router 6.
- Remplacer Webpack par Vite pour réduire la complexité build.
- Maintenir un changelog orienté impact utilisateur final.
