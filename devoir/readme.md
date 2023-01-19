# Devoir pratique de fin de Formation Linux

Ce devoir permet de tester vos aptitudes à utiliser les commandes linux de base pour manipuler les fichiers et les utilisateurs mais aussi vos aptitudes à manager un environnement dockorisé.

<u>Contexte : </u> Vous êtes administrateur systeme dans une entreprise informatique de la place. Votre principale role est d'assurer la maintenant du SI et la mise en services des produits informatique de l'entreprise. 

Dans votre entreprise, vous recevez souvent des clients qui se plaignent sur la qualité des services de l'entreprise :

* Serveurs trop lents;
* Les requetes prennent beaucoup de temps à envoyer une reponse;
* Les serveurs qui tombent en panne souvent ;
* etc.

Vous en tant que chef de service, vous decidez de faire plusieurs manipulations afin de resoudre ou proposer des pistes de solutions aux differents problemes des clients. 

## 1.  Manipulation de logs

Vous disposez d'un serveur web Apache. Ce serveur enregistre les informations des clients connectés à votre serveur à tout moment.

Le fichier de log `log-server.log` se trouve dans le dossier file.

Votre travail consite à :
* Determiner le nombre de ligne du fichier log
* Determiner le nombre de clients connecté au serveur
* Determiner le nombre de clients qui ont accedé au serveur avec succes
* Determiner le nombre de client qui ont accedé au serveur avec un message d'erreur

## 2. Detection d'intrusion

Apres manipulation, on se rend compte qu'un client se connecte sur le post du server( localhost, `127.0.0.1`). Ce client est un hacker de hau niveau.

* Determiner le nombre de fois que le hacker s'est connecté au serveur
* Identifier l'url appelé par le hacker.

Un autre diagnostique a montré que le hacker utilise son navigateur `Safari`

* Determiner le nombre de fois que le hacker s'est connecté avec son navigateur `safari`
* Determiner le systeme et la version de l'OS du hacker

Un auditeur du SI vient de publier son rapport. Dans ce rapport, il specifie que le serveur est sonvent attaqué par des senegalais.

* Determiner le nombre d'attaque subit par le serveur

## 3. Script shell

L'administration vous demande d'etablir un script leur permettant de manipuler les logs.

Sur la base de toutes les commandes effectuees, créer un script bash qui prend en entree le scrip et donne en sortie toutes les informations citées au-dessus.

## 4. Image docker(Bonus)

Vous vous rendez compte que partager un script bash n'est trop prratique dans un milieu professionnel. 

Donc vous devez créer une image docker dans laquelle vous mettez le script crée dans la section 3. 

Ensuite vous publiez votre image dans votre compte sur docker hub.