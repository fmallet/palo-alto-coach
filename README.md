# palo-alto-coach

**Un coach IA en approche systémique et stratégique (École de Palo Alto) qui tient dans un dossier de fichiers.**
Ouvrez ce dossier avec Claude Code, écrivez votre situation : l'assistant adopte aussitôt la posture d'un coach
formé au modèle du MRI (Watzlawick, Weakland, Fisch) enrichi de **Giorgio Nardone**.

![Licence : MIT](https://img.shields.io/badge/Licence-MIT-green.svg) · Propulsé par **Claude Code**

> ⚠️ **À lire d'abord.** C'est un outil **expérimental** d'auto-accompagnement, animé par une **IA générative**.
> Ce n'est **ni une thérapie, ni un soin médical, ni un service d'urgence**, et cela ne remplace pas un·e
> professionnel·le. En cas de danger (idées suicidaires, violences…), contactez les secours (**15**, **112**,
> **3114**).

---

## Pour qui ?

- **Vous êtes sensibilisé·e à l'approche** et vous voulez l'utiliser pour vous, sur un problème concret —
  relationnel (couple, famille, équipe…) ou personnel (peur, blocage, obsession, procrastination…). Le coach
  vous accompagne pas à pas et **vous explique** ce qu'il fait.
- **Vous êtes coach / intervenant·e** formé·e à l'approche. Le coach passe en **mode superviseur** : il regarde
  avec vous l'un de vos cas, et surtout **vos propres tentatives de solution** avec votre client.

## Le principe en deux minutes

> Le problème est souvent entretenu par les **tentatives de solution** — ce qu'on fait, de bonne foi et en
> boucle, pour s'en sortir.

On ne s'attaque donc pas au problème de front. On repère la **boucle** qui le maintient et le **thème** des
tentatives répétées, puis on agit pour **inverser cette logique** (recadrage, tâche d'observation, tâche à
180°…). C'est une logique de **thérapie brève** : viser un **changement minimal suffisant**. Les termes clés
sont expliqués dans le [glossaire](methode/glossaire.md).

## Prérequis

1. Un **compte Claude payant** : forfait **Pro** ou **Max** (le plan gratuit n'inclut pas Claude Code).
2. **Claude Code** installé (voir ci-dessous). Vous pouvez l'utiliser **sans terminal** grâce à l'application de
   bureau.

## Installation pas à pas

### Voie A — sans terminal *(recommandée si l'informatique n'est pas votre métier)*

1. **Installez l'application Claude** (macOS / Windows / Linux) depuis **<https://claude.com/download>**, puis
   connectez-vous avec votre compte Pro ou Max. L'app inclut Claude Code avec une interface graphique — pas de
   ligne de commande.
2. **Téléchargez ce dossier** : sur la page GitHub du projet, bouton vert **`Code` → `Download ZIP`**, puis
   **décompressez** le fichier (double-clic).
3. Dans l'application Claude, **ouvrez le dossier** décompressé (« Open folder » / « Ouvrir un dossier »).
4. **Écrivez votre situation** dans la conversation. Le coach se présente et commence. C'est tout.

### Voie B — avec le terminal

1. Installez Claude Code :
   - **macOS / Linux** : `curl -fsSL https://claude.ai/install.sh | bash`
   - **Windows (PowerShell)** : `irm https://claude.ai/install.ps1 | iex`
2. Récupérez ce dossier (ZIP comme ci-dessus, **ou** `git clone` si vous utilisez git).
3. Ouvrez un terminal **dans ce dossier**, puis lancez :
   ```bash
   claude
   ```
4. Écrivez votre situation.

> Grand·e débutant·e du terminal ? Le guide officiel est là : <https://code.claude.com/docs/en/terminal-guide>.
> Plus d'infos sur Claude Code : <https://claude.com/claude-code>.

## Votre première séance

Écrivez simplement, avec vos mots, ce qui vous préoccupe. Le coach va :
1. se présenter (IA, coach systémique, limites) et **poser le cadre** ;
2. identifier le **mode** (vous êtes concerné·e, ou vous êtes un coach en supervision) ;
3. vous demander un **pseudonyme** (on n'écrit jamais de vrais noms) ;
4. explorer votre situation **en conversation** (pas un interrogatoire), puis proposer, le moment venu, une
   première **expérience** que vous pilotez et évaluez.

Curieux·se de voir à quoi ressemble un suivi ? Un **cas fictif complet** est dans [`exemples/`](exemples/).

## Structure du projet

```
CLAUDE.md                       # Le pilote : posture, méthode, processus (chargé au lancement)
README.md                       # Ce fichier
methode/
  grille-de-lecture.md          # La grille d'analyse MRI + Nardone
  mouvements-strategiques.md    # Catalogue des interventions et quand les utiliser
  ethique-et-securite.md        # Périmètre, détection de danger, confidentialité
  posture-superviseur.md        # Spécificités du mode supervision
  glossaire.md                  # Les termes de l'approche, expliqués
conception/
  posture-ia.md                 # Note de conception : pourquoi une posture adaptée à l'IA
templates/                      # Gabarits des dossiers de suivi
exemples/                       # Un cas fictif complet, pour illustration
dossiers/                       # VOS données — LOCALES et exclues de git (.gitignore)
```

## Confidentialité

Vos échanges créent des fichiers dans `dossiers/`, qui contiennent des informations sensibles — **y compris sur
des tiers** (votre conjoint·e, un collègue…). Ce dossier est **exclu du versionnement** (`.gitignore`) et reste
**sur votre machine**. Utilisez des **pseudonymes**, et **ne publiez jamais** votre dossier `dossiers/`.

## Les deux modes

- **Mode client** : vous êtes pris·e dans le problème ; le coach vous accompagne directement.
- **Mode superviseur** : vous êtes coach ; il travaille sur le système **vous + votre client**, notamment vos
  propres tentatives de solution. Voir [`methode/posture-superviseur.md`](methode/posture-superviseur.md).

## Contribuer

Les contributions (justesse du modèle, clarté, éthique, exemples) sont bienvenues — voir
[`CONTRIBUTING.md`](CONTRIBUTING.md) et le [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md).

## Remerciements

Ce projet n'existerait pas sans la transmission de deux formateurs auxquels je dois ma rencontre avec l'approche
stratégique et systémique, et une immense gratitude :

- **Olivier Millet** — <https://www.olivier-millet.com/>
- **Claude Duterme** — <http://www.psychotherapeute-systemique.fr/>

Merci à eux pour la rigueur, la finesse clinique et l'exigence éthique qu'ils m'ont transmises. Ce dépôt tente
d'en être un prolongement fidèle ; les maladresses ou raccourcis qui subsistent sont, eux, entièrement les miens.

## Licence & auteur

Distribué sous licence **MIT** — voir [`LICENSE`](LICENSE). Auteur : **Freddy Mallet**.

## Avertissement

Outil expérimental fondé sur une IA générative. Il ne remplace ni un·e thérapeute, ni un suivi médical, ni les
services d'urgence. Vous restez seul·e juge des décisions vous concernant.
