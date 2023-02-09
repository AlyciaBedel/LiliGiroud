# Lili Giroud 
Création d'un site de réservation en massage madérothérapeutique 
<br />

![bannière](https://user-images.githubusercontent.com/98737248/217847571-90405e58-9ae5-4018-955e-b3f1b41a9ab4.jpg)

## Pré-requis pour ouvrir le projet
1 - Disposer d'un serveur local (ex : MAMP ou XAMPP) et d'un éditeur de code (ex: VSCode) <br />
2 - Installer la dernière version de PHP 8.1 <br />
3 - Installer composer <br />
4 - Installer symfony   
<br />
## Pour installer le projet
1 - Ouvrir le dossier ou cloner le Git Hub sur votre éditeur de code

2 - Ouvrir le terminal de votre éditeur de code, taper : <br />
    *composer install* 

3 - Ouvrir le fichier __.env__ changé la __ligne 35__ avec votre identifiant et votre mot de passe de PHPMyAdmin <br />
    *db_User = Votre identifiant PHPMyAdmin* <br />
    *db_Password = Votre mot de passe PHPMyAdmin*

4 - Ouvrir PHPMyAdmin, installer la base de données qui se trouve dans le __dossier public > database__, c'est le fichier : *liligiroud.sql*   

5 - Dans le terminal de votre éditeur de code taper une par une les commandes suivantes : <br />
    *symfony console make:migration* <br />
    *symfony console doctrine:migrations:migrate*

6- Toujours dans le terminal, taper : <br />
    *symfony serve*

7- Le projet est prêt !     
<br />
## Identifiants pour se connecter et découvrir les interfaces attitrées
__Connexion avec un compte administrateur__ <br />
Email : administrateur@liligiroud.fr <br />
Mot de passe : test

__Connexion avec un compte utilisateur__ <br />
Email : utilisateurs@liligiroud.fr <br />
Mot de passe : test
<br />
<br />
## Version alternative du calendrier 
Afin de découvrir le calendrier alternative crée par la chef de projet : Léonore, rendez-vous sur [le git hub de dépôt](https://github.com/AlyciaBedel/CalendarLeonore.git) !

__Objectif du développement :__ <br /> 
Ce développement a pour objectif d’ajouter un calendrier permettant aux utilisateurs du site web de placer leur rendez-vous directement en “un clique”. Les clients peuvent voir les créneaux déjà réservés.

__Déroulement :__ <br /> 
Le client choisit son produit cela l'emmène sur la page calendrier, il choisi le jour qui l'intéresse et la plage horaire en cliquant sur le calendrier, un créneaux du nom de la prestation est alors créé, ce créneaux a une durée correspondant à la durée de la prestation, une fois le créneaux choisi il doit aller valider son panier

__Réalisation :__ <br />
Le calendrier bloque la réservation au horaire de travail défini par l’utilisateur.(non effectué)
le calendrier affiche un bloc de couleur sans le nom de la prestation, lorsque le client arrive sur la page calendrier et qu’il na pas lui meme effectuer cette reservation, une reservation sur ce bloc est impossible (non effectuer)
le client peut déplacer la réservation qu’il a créée à un autre horaire/autre jour disponible (fait)
les réservations du client sont sauvegarder sur la page calendrier puis dans la base de donnée (non effectuer)
Lorsque le créneaux est posé, une validation est attendue de sa part afin qu’il soit redirigé vers le panier.
