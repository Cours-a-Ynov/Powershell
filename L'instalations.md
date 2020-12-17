# L'installation

- Comment installer Powershell sur Linux plus precisement Debian 10 :
-Nous allons le faire via un dépôt de packages dans Debian 10 :

1. Télécharger le répertoire clés GPG de Microsoft :
wget https://packages.microsoft.com/config/debian/10/packages-microsoft-prod.deb

2. Inserer le répertoire clés GPG de Microsoft :
sudo dpkg -i packages-microsoft-prod.deb

3. Il faut mettre à jour la liste des produits :
sudo apt-get update

4. Installer Powershell :
sudo apt-install -y powershell

5. Lancer powershell :
pwsh

- Si vous n'avez pas Powershell d'installer sur votre ordinateur sous windows, il suffit de suivre les instructions qui vont être donné prochainement.

1. Aller sur votre moteur de recherche. Taper dans la barre de recherche : Windows Management Framework ‘la version de vous souhaité’ (Exemple : Windows Framework 5)

2. Vérifier avant de télécharger le framework, qu’il est bien compatible à votre système d’exploitation.

3. Télécharger

4. Une fois télécharger, chercher l’application dans la barre de recherche windows en bas à droite

5. Exécuter Windows Powershell en tant qu’administrateur, sinon certaines commandes ne fonctionneront pas

Si certaines commandes powershell ne fonctionnent pas même en tant qu’administrateur :
Panneau de confinguration (dans la barre de recherche) – Compte utilisateur – Compte utilisateur – Modifier les paramètres de contrôles du compte utilisateur – baisser la jauge aux plus bas

[Retour au sommaire](https://github.com/Malo44490/Shell-Powershell/blob/main/README.md)
