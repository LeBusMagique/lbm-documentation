# lebusmagique-api

## Role du projet

Backend principal de la plateforme LeBusMagique :

- API métier (données GW2, services internes)
- Back-office d’administration
- Authentification et flux sécurisés (JWT)

## Statut

- **Etat** : Actif
- **Stack** : PHP, Symfony 6, Twig, Docker
- **Priorité 2025-2026** : consolidation API v3 + documentation OpenAPI

## Démarrage rapide

```bash
git clone https://github.com/LeBusMagique/lebusmagique-api.git
cd lebusmagique-api
make up
make bash
composer install
php bin/console doctrine:migrations:migrate
```

## Commandes utiles

```bash
php bin/console lexik:jwt:generate-keypair
php bin/console doctrine:fixtures:load
php bin/console lbm:events
php bin/console lbm:events --clean
```

## Points d’intégration

- `lebusmagique-assets` : consommation d’endpoints pour les composants.
- `lbm-observatory` : source potentielle pour centraliser les appels GW2.
- Bots Python : candidats pour appel API au lieu d’accès directs multiples.

## Risques / dette identifiés

- Documentation endpoint partielle selon les modules.
- Arbitrage architecture avec `lebusmagique-django` encore ouvert.
- Besoin d’un suivi de santé API et de versioning stabilisé.

## Actions recommandées

- Formaliser le contrat d’API (`/api/v1`, `/api/v2`, futur `/api/v3`).
- Ajouter des tests de non-régression sur les routes critiques.
- Produire une doc OpenAPI exploitable par les équipes front/outils.
