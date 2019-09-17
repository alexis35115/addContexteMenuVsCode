# Procédure à suivre pour ajouter Visual Studio Code dans le menu contextuel après l'installation

## Gains

Ça permet d'ouvrir rapidement un répertoire directement dans Visual Studio code via le menu contextuel.

## Avoir l'option dans le menu contextuel lors de l'installation

Pour avoir Visual Studio Code dans le menu contextuel directement suite à l'installation, il faut s'assurer de cocher les options suivantes :

![alt text](https://raw.githubusercontent.com/alexis35115/addContexteMenuVsCode/master/img/addContextMenuDuringInstallation.png)

## Étapes à suivre dans le cas où l'option n'est pas présente dans le menu contextuel

### Télécharger le fichier "addContextMenuVsCode.reg"

Se rendre à l'[adresse](https://github.com/alexis35115/addContexteMenuVsCode) et cliquer sur le bouton "Clone or download" et dans le menu cliquer sur l'option "Download ZIP". Se référer à l'image ici-bas :

![alt text](https://raw.githubusercontent.com/alexis35115/addContexteMenuVsCode/master/img/CloneOrDownloadExample.PNG)

### Identifiant l'endroit de l'installation de Visual Studio Code

Voici la procédure à suivre pour savoir à quel endroit se trouve votre installation de Visual Studio Code.

![alt text](https://raw.githubusercontent.com/alexis35115/addContexteMenuVsCode/master/img/PropertiesVsCode.PNG)

- Faire un clic droit sur l'icône de Visual Studio Code et cliquer sur "Propriétés"
- Copier le nom du dossier qui se trouve dans "Cible". Par exemple, C:\Users\garonmichauda\AppData\Local\Programs\Microsoft VS Code\

### Modifier le fichier registre

Ensuite, il faut dézipper le dossier téléchargé à partir de Github et faire un clic droit sur le fichier "addContextMenuVsCode.reg" et cliquer sur "Modifier".

Dans l'éditeur de texte, il faut chercher et remplacer "C:\\Users\\garonmichauda\\AppData\\Local\\Programs\\Microsoft VS Code\\" et remplacer par l'endroit de votre installation. Prendre note qu'il faut mettre "\\" au lieu de "\".

Sauvegarder le fichier.

### Exécuter un le fichier registre

Revenir dans le dossier dézippé et double cliquer sur le fichier "addContextMenuVsCode.reg" et accepter les modifications.

## Validation

Après avoir suivi les étapes, vous devriez voir dans le menu contextuel des dossiers l'option "Open Folder in Code". Voir l'image ici-bas :

![alt text](https://raw.githubusercontent.com/alexis35115/addContexteMenuVsCode/master/img/Validation.PNG)

## Prochaine étape

Lorsque j'aurai du temps, je vais créer un script powershell pour automatiser le tout.
