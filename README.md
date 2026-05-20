# Dépôt Kodi Personnel - smaLLion

Ce dépôt GitHub Pages héberge le dépôt officiel Kodi permettant l'installation et la mise à jour automatique du build personnalisé.

## Extensions incluses et modifications

* **Dépôt smaLLion** (`repository.smallion`) : L'extension mère du dépôt.
* **Wizard smaLLion** (`script.preloader.smallion`) : Le preloader de configuration. Installe automatiquement : Bingie (skin, widgets, TMDB Bingie Helper), vStream (listes Pastebin Les Alkodiques), Trakt, Up Next, YouTube, OpenWizard, AutoCompletion for virtual keyboard.
* **vStream (Modifié)** (`plugin.video.vstream`) : Version optimisée intégrant la prise en compte des logos des films ainsi qu'une option de filtrage des releases.
* **Skin Bingie (Modifié)** (`skin.bingie`) : L'habillage graphique adapté pour accepter des widgets pointant directement vers les dossiers internes de vStream. La fenêtre contextuelle présentant les releases a également été refondue pour offrir une meilleure lisibilité.

## Procédure d'installation dans Kodi

1. Dans Kodi, allez dans **Paramètres** > **Gestionnaire de fichiers** > **Ajouter une source**.
2. Saisissez l'URL exacte suivante : `https://saillmone.github.io/build.kodi.bingie.vstream/`
3. Nommez la source : `Dépôt smaLLion`.
4. Revenez au menu principal de Kodi, puis allez dans **Extensions** > icône de boîte ouverte > **Installer depuis un fichier ZIP**.
5. Sélectionnez `Dépôt smaLLion`.
6. Cliquez directement sur le fichier **`repository.smallion.zip`** visible à la racine pour installer le dépôt.

> ⚠️ **Erreur de connexion au dépôt ?** Si Kodi affiche "Impossible de se connecter au dépôt" après l'installation, **ferme Kodi complètement et relance-le** — le dépôt se synchronise automatiquement au démarrage.

7. Allez ensuite dans **Installer depuis un dépôt** > **Dépôt smaLLion** > **Extensions de programmes** > **Wizard smaLLion** > **Installer**.

> 🛑 **Installation réservée à un Kodi vierge.** Le Wizard supprime TOUTE la configuration existante (extensions, profils, bases de données). Effectue un Fresh Start avant de lancer le Wizard.

> ⚠️ **Configuration initiale :** Il est recommandé de renseigner vos différentes clés API dans la fenêtre de configuration qui s'affiche lors de l'installation. Cela permet d'obtenir un build clé en main immédiatement opérationnel dès la fin du déploiement.

---
*Maintenance : Les mises à jour des extensions sont gérées automatiquement par Kodi via l'index `addons.xml`.*