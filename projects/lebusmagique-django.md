# lebusmagique-django

## Role du projet

Backend Django expérimental pour les modules GW2.
Le dépôt contient des modèles métiers et des endpoints dédiés (pêche, homestead, wizard vault, etc.).

## Statut

- **Etat** : Expérimental
- **Stack** : Python, Django
- **Positionnement** : candidat d’intégration ou de migration vis-à-vis de `lebusmagique-api`

## Démarrage rapide

```bash
git clone https://github.com/LeBusMagique/lebusmagique-django.git
cd lebusmagique-django
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

## Portée fonctionnelle

- Modules GW2 spécialisés avec structure de données déjà en place.
- Base utile pour prototypes rapides en Python.
- Source de comparaison pour choix d’architecture backend.

## Risques / dette identifiés

- Faible volume de commits par rapport au backend Symfony.
- Pas de trajectoire documentée officielle sur le long terme.
- Risque de duplication de logique métier entre deux backends.

## Actions recommandées

- Formaliser une décision architecture (`absorber`, `coexister`, `migrer`).
- Documenter précisément les endpoints réellement utilisés.
- Arrêter les développements parallèles non planifiés avant arbitrage.
