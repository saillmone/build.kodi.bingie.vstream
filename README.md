# Dépôt Kodi - Bingie Mod & vStream

Ce dépôt GitHub Pages héberge une version modifiée du skin **Bingie** (`skin.bingie.mod`), une version personnalisée de **vStream**, ainsi que toutes les dépendances requises pour leur bon fonctionnement — notamment le module **TMDb Helper** spécifique au build. L'ensemble est packagé pour permettre l'installation et la mise à jour automatique via Kodi.

## Source à ajouter dans Kodi

Dans le **Gestionnaire de fichiers** de Kodi, ajoutez la source suivante :

> **`https://saillmone.github.io/build.kodi.bingie.vstream/`**

> ⚠️ **Erreur de connexion au dépôt ? (À lire avant tout)** Si Kodi affiche « Impossible de se connecter au dépôt » juste après l'ajout de la source ou l'installation, **fermez Kodi complètement et relancez-le** — le dépôt se synchronise automatiquement au démarrage. C'est le problème le plus fréquent et il se résout systématiquement ainsi. Cette mise en garde s'applique aux deux méthodes ci-dessous.

---

## Méthode 1 : Installation complète via Wizard (Recommandée)

C'est la méthode la plus simple : elle déploie l'intégralité du pack déjà pré-configuré (skin Bingie Mod, vStream, dépendances, réglages) en une seule opération.

1. Ajoutez la source ci-dessus via **Paramètres** > **Gestionnaire de fichiers** > **Ajouter une source**, puis nommez-la `Dépôt smaLLion`.
2. Allez dans **Extensions** > icône de boîte ouverte > **Installer depuis un fichier ZIP** > `Dépôt smaLLion`.
3. Cliquez directement sur le fichier **`repository.smallion.zip`** visible à la racine pour installer le dépôt.
4. Allez dans **Installer depuis un dépôt** > **Dépôt smaLLion** > **Extensions de programmes** > **Wizard smaLLion** > **Installer**.

> 🛑 **Mise en garde — perte de configuration.** Le Wizard **écrase le dossier `userdata`** de Kodi. Toute votre configuration locale existante (extensions, profils, réglages, bases de données) sera **définitivement perdue**. N'utilisez cette méthode que sur une installation Kodi vierge (ou après une sauvegarde).

> ⚠️ **Configuration initiale :** il est recommandé de renseigner vos différentes clés API dans la fenêtre de configuration qui s'affiche lors de l'installation. Cela permet d'obtenir un build clé en main immédiatement opérationnel dès la fin du déploiement.

---

## Méthode 2 : Installation modulaire (Avancé)

Cette méthode permet d'installer uniquement les extensions souhaitées, **sans toucher à votre configuration Kodi actuelle** (vos réglages sont préservés).

1. Ajoutez la source `https://saillmone.github.io/build.kodi.bingie.vstream/` via **Paramètres** > **Gestionnaire de fichiers** > **Ajouter une source**.
2. Allez dans **Extensions** > icône de boîte ouverte > **Installer depuis un fichier ZIP** > sélectionnez la source > cliquez sur **`repository.smallion.zip`** à la racine pour installer le dépôt.
3. Retournez dans **Extensions** > **Installer depuis un dépôt** > **Dépôt smaLLion**, puis téléchargez individuellement :
   * **Bingie mod** — dans la catégorie **Apparence / Skins**.
   * **vStream** — dans la catégorie **Extensions Vidéos**.

Les dépendances nécessaires (dont le module TMDb Helper) sont résolues automatiquement par Kodi lors de l'installation de chaque extension.

> ✅ Cette méthode **préserve les réglages actuels** de Kodi : aucune donnée `userdata` n'est écrasée.

---
*Maintenance : les mises à jour des extensions sont gérées automatiquement par Kodi via l'index `addons.xml`.*
