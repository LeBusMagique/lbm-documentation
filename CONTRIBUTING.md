# Contribuer à la documentation

## Principe

La documentation est maintenue **manuellement** pour garantir des fiches explicites, orientées exploitation et décision.

## Structure du dépôt

```text
lbm-documentation/
├── README.md            # Portail global
├── CONTRIBUTING.md      # Process de contribution
└── projects/            # Une fiche par repository
```

## Format attendu pour une fiche projet

Chaque fichier de `projects/` doit au minimum contenir :

1. `Role du projet`
2. `Statut`
3. `Démarrage rapide` (si applicable)
4. `Risques / dette identifiés`
5. `Actions recommandées`

## Workflow de contribution

```bash
git clone https://github.com/LeBusMagique/lbm-documentation.git
cd lbm-documentation
# Modifier README.md et/ou projects/*.md
git add .
git commit -m "docs: update project sheets"
git push
```

## Règles éditoriales

- Rester factuel, court et actionnable.
- Supprimer les contenus obsolètes au lieu de les empiler.
- Aligner les statuts (`Actif`, `Maintenance`, `Expérimental`, `A archiver`, `Archive`).
