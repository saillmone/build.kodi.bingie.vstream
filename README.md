# Dépôt Kodi - Bingie Mod & vStream

Ce dépôt GitHub Pages héberge une version modifiée du skin **Bingie** (`skin.bingie.mod`), une version personnalisée de **vStream**, ainsi que toutes les dépendances requises pour leur bon fonctionnement — notamment le module **TMDb Bingie Helper** spécifique au build. L'ensemble est packagé pour permettre l'installation et la mise à jour automatique via Kodi.

## Source à ajouter dans Kodi

Dans le **Gestionnaire de fichiers** de Kodi, ajoutez la source suivante :

> **`https://saillmone.github.io/build.kodi.bingie.vstream/`**

> ⚠️ **Erreur de connexion au dépôt ? (À lire avant tout)** Si Kodi affiche « Impossible de se connecter au dépôt » juste après l'ajout de la source ou l'installation, **fermez Kodi complètement et relancez-le** — le dépôt se synchronise automatiquement au démarrage. C'est le problème le plus fréquent et il se résout systématiquement ainsi. Cette mise en garde s'applique aux deux méthodes ci-dessous.

---

## Préparation des Clés API (Pour le Wizard)

Le Wizard d'installation permet d'injecter automatiquement vos clés API via un code [Pastebin](https://pastebin.com/).

1. Préparez un *paste* (visibilité "Public" ou "Unlisted") respectant strictement la syntaxe suivante (texte brut, aucune espace autour du `=`) :

```text
omdb=VOTRE_CLE
mdblist=VOTRE_CLE
alldebrid_token=VOTRE_TOKEN
youtube_key=VOTRE_CLE
youtube_id=VOTRE_ID
youtube_secret=VOTRE_SECRET
```

2. Enregistrez le *paste* et repérez l'URL générée. L'identifiant correspond aux caractères situés à la fin de l'URL. Par exemple, pour `https://pastebin.com/aBcD1eF2`, l'identifiant est **`aBcD1eF2`**. Conservez-le pour l'installation.

**Utilité et liens pour générer vos clés :**
* **OMDb API** *(Affiche les notes des films et séries)* : [omdbapi.com/apikey.aspx](https://www.omdbapi.com/apikey.aspx)
* **MDBList** *(Complète les notes et métadonnées)* : [mdblist.com](https://mdblist.com/) (Clé accessible dans les préférences du compte)
* **AllDebrid** *(Débloque l'accès aux releases)* : [alldebrid.fr/apikeys](https://alldebrid.fr/apikeys/)
* **YouTube API** *(Permet la lecture des bandes-annonces)* : [Consulter le tutoriel détaillé (TUTO_API_YOUTUBE.md)](TUTO_API_YOUTUBE.md)

### Principales extensions incluses dans le build

Le Wizard déploie un environnement pré-configuré comprenant notamment :
* **AutoCompletion for virtual keyboard** (`plugin.program.autocompletion`) : Suggestions de saisie pour le clavier virtuel.
* **OpenWizard** (`plugin.program.openwizard`) : Outils de maintenance, sauvegarde et restauration Kodi.
* **Environnement Bingie** : **Bingie mod pour vStream** (`skin.bingie.mod`) et extensions associées — Helper, Toolbox, Widgets, Skin Shortcuts, TMDb Bingie Helper — interface Netflix, menus et widgets du build.
* **vStream** (`plugin.video.vstream`) : Recherche et lecture de sources vidéo en streaming.
* **YouTube** (`plugin.video.youtube`) : Lecture des bandes-annonces et contenus YouTube.
* **Skin Helper Service Skin Backup** (`script.skin.helper.skinbackup`) : Sauvegarde et restauration des réglages skin.
* **Trakt** (`script.trakt`) : Synchronisation des visionnages avec le compte Trakt.
* **Backup** (`script.xbmcbackup`) : Sauvegarde et restauration complète du profil Kodi.
* **Up Next** (`service.upnext`) : Proposition automatique de l'épisode suivant à la fin.

## Méthode 1 : Installation complète via Wizard (Recommandée)

C'est la méthode la plus simple : elle déploie l'intégralité du pack déjà pré-configuré (skin Bingie Mod, vStream, dépendances, réglages) en une seule opération.

1. Ajoutez la source ci-dessus via **Paramètres** > **Gestionnaire de fichiers** > **Ajouter une source**, puis nommez-la `Dépôt smaLLion`.
2. Allez dans **Extensions** > icône de boîte ouverte > **Installer depuis un fichier ZIP** > `Dépôt smaLLion`.
3. Cliquez directement sur le fichier **`repository.smallion.zip`** visible à la racine pour installer le dépôt.
4. Allez dans **Installer depuis un dépôt** > **Dépôt smaLLion** > **Extensions de programmes** > **Wizard smaLLion** > **Installer**.

> 🛑 **Mise en garde — perte de configuration.** Le Wizard **écrase le dossier `userdata`** de Kodi. Toute votre configuration locale existante (extensions, profils, réglages, bases de données) sera **définitivement perdue**. N'utilisez cette méthode que sur une installation Kodi vierge (ou après une sauvegarde).

> 💡 **Configuration initiale :** Au lancement du Wizard, une fenêtre de configuration s'affiche. Saisissez votre identifiant Pastebin (ex: `aBcD1eF2`) pour injecter automatiquement toutes vos clés. Laissez vide si vous préférez les configurer manuellement plus tard.

## Méthode 2 : Installation modulaire (Avancé)

Cette méthode permet d'installer uniquement les extensions souhaitées, **sans toucher à votre configuration Kodi actuelle** (vos réglages sont préservés).

1. Ajoutez la source `https://saillmone.github.io/build.kodi.bingie.vstream/` via **Paramètres** > **Gestionnaire de fichiers** > **Ajouter une source**.
2. Allez dans **Extensions** > icône de boîte ouverte > **Installer depuis un fichier ZIP** > sélectionnez la source > cliquez sur **`repository.smallion.zip`** à la racine pour installer le dépôt.
3. Retournez dans **Extensions** > **Installer depuis un dépôt** > **Dépôt smaLLion**, puis téléchargez individuellement :
   - **Bingie mod** — dans la catégorie **Apparence / Skins**.
   - **vStream** — dans la catégorie **Extensions Vidéos**.

Les dépendances nécessaires (dont le module TMDb Helper) sont résolues automatiquement par Kodi lors de l'installation de chaque extension.

> ✅ Cette méthode **préserve les réglages actuels** de Kodi : aucune donnée `userdata` n'est écrasée.

---
*Maintenance : les mises à jour des extensions sont gérées automatiquement par Kodi via l'index `addons.xml`.*
