# lebusmagique-symfony-wordpress

> Génération 1 (Symfony + WordPress) — à archiver

## Stack technique

PHP · Symfony · Twig · Docker

## Installation

```bash
git clone https://github.com/LeBusMagique/lebusmagique-symfony-wordpress.git
cd lebusmagique-symfony-wordpress
```

```bash
make up
make bash
composer install
php bin/console doctrine:migrations:migrate
```



## Structure du projet

- `.env`
- `.env.test`
- `.gitignore`
- `Builds.png`
- `Builds.xmind`
- `Gw2Raids.xmind`
- `LBMv2.xmind`
- `README.md`
- `assets/images/arenanet-white.png`
- `assets/images/arenanet.png`
- `assets/images/background.jpg`
- `assets/images/eod.png`
- `assets/images/hot-eod.png`
- `assets/images/hot-pof-eod.png`
- `assets/images/hot-pof.png`
- `assets/images/hot.png`
- `assets/images/map-check.png`
- `assets/images/map-guide.png`
- `assets/images/map-play.png`
- `assets/images/map-uncheck.png`
- `assets/images/map-zoom.png`
- `assets/images/pof-eod.png`
- `assets/images/pof.png`
- `assets/images/sprite.png`
- `assets/images/sprites/a-quelques-pierres-de-la-maison-druidique.png`
- `assets/images/sprites/acquerir-son-hall-de-guilde-caverne-doree-precipice-perdu-et-refuge-de-chassevent.png`
- `assets/images/sprites/acte-1-succes.png`
- `assets/images/sprites/acte-2-succes.png`
- `assets/images/sprites/acte-3-succes.png`
- `assets/images/sprites/acte-4-succes.png`

## README original

# Le Bus Magique

## Process de mise en production

### En local

0. `git clone git@bitbucket.org:anthony-d/lebusmagique-symfony-wordpress.git .`
0. Lancer le fichier `production.sh`
0. S'il n'y a pas eu de modifications de composer, supprimer `/vendor`
0. Transférer les fichiers via FTP

### En ligne

0. `ssh amiibo`
0. `cd lebusmagique`
0. Si changements dans la base de données Symfony : `php bin/console doctrine:migrations:migrate`
0. `php bin/console cache:clear`


..


---

_Documentation générée automatiquement — 2026-05-22_
