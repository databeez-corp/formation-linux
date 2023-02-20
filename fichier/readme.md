# recherche dans des fichiers, commande grep
1. Quelles sont les options de grep qui permettent d’obtenir des lignes de contexte (qui précèdent t/ou suivent la ligne où figure le mot) ?
2. Comment faire apparaître le numéro de la ligne où figure le mot recherché ? Que se passe-t-il quand on demande également des lignes de contexte ?
3. Comment faire pour afficher le nombre d’occurences du mot recherché ?
4. Comment faire pour que grep ignore la casse des caractères (différence entre majuscules et minuscules) dans sa recherche ?
5. Comment faire pour faire apparaître non pas les lignes où figurent le mot, mais les noms des fichiers ?
6. Comment faire apparaître les lignes où ne figurent pas le mot recherché ?
7. Comment faire apparaître les noms des fichiers ne contenant pas le mot recherché ?
8. Comment faire pour que `grep` ne recherche que les lignes où figure le mot tel quel, et non pas ses variantes ? Par exemple : on cherche le mot «travail», mais pas «travailleur» ou «travailler».
9. Comment faire pour chercher plusieurs mots à la fois en faisant apparaître les numéros des lignes ?
    * Chercher toutes les lignes commençant par «a» ou «A».
    * Chercher toutes les lignes finissant par «rs».
    * Chercher toutes les lignes contenant au moins un chiffre.
    * Chercher toutes les lignes commençant par une majuscule.
    * Chercher toutes les lignes commençant par «B», «E» ou «Q».
    * Chercher toutes les lignes finissant par un point d’exclamation.
    * Chercher toutes les lignes ne finissant pas par un signe de ponctuation (point, virgule, point- virgule, deux-points, point d’interrogation, point d’exclamation).
    * Chercher tous les mots contenant un «r» précédé de n’importe quelle lettre majuscule ou mi- nuscule.
    * Chercher tous les mots dont la seconde lettre est un «r».

#  les commandes head et tail
1. Affichez les 15 premières lignes du fichier /etc/hosts, les 15 dernières lignes, toutes les lignes à partir de la quinzième, les lignes 15 à 20.

    * Pour afficher les 15 premières lignes du fichier /etc/hosts :
        `head -n 15 /etc/hosts`
    * Pour afficher les 15 dernières lignes du fichier /etc/hosts :
        `tail -n 15 /etc/hosts`
    * Pour afficher toutes les lignes à partir de la quinzième ligne :
        `tail -n +15 /etc/hosts`
    * Pour afficher les lignes 15 à 20 :
        `sed -n '15,20p' /etc/hosts`

2. Pour récupérer les lignes 5 à 9 d'un fichier de 12 lignes :
    `sed -n '5,9p' fichier.txt`
3. Pour afficher la cinquième ligne d'un fichier :
    `sed -n '5p' fichier.txt`
    Ou avec la commande head :
    `head -n 5 fichier.txt | tail -n 1`

2. Récupérer les lignes 5 à 9 d’un fichier de 12 lignes.
3. Comment afficher la cinquième ligne d’un fichier ?


# Correction 
1. Les options de grep permettant d'obtenir des lignes de contexte sont :
    `-A num` : affiche num lignes après la ligne contenant le mot recherché
    `-B num` : affiche num lignes avant la ligne contenant le mot recherché
    `-C num` : affiche num lignes de contexte avant et après la ligne contenant le mot recherché
2. Pour faire apparaître le numéro de la ligne où figure le mot recherché, on utilise l'option `-n`. Si l'on demande également des lignes de contexte, le numéro de ligne s'affichera également pour ces lignes.
3. Pour afficher le nombre d'occurrences du mot recherché, on utilise l'option -c.
4. Pour que grep ignore la casse des caractères, on utilise l'option -i.
5. Pour faire apparaître non pas les lignes où figurent le mot, mais les noms des fichiers, on utilise l'option -l.
6. Pour faire apparaître les lignes où ne figurent pas le mot recherché, on utilise l'option -v.
7. Pour faire apparaître les noms des fichiers ne contenant pas le mot recherché, on utilise les options -l et -v combinées.
8. Pour que grep ne recherche que les lignes où figure le mot tel quel, et non pas ses variantes, on utilise l'option -w.
9. Pour chercher plusieurs mots à la fois en faisant apparaître les numéros des lignes, on utilise la syntaxe suivante : grep -n `'mot1\|mot2\|mot3'` fichier. Cette commande cherchera les mots mot1, mot2, et mot3 dans le fichier et affichera les numéros de ligne correspondants.
    * Chercher toutes les lignes commençant par `«a»` ou `«A»` : grep `'^[aA]'` fichier.
    *  Chercher toutes les lignes finissant par «rs» : grep 'rs$' fichier.
    *  Chercher toutes les lignes contenant au moins un chiffre : grep `'[0-9]'` fichier.
    * Chercher toutes les lignes commençant par une majuscule : grep `'^[A-Z]'` fichier.
    * Chercher toutes les lignes commençant par «B», «E» ou «Q» : grep `'^[BEQ]'` fichier.
    * Chercher toutes les lignes finissant par un point d’exclamation : grep `'!$'` fichier.
    * Chercher toutes les lignes ne finissant pas par un signe de ponctuation : grep `'[^.,;:?!]$'` fichier.
    * Chercher tous les mots contenant un «r» précédé de n’importe quelle lettre majuscule ou minuscule : grep `'[a-zA-Z]r[a-zA-Z]'` fichier.
    * Chercher tous les mots dont la seconde lettre est un «r» : grep `'\<.[rR]'` fichier. Note : le symbole `\<` indique le début d'un mot.