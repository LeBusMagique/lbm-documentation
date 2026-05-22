# twitch-giveaways

> Giveaways Twitch (JavaScript)

## Stack technique

JavaScript / HTML / CSS

## Installation

```bash
git clone https://github.com/LeBusMagique/twitch-giveaways.git
cd twitch-giveaways
```

```bash
npm install
npm run dev
```


## Scripts disponibles

```bash
npm run test  # echo "Error: no test specified" && exit 1
```

## Dépendances principales

`dotenv`, `express`, `sqlite3`, `twing`, `twitchps`


## Structure du projet

- `.gitignore`
- `giveaways.db`
- `index.js`
- `package-lock.json`
- `package.json`
- `public/css/style.scss`
- `public/css/tailwind-2.0.3.min.css`
- `public/fontawesome/LICENSE.txt`
- `public/fontawesome/css/all.min.css`
- `public/fontawesome/webfonts/fa-brands-400.eot`
- `public/fontawesome/webfonts/fa-brands-400.svg`
- `public/fontawesome/webfonts/fa-brands-400.ttf`
- `public/fontawesome/webfonts/fa-brands-400.woff`
- `public/fontawesome/webfonts/fa-brands-400.woff2`
- `public/fontawesome/webfonts/fa-regular-400.eot`
- `public/fontawesome/webfonts/fa-regular-400.svg`
- `public/fontawesome/webfonts/fa-regular-400.ttf`
- `public/fontawesome/webfonts/fa-regular-400.woff`
- `public/fontawesome/webfonts/fa-regular-400.woff2`
- `public/fontawesome/webfonts/fa-solid-900.eot`
- `public/fontawesome/webfonts/fa-solid-900.svg`
- `public/fontawesome/webfonts/fa-solid-900.ttf`
- `public/fontawesome/webfonts/fa-solid-900.woff`
- `public/fontawesome/webfonts/fa-solid-900.woff2`
- `public/img/background.jpg`
- `public/img/face-a.png`
- `public/img/face-b.png`
- `public/js/confetti.min.js`
- `public/js/jquery-3.6.0.min.js`
- `public/js/script.js`

## README original

# Le Bus Magique Twitch Giveaways

Ce bot récupère les achats de tickets avec les points de chaîne et les enregistre, tant qu'il est actif.

## Installer le bot

``npm install``

## Configurer le bot

Créer un fichier .env avec les informations suivantes :

```
PORT=0000
CHANNEL=0000000
REWARD=0abcde1f-34gh-5678-9ij0-123456klmno7
```

- PORT : port à écouter, exemple : 3000 (http://localhost:3000)
- CHANNEL : identifiant de la chaîne Twitch
- REWARD : identifiant de la récompense personnalisée

## Démarrer le bot

``node index.js``

## Arrêter le bot

Utilisez la combinaison de touches : Ctrl+C.

## OBS Studio

Créer une source "Navigateur" :
- URL : http://localhost:3000
- Largeur : largeur de votre écran
- Hauteur : hauteur de votre écran

Cocher :
- Désactiver la source quand elle n'est pas visible
- Rafraîchir le navigateur lorsque la scène devient active

Pour activer les boutons, clic droit sur la scène > Interagir.

Les boutons, de gauche à droite :
- Recharger la fenêtre (et donc les tickets et le gagnant)
- Révéler le gagnant
- Valider le gagnant et supprimer son ticket
- Supprimer tous les tickets

**Attention :** les tickets sont enregistrés en base de données (SQLite), donc lorsque vous effectuez une action (valider le gagnant, supprimer tous les tickets), cela n'a d'effet que sur la base de données. **Il faut penser aussi à compléter les demandes sur Twitch.**


---

_Documentation générée automatiquement — 2026-05-22_
