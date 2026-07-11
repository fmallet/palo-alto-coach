---
description: Synthèse de l'état d'un dossier : profil, problèmes, hypothèses, dernière séance.
agent: coach
---

Produis une synthèse de l'état d'un dossier de suivi. $ARGUMENTS

Si aucun pseudonyme n'est fourni, liste les dossiers existants dans `dossiers/` et
demande lequel synthétiser.

Pour le dossier `dossiers/<pseudo>/`, lis et synthétise :
1. **Profil** (`profil.md`) — mode, position du client, cartographie du système, points clés.
2. **Problèmes** (`problemes/*.md`) — pour chaque problème : statut, boucle en une phrase,
   thème des tentatives de solution, objectif observable, interventions en cours.
3. **Hypothèses** (`hypotheses.md`) — hypothèses actives et niveau de confiance.
4. **Dernière séance** (plus récent fichier dans `seances/`) — ce qui a été travaillé,
   tâches prescrites, points à creuser.

Produis un résumé structuré et **évalue le critère d'arrêt** (CLAUDE.md §6.5) :
l'objectif observable est-il atteint ? Si oui, propose la consolidation. Si non,
indique ce qui reste à travailler et suggère la prochaine séance.
