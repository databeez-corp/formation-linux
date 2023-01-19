# Enoncé exercices Gestion des processus

1. Créez un script qui affiche les informations sur les processus en cours d'exécution toutes les 5 secondes. Utilisez la commande ps aux pour afficher les informations et la commande sleep pour mettre en pause le script pendant 5 secondes.

2. Créez un script qui lance une boucle infinie et qui utilise la commande nice pour réduire la priorité de chaque tour de boucle. Utilisez la commande top pour vérifier que la priorité change effectivement.

3. Lancez un processus qui prend beaucoup de temps à s'exécuter (par exemple, un grep sur un fichier volumineux) en arrière-plan avec la commande &. Utilisez la commande jobs pour vérifier que le processus est en cours d'exécution en arrière-plan, puis utilisez la commande fg pour le passer en avant-plan. Utilisez la commande bg pour le remettre en arrière-plan.

4. Utilisez la commande pgrep pour trouver le numéro de processus d'un processus en cours d'exécution (par exemple, pgrep firefox), puis utilisez la commande kill pour tuer ce processus.

5. Utilisez la commande top pour trouver un processus qui utilise beaucoup de ressources système, puis utilisez la commande kill pour tuer ce processus.

6. Utilisez la commande htop pour lister les processus en cours d'exécution, trier par utilisation de la mémoire et identifier les processus qui utilisent le plus de mémoire, ensuite utilisez kill pour tuer ces processus.

Utilisez la commande pgrep pour trouver les processus en cours d'exécution de plusieurs programmes (par exemple: firefox, chrome, sublime) et utilisez la commande killall pour tuer tous les processus trouvés.