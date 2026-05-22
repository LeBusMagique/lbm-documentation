# lebusmagique-assets

> WebComponents (Vue 3 · Vite · Tailwind · lbm-assets.vercel.app)

## Stack technique

Vue 3 · Vite · Tailwind CSS · WebComponents

## Installation

```bash
git clone https://github.com/LeBusMagique/lebusmagique-assets.git
cd lebusmagique-assets
```

```bash
npm install
npm run dev
```


## Scripts disponibles

```bash
npm run dev  # vite
```
```bash
npm run build  # vite build
```
```bash
npm run preview  # vite preview
```
```bash
npm run lint  # eslint . --ext .vue,.js,.jsx,.cjs,.mjs --fix --ignore-path .gitignore
```
```bash
npm run format  # prettier --write src/
```
```bash
npm run json-data  # node ./scripts/json-data.js
```

## Dépendances principales

`axios`, `crypto-js`, `lodash.debounce`, `markdown-it`, `markdown-it-shortcode-tag`, `pinia`, `tippy.vue`, `uuid`, `vue`, `vue-draggable-plus`


## Structure du projet

- `.eslintrc.cjs`
- `.gitignore`
- `.prettierrc.json`
- `.vscode/extensions.json`
- `README.md`
- `index.html`
- `package-lock.json`
- `package.json`
- `postcss.config.js`
- `public/favicon.ico`
- `public/img/Activation.png`
- `public/img/Recharge.png`
- `public/img/day.svg`
- `public/img/dusk_dawn.svg`
- `public/img/events/ACHIEVEMENT.png`
- `public/img/events/BOUNTY.png`
- `public/img/events/DEFAULT.png`
- `public/img/events/DUNGEON.png`
- `public/img/events/EVENT.png`
- `public/img/events/FESTIVAL.png`
- `public/img/events/FRAC.png`
- `public/img/events/GUILD_MISSION.png`
- `public/img/events/HP_RUN.png`
- `public/img/events/META_EVENT.png`
- `public/img/events/PVP.png`
- `public/img/events/RAID.png`
- `public/img/events/ROLE_PLAY.png`
- `public/img/events/STORY.png`
- `public/img/events/STREAM.png`
- `public/img/events/STRIKE.png`

## README original

# Assets du Bus Magique

Outils et ressources pour le site du Bus Magique.

Les icônes proviennent de remixicon.com

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```

## Intégrer au site du Bus Magique

Sur e-monsie, dans "Options de référencement" puis "Balises méta supplémentaires", importer le script `<script type="module" src="https://lbm-assets.vercel.app/index.js"></script>`
(ne pas oublier l'atribut type=module !) et `<link rel="stylesheet" href="https://lbm-assets.vercel.app/index.css">` puis dans le code de la page, utiliser les balises CustomElements.

## CustomElements

### LBM Menu

Pour afficher le menu :

```html
<lbm-menu></lbm-menu>
```

**Attributs**

| Attribut | Description                                             | Exemple         |
| -------- | ------------------------------------------------------- | --------------- |
| color    | Changer la couleur principale du menu, code hexadécimal | color="#ff00ff" |

**Sprites**

Les images pour le sprite se trouvent dans : `src\sprites`. Le taille doit être de 24&times;24px.

**Éditeur de menu**

Pour utiliser l'éditeur du menu, il faut ajouter dans la page :

```html
<div id="lbm-menu-editor"></div>
```

### GW2 Wizard Vault

```html
<gw2-wizard-vault></gw2-wizard-vault>
```

Application de la chambre forte du sorcier en 3 onglets (objectifs, récompenses et héritage).

### GW2 Timers (Work in progress)

```html
<gw2-events-timer></gw2-events-timer>
```

Nouvelle version des timers des événements et worl boss de Guild Wars 2.

### Demande de ticket (Work in progress)

```html
<lbm-ticket-request></lbm-ticket-request>
```

### Compagnon de pêche

```html
<gw2-fishes></gw2-fishes>
```

### Recettes

Afficher une recette sous la forme d'un bloc :

```html
<gw2-recipe id="7283"></gw2-recipe>
```

Afficher une recette sous la forme d'une ligne :

```html
<gw2-recipe id="7283" display="inline"></gw2-recipe>
```

Afficher une recette sous la forme d'une liste :

```html
<gw2-recipe id="7283" display="list"></gw2-recipe>
```

### Décorations du pavillon

Afficher l'outil de décorations du pavillon.

⚠️ **L'URL de la page doit être ajoutée à GW2Auth !**

```html
<gw2-homestead></gw2-homestead>
```

Possibilité d'ajouter les attributes "panel" et "tab" :

- panel "upgrades" :
    - tabs :
        - cats
        - nodes
        - glyphs
- panel "homestead"
- panel "guildhall"


---

_Documentation générée automatiquement — 2026-05-22_
