# utilisation de la commande vi
## Fichier
Soit le fichier `test.txt` contenant le texte suivant :
```
Mon fichier d'exemple contenant du texte.

Ceci est la première ligne.
Ceci est la deuxième ligne.
Ceci est la troisième ligne.

Merci d'utiliser l'éditeur Vi !
```

## Questions 
1. Ouvrez le fichier avec Vi.
      * La commande pour ouvrir un fichier existant dans Vi est : vi `test.txt`.

2. Placez le curseur à la fin du fichier.
      * Pour déplacer le curseur à la fin du fichier dans Vi, utilisez la commande : `G`.

3. Ajoutez une nouvelle ligne après la troisième ligne.
      * Pour insérer une nouvelle ligne après la position actuelle du curseur dans Vi, utilisez la commande : `o`.

4. Supprimez la deuxième ligne.
      * La commande pour supprimer une ligne entière dans Vi est : `dd`.

5. Recherchez la première occurrence du mot "utiliser" dans le fichier.
      * Pour rechercher un mot spécifique dans Vi, utilisez la commande : `/utiliser`.

6. Remplacez toutes les occurrences du mot "Ceci" par "Cela".
      * Pour remplacer une chaîne de caractères dans tout le fichier, utilisez la commande : :`%s/Ceci/Cela/g`.

7. Enregistrez les modifications et quittez Vi.
      * Pour enregistrer les modifications dans Vi, utilisez la commande : `:w`.
      * Pour quitter Vi, utilisez la commande : `:q`.

