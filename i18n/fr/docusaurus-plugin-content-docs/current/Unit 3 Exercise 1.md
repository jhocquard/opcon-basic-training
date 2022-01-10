---
sidebar_label: 'Unité 3 Exercice 1'
hide_title: 'false'
---

## Exercice 1: Créer un Profil (Rôle) et un compte utilisateur

##### Objectif:

Créez un **Profil** nommé ```Training```. Assurez-vous qu'il n'hérite PAS de privilèges.

Créez un **compte d'utilisateur** nommé ```Student1``` (Nom d'utilisateur complet: ```Student Number 1```.)

Copiez le mot de passe dans votre presse-papiers et remplacez le mot de passe copié par ```password1``` et confirmez.

Donnez à ```Student 1``` le profil ```Training```.

Vérifiez les privilèges du compte d'utilisateur en vous déconnectant d'Enterprise Manager et en vous reconnectant en tant que Student1. L'utilisateur doit avoir un accès limité aux menu qui peut être vérifié en choisissant Machine Status. Aucune machine ne doit être visible.


<div>
<video width="320" height="240" controls>
  <source src="videobasic/U3E1.mp4" type="video/mp4"></source>
Your browser does not support the video tag.
</video>
</div>

<details>

<summary>Cliquez pour obtenir des instructions étape par étape</summary>

1. Créer un profil:
  * Sous la rubrique Sécurité, double-cliquez sur **Profil**.
  * Cliquez sur le bouton **Ajouter** dans la barre d'outils Profil.
  * Dans le champ **Nom** saisissez ```Training```.
  * Dans le champ **Documentation**, saisissez : « Rôle à utiliser lors des exercices de sécurité ».
  * Sous Privilèges, assurez-vous que toutes les cases à cocher Hériter des Privileges sont décochées.
  * Cliquez sur le bouton Sauvegarder.
  * Fermez l'onglet « Profil ».
2. Créer un Compte Utilisateur:
  * Sous la rubrique **Sécurité**, double-cliquez sur **Comptes Utilisateurs**.
  * Cliquez sur le bouton Ajouter dans la barre d'outils Comptes Utilisateurs.
  * Dans le champ Nom, saisissez ```Student1```.
  * Dans le champ **Nom complet Utilisateur**, saisissez ```Student Number 1```.
  * Cliquez sur le bouton Sauvegarder dans la barre d'outils Comptes Utilisateurs.
  * Dans la fenêtre de Mot de passe défini, cliquez sur le bouton **Oui** pour placer le mot de passe dans votre presse-papiers.
  * Cliquez sur le bouton **Modifier Mot de passe Utilisateur** (côté droit de l'écran)
  * Cliquez avec le bouton droit de la souris dans le champ **Ancien Mot de passe** et collez l'ancien mot de passe.
  * Cliquez dans le champ **Nouveau Mot de passe** et saisissez ```password1``` (minuscules).
  * Cliquez à l'intérieur du champ **Confirmer Mot de passe** et saisissez ```password1``` (en minuscules).
  * Cliquez sur le bouton **OK**.
  * Sélectionnez le rôle de **Training** dans la liste **Non-autorisé**, puis cliquez sur la flèche verte (pointant vers la droite) pour placer Student1 dans le rôle de Training. Notez que le rôle de Training sera sous la liste Autorisé.
  * Cliquez sur le bouton Sauvegarder dans la barre d'outils Comptes Utilisateurs.
  * Fermez l'onglet Comptes Utilisateurs.
3. Vérifier les Privilèges des Comptes Utilisateurs:
  * Déconnectez-vous d'Enterprise Manager. Cliquez sur le bouton Déconnexion ou sélectionnez Déconnexion dans la barre de menus d'Enterprise Manager.
  * Cliquez sur **OK** pour confirmer que vous vous déconnectez.
  * À partir de l'écran de connexion OpCon/xps, tapez ```Student1``` dans le champ Nom Utilisateur  et ```password1``` dans le champ Mot de Passe. Cliquez sur Connexion.
  * Vérifiez les sujets auxquels l'utilisateur a accès :
    * Opérations
      * Vue Machines
      * Acquittement des Notification
    * Outils Externes
      * Import Export
      * Windows Tools
    * Information
      * Logs
    * Scripts
      * Repository
      * Runners
      * Types
    * Support
      * Support
      * Rapport d'incident
* Double-cliquez sur **Vue Machine** sous Opération
* Aucune machine ne devrait apparaître là.
* Fermez l'onglet Vue Machine, puis déconnectez-vous d'Enterprise Manager. Cliquez sur **OK** pour confirmer que vous vous déconnectez.
* À partir de l'écran de connexion OpCon/xps, laissez les champs Nom Utilisateur et Mot de Passe vides et cliquez sur **Connexion**.

</details>
