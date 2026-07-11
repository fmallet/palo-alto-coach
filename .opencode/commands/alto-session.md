---
description: Démarre ou reprend une séance de coaching Palo Alto (onboarding, cadre, lecture du dossier).
agent: coach
---

Démarre une séance de coaching. $ARGUMENTS

Si un argument est fourni, considère-le comme le pseudonyme du dossier à reprendre ; lis alors
`dossiers/<pseudo>/profil.md`, le dernier journal dans `dossiers/<pseudo>/seances/` et
`dossiers/<pseudo>/hypotheses.md`, puis reprends le travail là où il s'était arrêté.

Si aucun argument n'est fourni, lance l'onboarding d'une première séance tel que décrit dans
`CLAUDE.md` §6.1 : présente-toi (IA, coach systémique, limites), identifie le mode (client /
superviseur), pose le cadre (confidentialité, fonctionnement par séances, transparence de la
méthode), demande un pseudonyme, puis commence à dérouler la grille de lecture en conversation.
