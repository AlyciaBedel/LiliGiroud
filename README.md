# LiliGiroudProjet-4
Création d'un site de réservation en massage madérothérapeutique 

## PREREQUIS POUR OUVRIR LE PROJET : 
1 - Installer la dernière version de PHP 8.1
2 - Installer composer   
3 - Installer symfony   


## POUR INSTALLER LE PROJET 
1 - Ouvrir le dossier ou cloner le Git Hub sur votre éditeur de code (ex: Visual Studio Code)  

2 - Ouvrir le terminal de votre éditeur de code, taper :  
*composer install* 

3 - Ouvrir le fichier __.env__ changé la __ligne 35__ avec votre identifiant et votre mot de passe de PHPMyAdmin.  
*db_User = Votre identifiant PHPMyAdmin*  
*db_Password = Votre mot de passe PHPMyAdmin*

4 - Ouvrir PHPMyAdmin, installer la base de données qui se trouve dans le __dossier public > database__, c'est le fichier : *liligiroud.sql*   

5 - Dans le terminal de votre éditeur de code taper une par une les commandes suivantes :     
    *symfony console make:migration*. 
    *symfony console doctrine:migrations:migrate*

6- Toujours dans le terminal, taper :    
    *symfony serve*

7- Le projet est prêt !     


## IDENTIFIANTS POUR SE CONNECTER ET DÉCOUVRIR LES INTERFACES ATTITRÉES
__Connexion avec un compte administrateur__. 
Email : administrateur@liligiroud.fr. 
Mot de passe : test. 

__Connexion avec un compte utilisateur__. 
Email : utilisateurs@liligiroud.fr. 
Mot de passe : test. 


## VERSION ALTERNATIVE DU CALENDRIER. 
