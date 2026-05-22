# lebusmagique-api

> API & back-office (Symfony 6 · PHP · JWT · Docker)

## Stack technique

PHP · Symfony · Twig · Docker

## Installation

```bash
git clone https://github.com/LeBusMagique/lebusmagique-api.git
cd lebusmagique-api
```

```bash
make up
make bash
composer install
php bin/console doctrine:migrations:migrate
```


## Scripts disponibles

```bash
npm run auto-scripts  # {'cache:clear': 'symfony-cmd', 'assets:install %PUBLIC_DIR%': 'symfony-cmd'}
```
```bash
npm run post-install-cmd  # ['@auto-scripts']
```
```bash
npm run post-update-cmd  # ['@auto-scripts']
```


## Structure du projet

- `.env`
- `.env.test`
- `.github/FUNDING.yml`
- `.github/workflows/main.yml`
- `.gitignore`
- `Makefile`
- `assets/app.css`
- `assets/app.js`
- `assets/bootstrap.js`
- `assets/controllers.json`
- `assets/controllers/hello_controller.js`
- `bin/console`
- `bin/phpunit`
- `composer.json`
- `composer.lock`
- `config/bundles.php`
- `config/jwt/.gitkeep`
- `config/packages/algolia_search.yaml`
- `config/packages/cache.yaml`
- `config/packages/debug.yaml`
- `config/packages/doctrine.yaml`
- `config/packages/doctrine_migrations.yaml`
- `config/packages/framework.yaml`
- `config/packages/gesdinet_jwt_refresh_token.yaml`
- `config/packages/lexik_jwt_authentication.yaml`
- `config/packages/liip_imagine.yaml`
- `config/packages/mailer.yaml`
- `config/packages/messenger.yaml`
- `config/packages/monolog.yaml`
- `config/packages/nelmio_cors.yaml`

## README original

![](https://img.shields.io/github/last-commit/thoanny/lebusmagique-api?style=for-the-badge)
![](https://img.shields.io/github/issues/thoanny/lebusmagique-api?style=for-the-badge)

# 🚍 Le Bus Magique (API)

API et back-office des outils du Bus Magique.

## Auteur

- [@thoanny](https://github.com/thoanny)

## Contribuer

Toute aide est bienvenue ! 

Si vous souhaitez partiper au développement de l'API du Bus Magique, contactez Thoanny. 

Si vous rencontrez des bugs, des erreurs ou si vous souhaitez partager des idées d'améliorations, de fonctionnalités, vous avez la possibilité d'[ouvrir un ticket](https://github.com/thoanny/lebusmagique-api/issues) (requiert un compte Github).
## Développement

### Démarrer la machine
```bash
  make up
```

### Premier lancement

#### Accèder à la console sur le serveur
```bash
make bash
```

#### Installer les librairires Composer (Docker)
```bash
composer install
```

#### Exécuter les migrations (Docker)
```bash
php bin/console doctrine:migrations:migrate
```

#### Importer les fixtures (Docker)
```bash
php bin/console doctrine:fixtures:load
```

#### Générer les clés JWT (Docker)
```bash
php bin/console lexik:jwt:generate-keypair
```

#### Installer les librairies NPM (local)
```bash
npm i
```

#### Générer les assets (local)
```bash
npm run dev
```

## Traductions

Pour générer les fichiers de traductions :

``php bin/console translation:extract --force fr --format=json``

## Commandes

### php bin/console lbm:events

Ajouter/mettre à jour les événements.

### php bin/console lbm:events --clean

Supprimer les événements startAt > 7 mois.

---

_Documentation générée automatiquement — 2026-05-22_
