---
description: Crée un nouveau dossier de suivi client à partir des gabarits.
agent: coach
---

Crée un nouveau dossier de suivi pour le pseudonyme fourni. $ARGUMENTS

Étapes :
1. Demande un pseudonyme si aucun argument n'est fourni (jamais le vrai nom).
2. Vérifie que `dossiers/<pseudo>/` n'existe pas déjà. S'il existe, propose plutôt de
   reprendre le dossier existant (commande `/seance <pseudo>`).
3. Crée la structure suivante en copiant les gabarits de `templates/` :
   ```
   dossiers/<pseudo>/
     profil.md          # depuis templates/profil.md
     hypotheses.md      # depuis templates/hypotheses.md
     problemes/         # dossier vide (créé au besoin)
     seances/           # dossier vide (créé au besoin)
   ```
4. Remplis le `profil.md` avec le pseudonyme, la date du jour, et laisse les autres champs
   vides (à compléter au fil des séances).
5. Confirme la création et propose de démarrer la première séance avec `/seance <pseudo>`.
