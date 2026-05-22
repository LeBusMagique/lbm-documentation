# Contribuer à la documentation

Cette documentation est **générée automatiquement** depuis les repos GitHub de l'org LeBusMagique.

## Mettre à jour la documentation

```bash
# Cloner le repo d'outils
git clone https://github.com/LeBusMagique/lbm-documentation.git

# Mettre à jour un projet spécifique
GITHUB_TOKEN=xxx ANTHROPIC_API_KEY=xxx python3 create-lbm-docs.py
```

## Structure

```
lbm-documentation/
├── README.md              # Index de tous les projets
├── CONTRIBUTING.md        # Ce fichier
└── projects/
    ├── lebusmagique-api.md
    ├── lebusmagique-assets.md
    ├── lbm-observatory.md
    └── ...
```

## Modifier manuellement

Les fichiers dans `projects/` peuvent être édités directement sur GitHub.
Attention : ils seront écrasés à la prochaine génération automatique.
