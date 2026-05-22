# Documentation Technique LeBusMagique

Documentation de référence pour l’ensemble des dépôts de l’organisation `LeBusMagique`.

## Objectif

- Donner une vue claire de chaque projet (rôle, stack, statut, exploitation).
- Faciliter les reprises de maintenance et les décisions de migration.
- Centraliser les conventions pour éviter la dérive documentaire entre repos.

## Cartographie des projets

| Projet | Domaine | Stack principale | Statut |
|--------|---------|------------------|--------|
| [lbm-documentation](./projects/lbm-documentation.md) | Documentation | Markdown | Actif |
| [lebusmagique-api](./projects/lebusmagique-api.md) | API / Back-office | PHP, Symfony, JWT, Docker | Actif |
| [lebusmagique-assets](./projects/lebusmagique-assets.md) | Front / WebComponents | Vue 3, Vite, Tailwind | Actif |
| [lbm-observatory](./projects/lbm-observatory.md) | Front GW2 | React 16, Webpack 5 | Actif |
| [lebusmagique-django](./projects/lebusmagique-django.md) | Backend expérimental GW2 | Python, Django | Expérimental |
| [le-bot-magique](./projects/le-bot-magique.md) | Bot Discord | Python | Maintenance |
| [le-correcteur-magique](./projects/le-correcteur-magique.md) | Bot rédaction | Python | Maintenance |
| [twitch-giveaways](./projects/twitch-giveaways.md) | Outil stream | Node.js, Express, SQLite | Maintenance |
| [lebusmagique-assets-old](./projects/lebusmagique-assets-old.md) | Legacy front | Grunt, SCSS | A archiver |
| [lebusmagique-symfony-wordpress](./projects/lebusmagique-symfony-wordpress.md) | Legacy backend/site | Symfony, WordPress | A archiver |
| [toolbox](./projects/toolbox.md) | Outil historique | Svelte, Rollup | Archive |
| [lbm-connect](./projects/lbm-connect.md) | Bot Discord vérification | Node.js, discord.js | Archive |
| [maintenance](./projects/maintenance.md) | Landing maintenance | HTML/CSS | Faible activité |
| [newsletters](./projects/newsletters.md) | Templates communication | MJML, HTML | Faible activité |

## Architecture cible (vision)

```text
LeBusMagique
├── Plateforme API
│   ├── lebusmagique-api (socle principal)
│   └── lebusmagique-django (modules GW2 à arbitrer)
├── Expérience utilisateur
│   ├── lebusmagique-assets (composants réutilisables)
│   └── lbm-observatory (application dédiée quêtes)
├── Automations communautaires
│   ├── le-bot-magique
│   ├── le-correcteur-magique
│   └── twitch-giveaways
└── Historique / patrimoine
    ├── lebusmagique-assets-old
    ├── lebusmagique-symfony-wordpress
    ├── toolbox
    ├── lbm-connect
    ├── maintenance
    └── newsletters
```

## Priorités transverses 2025-2026

- Finaliser la stratégie backend (`Symfony seul` vs `coexistence Django`).
- Réduire le périmètre legacy en planifiant les archivages.
- Standardiser les README, les scripts de lancement, les variables d’environnement.
- Installer une routine de mise à jour de cette documentation à chaque chantier majeur.

## Utilisation de ce dépôt

- Entrée principale : `README.md`
- Fiches détaillées : `projects/*.md`
- Process de contribution : `CONTRIBUTING.md`

## Sources

- [Organisation LeBusMagique (liste des repos)](https://github.com/orgs/LeBusMagique/repositories)
- [API Guild Wars 2](https://api.guildwars2.com/v2)
