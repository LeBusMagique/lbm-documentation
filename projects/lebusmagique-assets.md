# lebusmagique-assets

## Role du projet

Bibliothèque de WebComponents du Bus Magique.
Le dépôt fournit des composants front réutilisables injectés sur les pages du site.

## Statut

- **Etat** : Actif
- **Stack** : Vue 3, Vite, Tailwind CSS, Custom Elements
- **Déploiement** : Vercel (`index.js`, `index.css`)

## Démarrage rapide

```bash
git clone https://github.com/LeBusMagique/lebusmagique-assets.git
cd lebusmagique-assets
npm install
npm run dev
```

## Scripts clés

```bash
npm run dev
npm run build
npm run lint
npm run format
npm run json-data
```

## Composants majeurs

- `lbm-menu`
- `gw2-wizard-vault`
- `gw2-events-timer` (en stabilisation)
- `gw2-fishes`
- `gw2-recipe`
- `gw2-homestead`

## Intégration site

```html
<script type="module" src="https://lbm-assets.vercel.app/index.js"></script>
<link rel="stylesheet" href="https://lbm-assets.vercel.app/index.css">
```

## Dépendances fonctionnelles

- Données GW2 via API officielle et services LBM.
- Endpoints dédiés fournis progressivement par `lebusmagique-api`.

## Actions recommandées

- Stabiliser les composants marqués WIP avant extension du catalogue.
- Publier une doc de props/events pour chaque composant.
- Mettre en place des snapshots visuels pour limiter les régressions UI.
