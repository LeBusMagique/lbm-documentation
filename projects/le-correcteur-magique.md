# le-correcteur-magique

## Role du projet

Automatisation de correction/relecture pour l’équipe éditoriale.
Le service notifie et assiste le flux rédactionnel (notamment via Discord/Trello).

## Statut

- **Etat** : Maintenance
- **Stack** : Python
- **Besoins actuels** : amélioration UX pour les rédacteurs non techniques

## Démarrage rapide

```bash
git clone https://github.com/LeBusMagique/le-correcteur-magique.git
cd le-correcteur-magique
pip install -r requirements.txt
python main.py
```

## Intégrations connues

- Discord (notifications)
- Trello (déclencheurs de workflow éditorial)
- Potentiel futur avec API LBM pour enrichir les vérifications

## Risques / dette identifiés

- Expérience orientée technique, peu accessible aux profils non dev.
- Documentation d’exploitation limitée.
- Couverture test non documentée.

## Actions recommandées

- Créer une interface web simple pour l’équipe rédaction.
- Documenter les règles de correction et les scénarios de notification.
- Ajouter un guide d’exploitation "qui fait quoi en cas d’erreur".
