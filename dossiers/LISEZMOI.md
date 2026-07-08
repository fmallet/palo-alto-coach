# Dossiers de suivi

Ce répertoire accueille un sous-dossier par personne accompagnée, créé automatiquement par le coach
(en supervision, la personne accompagnée est le **coach** lui-même) :

```
dossiers/<pseudo>/
  profil.md            # cf. templates/profil.md
  problemes/<slug>.md  # cf. templates/probleme.md (un fichier par problème)
  seances/AAAA-MM-JJ.md# cf. templates/seance.md (un fichier par séance)
  hypotheses.md        # cf. templates/hypotheses.md
```

> Pour voir à quoi ressemble un dossier rempli, regardez l'exemple **fictif** dans [`../exemples/`](../exemples/).

## ⚠️ Confidentialité
- Le contenu de `dossiers/` est **exclu de git** (voir `.gitignore`). Seuls ce fichier et `.gitkeep` sont suivis.
- Utilisez des **pseudonymes** pour la personne accompagnée **et** pour les tiers cités.
- Ces données restent **en local**. Ne jamais les pousser sur un dépôt public.
