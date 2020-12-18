# Exercices

## 1 - Scripts de gestion des comptes utilisateurs

Faire un script de gestion des utilisateurs, qui doit permettre : 

- de créer des utilisateurs
- de modifier des utilisateurs
- de supprimer des utilisateurs
- de voir tous les utilisateurs
- de faire une recherche sur l'existence d'un utilisateur en particulier
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

    #Création de variable semblable à un input
    $choose = Read-Host -prompt('Voulez vous faire : 1 = créer un utilisateur, 2 = modifier un utilisateur, 3 = supprimer un utilisateur, 4 = voir tout les utilisateurs,  5 = faire un recherche sur un utilisateur en particulier')


    #Création d'utilisateur 
    If ($choose -eq 1)
    {
        $name = Read-Host -prompt('Quel nom voulez vous donner à votre nouvel utilisateur ?')
        New-LocalUser -Name $name 
    }
    #Modification du nom de l'utilisateur
    elseif ($choose -eq 2)
    {
        $nametochange = Read-Host -prompt ("Quelle nom d'utilisateur voulez-vous changer")
        $namechange = Read-Host -prompt('Quel nouveau nom voulez vous donner à votre nouvel utilisateur ?')
        Rename-LocalUser -Name $nametochange -NewName $namechange 
    }
    #Suppression d'un utilisateur
    elseif ($choose -eq 3){
        $removename = Read-Host -Prompt("Quelle est le nom de l'utilisateur que vous voulez supprimer ?")
        Remove-LocalUser -Name $removename
    } 
    #Afficher tout les utilisateurs
    elseif ($choose -eq 4){
        Get-LocalUser
    }
    #Afficher les informations sur un utilisateur en particulier
    else {
        $infoname = Read-Host -Prompt("Quelle est le nom de l'utilisateur où vous voulez rechercher des informations")
        Get-LocalUser -Name $infoname
    }

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 2 - Exercice d'installation automatique d'un serveur web Apache

Créer un script qui va automatiquement installer et paramétrer un serveur web Apache. Le script devra pouvoir : 

- installer Apache
- permettre d'activer ou désactiver des modules apache
- permettre de lister les modules apaches actifs
- permettre de lister les modules apaches non actifs, mais disponibles
- permettre de créer un nouveau répertoire pour accueillir un nouveau site web (avec la création des virtualhost automatique)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 3 - Créer un script permettant de réaliser des sauvegardes automatique de votre serveur web Apache

Le script devra permettre d'automatiser la sauvegarde de l'ensemble des sites internet, ainsi que des virtualhosts et de la configuration d'apache. Cette sauvegarde devra être compressée dans un seul et même dossier.

Le script devra ensuite pouvoir redéployer l'ensemble des sites, Vhost & configurations à partir d'une sauvegarde.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 4 - Créer un annuaire téléphonique

Le script devra permettre la gestion d'un annuaire téléphonique. Il devra inclure les fonctionnalités suivantes : 

- ajouter un contact (nom + tel + mail)
- modifier un contact
- voir la liste de tous les contacts (triés par ordre alphabétiques grâce à leurs noms et n'afficher que leurs noms)
- voir le détail d'un contact grâce à son nom
- retrouver le nom d'un contact grâce à son adresse mail
- retrouver le nom d'un contact grâce à son téléphone
- supprimer un contact

L'ensemble des informations devront être enregistrées dans un fichier texte
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 5 - Créer un agenda

Le script devra permettre de gérer un agenda. Il devra inclure les fonctionnalités suivantes : 

- ajouter un évènement (date + heure + nom + durée)
- voir la liste des évènements par ordre chronologique
- modifier un évènement
- supprimer un évènement

L'ensemble des informations devront être enregistrées dans un fichier texte
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
[Retour au sommaire](https://github.com/Malo44490/Powershell/blob/main/README.md#sommaire)
