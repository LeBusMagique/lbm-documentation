# 📚 Documentation — Le Bus Magique

> Documentation centralisée de tous les projets de l'organisation [LeBusMagique](https://github.com/LeBusMagique).

_Générée automatiquement le 22/05/2026_

---

## 🗂️ Projets

### 🖥️ Front-end & WebComponents

| Projet | Description | Stack | Statut |
|--------|-------------|-------|--------|
| [lebusmagique-assets](./projects/lebusmagique-assets.md) | WebComponents injectés sur le site | Vue 3 · Vite · Tailwind | ✅ Actif |
| [lbm-observatory](./projects/lbm-observatory.md) | Suivi des quêtes GW2 | React 16 · Webpack 5 | ✅ Actif |
| [lebusmagique-assets-old](./projects/lebusmagique-assets-old.md) | Assets legacy | Grunt · SCSS | ⚠️ À archiver |

### ⚙️ API & Back-end

| Projet | Description | Stack | Statut |
|--------|-------------|-------|--------|
| [lebusmagique-api](./projects/lebusmagique-api.md) | API REST + back-office | Symfony 6 · PHP · JWT | ✅ Actif |
| [lebusmagique-django](./projects/lebusmagique-django.md) | Backend expérimental GW2 | Django · Python | 🔬 Expérimental |
| [lebusmagique-symfony-wordpress](./projects/lebusmagique-symfony-wordpress.md) | Génération 1 | Symfony + WordPress | ⚠️ À archiver |

### 🤖 Bots & Outils

| Projet | Description | Stack | Statut |
|--------|-------------|-------|--------|
| [le-bot-magique](./projects/le-bot-magique.md) | Bot Discord | Python | ✅ Actif |
| [le-correcteur-magique](./projects/le-correcteur-magique.md) | Outil rédacteurs | Python | ✅ Actif |
| [twitch-giveaways](./projects/twitch-giveaways.md) | Giveaways Twitch | JavaScript | 🔍 À évaluer |

### 📦 Archivés

| Projet | Description | Archivé |
|--------|-------------|---------|
| [toolbox](./projects/toolbox.md) | Boîte à outils | Jul 2022 |
| [lbm-connect](./projects/lbm-connect.md) | Bot Discord vérification | Jun 2022 |
| [newsletters](./projects/newsletters.md) | Sources newsletters | 2020 |
| [maintenance](./projects/maintenance.md) | Page de maintenance | 2021 |

---

## 🏗️ Architecture globale

```
LeBusMagique
├── Front (Vercel)
│   ├── lebusmagique-assets   → lbm-assets.vercel.app (WebComponents)
│   └── lbm-observatory       → suivi quêtes GW2
│
├── API (serveur dédié)
│   ├── lebusmagique-api      → API REST + back-office (Symfony)
│   └── lebusmagique-django   → modules GW2 expérimentaux
│
└── Bots (serveur Discord)
    ├── le-bot-magique        → bot Discord principal
    └── le-correcteur-magique → outil rédacteurs
```

---

## 🔗 Liens utiles

- [Organisation GitHub](https://github.com/LeBusMagique)
- [Site Le Bus Magique](https://lebusmagique.fr)
- [API GW2 officielle](https://api.guildwars2.com/v2)
- [GitHub Project — Roadmap](https://github.com/orgs/LeBusMagique/projects)

---

_Cette documentation est générée automatiquement depuis les repos GitHub de l'organisation._
