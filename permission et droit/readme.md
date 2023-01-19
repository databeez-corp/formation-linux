# Solution : droits d’accès, liens
1. Changez les droits d’un fichier fic1 pour que tous ceux de votre groupe puissent écrire de- dans.
    * `chmod 660 fic1`
2. Donnez en une seule ligne le droit d’exécution à tous les utilisateurs d’un fichier script qui n’a jusqu’alors que des droits standards (-rw-r–r–).
    * `chmod +x script.sh`
3. Le fichier toto a les droits suivants:-rwxr–r–. Modifiez-en les droits en une ligne de commande de sorte que le propriétaire n’ait plus que le droit de lecture.
    * `chmod 400 toto`

4. Modifier les droits du fichier toto (-rwxr–r–) de sorte que le groupe et les autres utilisateurs aient les mêmes droits que le propriétaire.
    * `chmod 755 toto`
5. Quelle option permet de modifier récursivement les droits d’un répertoire et des fichiers qu’il contient ?
    * `chmod -R 755 répertoire`
6. Quelle option de mkdir permet de créer un répertoire en spécifiant les droits sur ce répertoire ?
    * `mkdir -m 755 nouveau_répertoire`
7. Affichez et interprétez les droits de /usr/games/.
    * `ls -l /usr/games/`
8. Vous avez chez vous un répertoire tmp/ qui contient un fichier bidon. Créez un lien physique sur tmp/bidon appelé blo, dans votre répertoire d’accueil (HOME). Comparez les contenus de tmp/bidon et de blo. Que contient blo ?
    * `ln /chemin/vers/tmp/bidon ~/blo`
    *  Le contenu de tmp/bidon et de blo sera le même.
9. Même question avec un lien symbolique.
    * `ln -s /chemin/vers/tmp/bidon ~/blo`
    * Le contenu de tmp/bidon et de blo sera le même.
10. Quelles sont les différences entre les liens durs et les liens symboliques ?
    * Les liens durs (hard links) créent une nouvelle référence au fichier cible, tandis que les liens symboliques (soft links ou symbolic links) créent un raccourci vers le fichier cible. Les liens durs ne dépendent pas de l'emplacement du fichier cible, tandis que les liens symboliques dépendent de l'emplacement du fichier cible.
11. Dans quel cas ne peut-on pas faire de lien physique ? Que faut-il faire ?
    * On ne peut pas faire de lien physique sur un lien symbolique ou une boîte aux lettres. Il faut utiliser un lien symbolique dans ces cas-là.
12. Quel est l’effet de chmod sur un lien ? 
    * La commande chmod modifie les droits sur le lien lui-même, mais pas sur le fichier cible.