# Tutoriel : Obtenir ses clés API YouTube

Ce guide explique comment obtenir les trois informations nécessaires pour l'intégration YouTube dans Kodi (`youtube_key`, `youtube_id`, `youtube_secret`).

## Étape 1 : Créer un projet
1. Connectez-vous à la [Console Google Cloud](https://console.cloud.google.com/).
2. Cliquez sur la liste déroulante des projets en haut de la page, puis sur **Nouveau projet**.
3. Nommez le projet (ex: `Kodi vStream`) et cliquez sur **Créer**.

## Étape 2 : Activer l'API YouTube
1. Dans le menu de navigation (☰), allez dans **API et services** > **Bibliothèque**.
2. Cherchez **YouTube Data API v3** et sélectionnez-la.
3. Cliquez sur **Activer**.

## Étape 3 : Créer la Clé API (`youtube_key`)
1. Dans le menu de gauche, allez dans **API et services** > **Identifiants**.
2. Cliquez sur **Créer des identifiants** (en haut) > **Clé API**.
3. Copiez la clé générée. Elle correspond à votre `youtube_key`.

## Étape 4 : Configurer l'écran de consentement OAuth
1. Dans le menu de gauche, cliquez sur **Écran de consentement OAuth**.
2. Choisissez le type d'utilisateur **Externe** et cliquez sur **Créer**.
3. Remplissez les champs obligatoires (Nom de l'application, adresse e-mail d'assistance, adresse e-mail du développeur).
4. Cliquez sur **Enregistrer et continuer** pour les étapes suivantes (Champs d'application). 
5. À l'étape **Utilisateurs tests**, ajoutez votre propre adresse e-mail Google pour autoriser votre compte à utiliser l'application, puis enregistrez.

## Étape 5 : Créer l'ID et le Secret OAuth (`youtube_id` et `youtube_secret`)
1. Retournez dans la section **Identifiants**.
2. Cliquez sur **Créer des identifiants** > **ID client OAuth**.
3. Dans la liste **Type d'application**, choisissez **Téléviseurs et appareils à saisie limitée**.
4. Nommez le client (ex: `Kodi Client`) et cliquez sur **Créer**.
5. Une fenêtre affiche votre **ID client** (`youtube_id`) et votre **Code secret du client** (`youtube_secret`). Copiez-les pour les intégrer à votre configuration Pastebin.

---
