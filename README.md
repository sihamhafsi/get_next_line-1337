# get_next_line-1337
--------------------------------------------------------------------------------------------------------------------------------------------------------------
# partie obligatoire
Nom de la fonction : get_next_line </br>
Prototype : char *get_next_line(int fd);</br>
Rendre les fichiers : get_next_line.c, get_next_line_utils.c, get_next_line.h</br>
Paramètres : fd : Le descripteur de fichier à lire </br>
Valeur de retour : ligne de lecture : comportement correct</br>
NULL : il n'y a rien d'autre à lire ou une erreur s'est produite</br>
Fonctions externes : read, malloc, free</br>
Description : Ecrire une fonction qui retourne une ligne lue depuis un descripteur de fichier </br>
• Des appels répétés (par exemple, en utilisant une boucle) à votre fonction get_next_line() devraient vous permettre de lire le fichier texte pointé par le descripteur de fichier, une ligne à la fois.</br>
• Votre fonction doit renvoyer la ligne qui a été lue. S'il n'y a rien d'autre à lire ou si une erreur s'est produite, elle doit renvoyer NULL.</br>
• Assurez-vous que votre fonction fonctionne comme prévu à la fois lors de la lecture d'un fichier et lors de la lecture à partir de l'entrée standard.</br>
• Veuillez noter que la ligne renvoyée doit inclure le caractère \n de fin, sauf si la fin du fichier a été atteinte et ne se termine pas par un caractère \n. </br>
• Votre fichier d'en-tête get_next_line.h doit au moins contenir le prototype de la fonction get_next_line().</br>
• Ajoutez toutes les fonctions d'assistance dont vous avez besoin dans le fichier get_next_line_utils.c . </br>
# partie bonus
• Développez get_next_line() en utilisant une seule variable statique.</br>
• Votre get_next_line() peut gérer plusieurs descripteurs de fichiers en même temps.
Par exemple, si vous pouvez lire à partir des descripteurs de fichier 3, 4 et 5, vous devriez pouvoir lire à partir d'un fd différent par appel sans perdre le fil de lecture de chaque descripteur de fichier ou renvoyer une ligne à partir d'un autre fd.</br>
Cela signifie que vous devriez pouvoir appeler get_next_line() pour lire depuis fd 3, puis fd 4, puis 5, puis encore une fois 3, encore une fois 4, et ainsi de suite.</br>
