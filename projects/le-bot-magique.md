# le-bot-magique

## Role du projet

Bot Discord principal du Bus Magique.
Il supporte l’automatisation communautaire et des flux d’information liés aux activités de la communauté.

## Statut

- **Etat** : Maintenance
- **Stack** : Python
- **Risque** : faible documentation native du repo

## Démarrage rapide

```bash
git clone https://github.com/LeBusMagique/le-bot-magique.git
cd le-bot-magique
pip install -r requirements.txt
python main.py
```

## Fichiers clés

- `main.py` : point d’entrée du bot
- `feeds.py` : logique de récupération/traitement des flux
- `feeds.csv` : données de configuration ou mapping

## Dépendances et intégrations

- Discord API
- Eventuels flux externes selon les commandes/notifications actives

## Actions recommandées

- Ajouter un README opérationnel (variables, permissions bot, commandes).
- Écrire des docstrings sur les commandes et handlers.
- Mettre en place une stratégie de logs structurés et alertes d’erreur.
