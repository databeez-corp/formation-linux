# TP Scripting shell
Votre entreprise a besoin d’une solution sécurisée permettant aux personnels de la supervision d’intervenir dans un cadre maîtrisé sur les serveurs et d'effectuer certaines actions. 

## Le besoin
Votre responsable vous demande de développer un outil destiné aux superviseurs. Ils pourront effectuer quelques actions d’administration ainsi que les premiers diagnostics avant de faire intervenir le personnel d’astreinte.

Le personnel doit pouvoir se connecter aux serveurs via un compte générique : `supervision`.

Lorsque l’utilisateur se connecte, un menu est proposé, lui permettant 
* De gérer les utilisateurs 
    * afficher le nombre d’utilisateurs du serveur et les afficher sous formes de 2 listes 
        1. les utilisateurs systèmes,
        2. les utilisateurs standards ;

    * afficher les groupes du serveur et les afficher sous forme de 2 listes 
        1. les groupes systèmes,
        2. les groupes standards ;

    * créer un groupe : le superviseur devra fournir le `GID` ;

    * créer un utilisateur : le superviseur devra fournir l’`UID`, le `GID`, etc. ;

    * changer le mot de passe d’un utilisateur ; l’utilisateur sera forcé de changer son mot de passe lors de sa prochaine connexion.

* De gérer les services 
    * relancer le serveur `apache` ;
    * relancer le serveur `mysql`.

* De tester le réseau :

    * Afficher les informations du réseau (Adresse IP, masque, passerelle, serveurs DNS) ;
    * Tester le réseau (localhost, ip, passerelle, serveur distant, résolution DNS).

* Actions diverses :
    * redémarrer le serveur ;
    * quitter le script (l’utilisateur est déconnecté).

Les actions du superviseur devront être renseignées dans les journaux systèmes.

## Consignes
* Les scripts sont stockés dans `/opt/supervision/scripts/` ;

* Effectuer tous les tests que vous jugerez nécessaires ;

* Découper le code en plusieurs scripts ;

* Utiliser des fonctions pour organiser le code ;

* Commenter le code.