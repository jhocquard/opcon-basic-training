---
sidebar_label: 'Unite 3 Exercice 2'
hide_title: 'false'
---

## Exercice 2: privilèges machine

##### Objectif:

Autorisez les **privilèges de machine** au rôle ```Training```.

Vérifiez que les privilèges machine ont été autorisés en vous déconnectant d'Enterprise Manager et en vous reconnectant en tant que ```Student1```.

Notez que ```Student1``` n'aura toujours pas les privilèges pour voir les machines dans l'administration, mais pourra voir la machine ```SMATraining``` dans Machine Status (mais ne pourra pas changer l'état de la communication ou éditer la machine).


<div>
<video width="320" height="240" controls>
  <source src="videobasic/U3E2.mp4" type="video/mp4"></source>
Your browser does not support the video tag.
</video>
</div>

<details>

<summary>Cliquez pour obtenir des instructions étape par étape</summary>

1. Sous la rubrique **Security> Privileges**, double-cliquez sur **Machine Privileges**.
2. Dans la liste déroulante **Select Role**, sélectionnez le rôle de **Training**.
3. Sous la liste Revoked, cliquez sur la machine ```SMATraining```, puis sur la flèche verte (pointant vers la droite) pour placer ```SMATraining``` sous la liste **Autorisé**.
4. Fermez l'onglet Machine Privileges.

:::note Remarque
l'utilisateur ```Student1``` (qui se trouve sous le rôle de **Training**) peut désormais sélectionner cette machine pour exécuter des Jobs lors de leur configuration dans l'écran Job Details
:::

5. Déconnectez-vous d'Enterprise Manager. Cliquez sur le bouton Logout ou sélectionnez Logout dans la barre de menus d'Enterprise Manager.
6. Cliquez sur OK pour confirmer que vous vous déconnectez.
7. À partir de l'écran de connexion OpCon / xps, tapez ```Student1``` dans le champ **Username** et ```password1``` dans le champ **Password**. Cliquez sur **Login**.
8. Notez que l'utilisateur n'a toujours pas le privilège de voir les **machines** sous la rubrique **Administration**
9. Double-cliquez **Machine Status** sous Operations
10. Cliquez avec le bouton droit sur la machine ```SMATraining``` et vérifiez que l'utilisateur ne peut pas modifier l'état de communication de la machine.
11. Essayez de sélectionner **Edit Machine**. Vous recevrez un message d'erreur.
12. Fermez l'onglet Machine Status, puis déconnectez-vous d'Enterprise Manager. Cliquez sur OK pour confirmer que vous vous déconnectez.
13. À partir de l'écran de connexion OpCon / xps, laissez les champs **Username** et **Password** et cliquez sur **Login**.

:::caution Remarque
l'utilisateur ```Student1``` ne peut mettre à jour aucune information pour aucune machine dans la configuration, mais pourra sélectionner cette machine lors de la configuration des Jobs SI les privilèges pour cette machine sont configurés.
:::

</details>