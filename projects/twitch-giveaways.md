# twitch-giveaways

## Role du projet

Outil de gestion de giveaways Twitch basé sur les points de chaîne.
Le service enregistre les participants et fournit une interface utilisable en stream (OBS navigateur).

## Statut

- **Etat** : Maintenance
- **Stack** : Node.js, Express, SQLite, front statique
- **Usage** : activation ponctuelle pendant les événements stream

## Démarrage rapide

```bash
git clone https://github.com/LeBusMagique/twitch-giveaways.git
cd twitch-giveaways
npm install
node index.js
```

## Configuration attendue

Fichier `.env` minimal :

```env
PORT=3000
CHANNEL=<id_chaine_twitch>
REWARD=<id_reward_twitch>
```

## Comportement fonctionnel

- Enregistrement des tickets en base SQLite (`giveaways.db`).
- Interface locale accessible sur `http://localhost:<PORT>`.
- Contrôle stream via source navigateur OBS.

## Risques / dette identifiés

- Tests absents (`npm test` par défaut non implémenté).
- Gestion de concurrence/transactions SQLite à fiabiliser.
- Documentation de procédure stream à standardiser.

## Actions recommandées

- Ajouter des tests d’intégration sur les cas critiques (tirage, suppression, reset).
- Documenter un runbook "avant / pendant / après stream".
- Prévoir sauvegarde/restauration de la base locale.
