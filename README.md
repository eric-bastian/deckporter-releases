# Deckporter - downloads

> 🇬🇧 **English** — 🇫🇷 la version française de ce document est disponible plus
> bas : **[aller à la version française](#version-française)**.

Transfer your playlists **and their preparation** — hot cues, memory cues,
loops, beatgrids — between **Rekordbox**, **Serato** and **Traktor**, instead
of redoing by hand work you have already done in another program.

This repository holds **only the published binaries and the release notes**.

<p align="center">
  <img src="./Deckporter%20screenshot.png" width="700" alt="Preview">
</p>

## Features

- **All six directions** between Rekordbox, Serato and Traktor.
- **What travels**: playlists in their order, hot cues and memory cues (with
  their pad and colour — towards Serato, keep the source colours or use
  Serato's defaults), loops, beatgrids, track information.
- **Three ways of working**:
  - **Local conversion** — both programs are on this computer;
  - **Create a package** — take one or more playlists to another computer in a
    portable `.dkp` file, with the audio files if you wish; the destination
    program is chosen when importing;
  - **Import a package** — into the program of your choice on this computer.
- **Choose what goes**: browse the playlist tree, tick the playlists, untick
  individual tracks, listen to a track with its waveform and cue points.
- **Matching**: tracks already present at the destination are recognised, even
  under another path; doubtful cases are shown to you for a decision.
- **Conflicts**: when a track's preparation differs on both sides, you choose —
  keep the source, keep the destination, merge or ignore — track by track or in
  bulk.
- **Merge, never blind overwrite**: an existing library is completed, not
  replaced. A converted playlist replaces its previous conversion instead of
  piling up next to it.
- **Serato**: works on **copies** by default, your originals are never touched
  (writing in place is available); a crate is created in the playlist's order.
- **Rekordbox**: tracks missing from the library are created, ready to be
  analysed by Rekordbox.
- **Safety first**:
  - refuses to write while a DJ program is open;
  - a snapshot is taken before every write;
  - a **history of transfers** tells you, before any restore, what it would do
    and what it would lose — including changes made since in Rekordbox,
    Serato or Traktor; a restore can itself be undone.
- **Guided interface**: bubbles show the next step, and a report tells what
  happened to each piece of data after every transfer.
- **Four languages**: English, French, Spanish and German — Deckporter follows
  the Windows language, and the flag at the top right switches it.
- **Your library stays on your computer**: no playlist title, track title,
  artist, path or file is ever sent. At startup, Deckporter contacts its
  server to renew its licence and check for updates; it sends anonymous usage
  statistics only if you agree, and your email address only if you add one in
  **My account** (details in the release notes).

## Download

➡️ **[Latest release](../../releases/latest)**

Windows 10 / 11, 64-bit. The interface is available in English, French,
Spanish and German.

The installer is **not digitally signed**: Windows SmartScreen will show a
warning on first launch ("More info" → "Run anyway"). Check the SHA-256
fingerprint published on the release page:

```powershell
Get-FileHash .\Deckporter_Setup.exe -Algorithm SHA256
```

Installation is **per user** and requires no administrator rights.
Uninstalling removes Deckporter and its snapshot history, never what it wrote
into your DJ libraries.

## Requirements

- Windows 10 or 11, 64-bit
- At least one of: Rekordbox 6 / 7, Serato DJ Pro, Traktor
- Microsoft Edge WebView2 (present on Windows 11; installed automatically if
  missing)

## Warning

**Experimental** software, provided "as is", **without any warranty**.
Deckporter **writes into your DJ libraries**: close your DJ programs before a
transfer, and keep your own backups — snapshots are a safety net, not a
substitute. **The user assumes the entirety of the risks.**

The Traktor side has not yet been checked inside Traktor itself.

Deckporter reads and writes the encrypted Rekordbox database with the
third-party library pyrekordbox. This use **may breach the end-user licence
agreement (EULA) of AlphaTheta / Pioneer DJ**; by using it, you act in full
knowledge of the facts.

Copying audio files into a package and handing it to someone else can infringe
copyright and the licence of promotional pools: you are responsible for the
files you transfer.

---

<a id="version-française"></a>

# 🇫🇷 Version française

Transférez vos playlists **et leur préparation** — hot cues, memory cues,
boucles, grilles de tempo — entre **Rekordbox**, **Serato** et **Traktor**, au
lieu de refaire à la main un travail déjà fait dans un autre logiciel.

Ce dépôt ne contient **que les binaires publiés et les notes de version**.

<p align="center">
  <img src="./Deckporter%20screenshot.png" width="700" alt="Aperçu">
</p>

## Fonctionnalités

- **Les six directions** entre Rekordbox, Serato et Traktor.
- **Ce qui voyage** : les playlists dans leur ordre, les hot cues et memory cues
  (avec leur pad et leur couleur — vers Serato, celles de la source ou celles
  que Serato donne par défaut), les boucles, les grilles de tempo, le
  descriptif des morceaux.
- **Trois façons de travailler** :
  - **Conversion locale** — les deux logiciels sont sur cet ordinateur ;
  - **Créer un paquet** — emporter une ou plusieurs playlists vers un autre
    ordinateur dans un fichier `.dkp` portable, avec les fichiers audio si vous
    le souhaitez ; le logiciel d'arrivée se choisit à l'import ;
  - **Importer un paquet** — dans le logiciel de votre choix sur cet ordinateur.
- **Choisir ce qui part** : parcourir l'arborescence des playlists, cocher les
  playlists, décocher des morceaux, écouter un morceau avec sa forme d'onde et
  ses points de repère.
- **Appariement** : les morceaux déjà présents à l'arrivée sont reconnus, même
  sous un autre chemin ; les cas douteux vous sont soumis.
- **Conflits** : quand la préparation d'un morceau diffère des deux côtés, vous
  choisissez — garder la source, garder l'arrivée, fusionner ou ignorer —
  morceau par morceau ou en masse.
- **Fusionner, jamais écraser à l'aveugle** : une bibliothèque existante est
  complétée, pas remplacée. Une playlist convertie remplace sa conversion
  précédente au lieu de s'empiler à côté.
- **Serato** : travail sur des **copies** par défaut, vos originaux ne sont
  jamais touchés (l'écriture en place reste possible) ; un crate est créé dans
  l'ordre de la playlist.
- **Rekordbox** : les morceaux absents de la bibliothèque sont créés, prêts à
  être analysés par Rekordbox.
- **La sécurité d'abord** :
  - refus d'écrire tant qu'un logiciel DJ est ouvert ;
  - un instantané est pris avant chaque écriture ;
  - un **historique des transferts** dit, avant toute restauration, ce qu'elle
    ferait et ce qu'elle ferait perdre — y compris les modifications faites
    depuis dans Rekordbox, Serato ou Traktor ; une restauration peut elle-même
    être défaite.
- **Interface guidée** : des bulles montrent l'étape suivante, et un rapport dit
  ce qu'est devenue chaque donnée après chaque transfert.
- **Quatre langues** : français, anglais, espagnol et allemand — Deckporter suit
  la langue de Windows, et le drapeau en haut à droite permet d'en changer.
- **Votre bibliothèque reste sur votre ordinateur** : aucun titre de playlist,
  aucun titre de morceau, aucun artiste, aucun chemin et aucun fichier n'est
  jamais envoyé. Au démarrage, Deckporter contacte son serveur pour renouveler
  sa licence et vérifier les mises à jour ; il n'envoie des statistiques
  d'usage anonymes qu'avec votre accord, et votre adresse e-mail que si vous en
  ajoutez une dans **Mon compte** (détails dans les notes de version).

## Télécharger

➡️ **[Dernière version](../../releases/latest)**

Windows 10 / 11, 64 bits. Interface en français, anglais, espagnol et
allemand.

L'installateur n'est **pas signé numériquement** : Windows SmartScreen affichera
un avertissement au premier lancement (« Informations complémentaires » →
« Exécuter quand même »). Vérifiez l'empreinte SHA-256 publiée sur la page de la
release :

```powershell
Get-FileHash .\Deckporter_Setup.exe -Algorithm SHA256
```

L'installation se fait **pour l'utilisateur courant**, sans droits
administrateur. La désinstallation retire Deckporter et son historique
d'instantanés, jamais ce qu'il a écrit dans vos bibliothèques DJ.

## Prérequis

- Windows 10 ou 11, 64 bits
- Au moins un de : Rekordbox 6 / 7, Serato DJ Pro, Traktor
- Microsoft Edge WebView2 (présent sur Windows 11 ; installé automatiquement
  s'il manque)

## Avertissement

Logiciel **expérimental**, fourni « en l'état », **sans aucune garantie**.
Deckporter **écrit dans vos bibliothèques DJ** : fermez vos logiciels DJ avant un
transfert, et gardez vos propres sauvegardes — les instantanés sont un filet,
pas un substitut. **L'utilisateur assume l'intégralité des risques.**

Le côté Traktor n'a pas encore été vérifié dans Traktor lui-même.

Deckporter lit et écrit la base chiffrée de Rekordbox au moyen de la
bibliothèque tierce pyrekordbox. Cet usage **peut contrevenir au contrat de
licence utilisateur final (CLUF) d'AlphaTheta / Pioneer DJ** ; en l'utilisant,
vous agissez en connaissance de cause.

Copier des fichiers audio dans un paquet et le remettre à quelqu'un peut porter
atteinte au droit d'auteur et à la licence des pools promotionnels : vous êtes
responsable des fichiers que vous transférez.
