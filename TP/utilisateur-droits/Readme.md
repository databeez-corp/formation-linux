# TP Gestion des Utilisateurs et Droits

## Objectifs
*	Gestion des utilisateurs et des groupes sous linux
*	Gestion des droits d'accès aux dossiers ou aux fichiers sous linux
## Configuration initiale
Ce TD est à réaliser avec une station sous linux ubuntu ou debian dans virtualbox.
## Prérequis
* Pratique de base de linux, pratique du shell et des commandes de base, pratique d'un éditeur de texte Vi


## Exercice 1: gestion des utilisateurs et des groupes
1.	creéz les utilisateurs `user1`, `user2`, `user3` et `user4` de mots de passe respectif: `passeruser1`, `passeruser2`, `passeruser3` et `passeruser4` à l'aide de la commande useradd.
2.	Quel est le shell de connexion de vos utilisateurs ?Changer celui de user3 pour `/bin/sh`
3.	Créez un groupe nommé databeez à l'aide de la commande addgroup. Consultez le fichier `/etc/group` pour trouver son gid et la liste des utilisateurs y appartenant.
4.	ajoutez les utilisateurs `user1` et `user2` au groupe  databeez en utilisant la commande useradd.
