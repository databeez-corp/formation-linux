# Correction exercices Gestion des processus

1. Créez un script qui affiche les informations sur les processus en cours d'exécution toutes les 5 secondes. Utilisez la commande ps aux pour afficher les informations et la commande sleep pour mettre en pause le script pendant 5 secondes.
    * Pour vérifier que le script affiche bien les informations sur les processus toutes les 5 secondes, vous pouvez exécuter le script et vérifier que les informations sont affichées toutes les 5 secondes. Vous pouvez également utiliser la commande ps aux pour vérifier que les informations affichées par le script correspondent aux informations affichées par la commande ps aux.

2. Créez un script qui lance une boucle infinie et qui utilise la commande nice pour réduire la priorité de chaque tour de boucle. Utilisez la commande top pour vérifier que la priorité change effectivement.
    *  Pour vérifier que le script utilise bien la commande nice pour réduire la priorité de chaque tour de boucle, vous pouvez utiliser la commande top pour vérifier que la priorité du processus exécutant le script est effectivement réduite à chaque tour de boucle.

3. Lancez un processus qui prend beaucoup de temps à s'exécuter (par exemple, un grep sur un fichier volumineux) en arrière-plan avec la commande &. Utilisez la commande jobs pour vérifier que le processus est en cours d'exécution en arrière-plan, puis utilisez la commande fg pour le passer en avant-plan. Utilisez la commande bg pour le remettre en arrière-plan.
    * Pour vérifier que le processus est bien lancé en arrière-plan avec la commande &, vous pouvez utiliser la commande jobs pour vérifier que le processus est en cours d'exécution en arrière-plan. Utilisez la commande fg pour le passer en avant-plan. Utilisez la commande bg pour le remettre en arrière-plan. Vous pouvez vérifier que le processus est bien en cours d'exécution en arrière-plan en vérifiant que le curseur est revenu à la ligne de commande après l'avoir lancé.

4. Utilisez la commande pgrep pour trouver le numéro de processus d'un processus en cours d'exécution (par exemple, pgrep firefox), puis utilisez la commande kill pour tuer ce processus.
    * Pour vérifier que le processus a bien été tué avec la commande kill, vous pouvez utiliser la commande ps pour vérifier que le processus n'est plus en cours d'exécution.

5. Utilisez la commande top pour trouver un processus qui utilise beaucoup de ressources système, puis utilisez la commande kill pour tuer ce processus.
    * Pour vérifier que le processus a bien été tué avec la commande kill, vous pouvez utiliser la commande ps pour vérifier que le processus n'est plus en cours d'exécution.

6. Utilisez la commande htop pour lister les processus en cours d'exécution, trier par utilisation de la mémoire et identifier les processus qui utilisent le plus de mémoire, ensuite utilisez kill pour tuer ces processus.
    * Pour vérifier que les processus tués ont été effectivement tué, vous pouvez utiliser la commande ps pour vérifier que les processus tués ne sont plus en cours d'exécution

7. Utilisez la commande pgrep pour trouver les processus en cours d'exécution de plusieurs programmes (par exemple: firefox, chrome, sublime) et utilisez la commande killall pour tuer tous les processus trouvés.
    * Pour vérifier que les processus tués ont été effectivement tué, vous pouvez utiliser la commande ps pour vérifier que les processus tués ne sont plus en cours d'exécution.


# En général, il est important de vérifier que les commandes ont été utilisées correctement et que les résultats sont ceux attendus. Si vous rencontrez des problèmes, n'hésitez pas à demander de l'aide pour comprendre ce qui ne fonctionne pas.