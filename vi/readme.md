# Correction : utilisation de la commande vi
1. Utilisez `VI` pour créer un fichier de texte simple qui contient votre nom, votre âge et votre ville natale. Ensuite, utilisez les commandes de base pour ajouter, supprimer et modifier le contenu du fichier.
    *  vous pouvez utiliser la commande `:sort` pour trier les lignes du fichier dans l'ordre alphabétique. Assurez-vous de sauvegarder le fichier après avoir effectué la modification en utilisant la commande `:wq`.

2. Utilisez `VI` pour créer un fichier de script shell qui affiche un message de bienvenue à l'utilisateur en utilisant la commande echo.
    * utiliser les variables d'environnement pour afficher un message de bienvenue personnalisé. Par exemple, en utilisant la commande `echo "Bonjour $USER, bienvenue sur votre système` pour afficher un message de bienvenue pour l'utilisateur actuel.

3. Utilisez `VI` pour éditer un fichier de configuration pour changer les paramètres d'un service spécifique sur votre système (par exemple, changer le port utilisé par un serveur web).
    * utiliser les commandes de base de VI pour rechercher et remplacer les paramètres spécifiques dans le fichier de configuration. Assurez-vous de sauvegarder le fichier après avoir effectué la modification en utilisant la commande `:wq`.
    * par exemple changer le port d'un fichier httpd.conf `:%s/port = 80/port = 8080/g` Nouveau port 8080 remplace l'ancien port 80, cela permet de sauvegarder les modifications en utilisant la commande : `:wq`


4. Utilisez `VI` pour créer un fichier de script qui automatise la sauvegarde de fichiers dans un emplacement spécifique en utilisant la commande cp.
    * utiliser la commande `cp` pour copier les fichiers à l'emplacement spécifié, puis utiliser un cron pour automatiser la sauvegarde à des intervalles spécifiés.
    * `cp /chemin/vers/fichiers /chemin/vers/emplacement/de/sauvegarde`

5. Utilisez `VI` pour ouvrir un fichier de journal et rechercher des entrées d'erreur spécifiques en utilisant la commande grep.
    * utiliser la commande `grep` pour rechercher des entrées d'erreur spécifiques dans le fichier de journal. Il est important de vérifier que les entrées d'erreur ont été correctement
    * `grep "erreur" /chemin/vers/fichier/de/journal`

