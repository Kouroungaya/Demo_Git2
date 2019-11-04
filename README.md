# Demo_Git2

Demo de l'utilisation d'un repo git de project Unity 3D

## Comment Insérer un projet Unity dans un dossier git déjà existant

( unity ne supporte pas de créer un nouveau projet dans un dossier déjà existant ).

Deux solutions possible :

1. Création du projet Unity avec son dossier en sous-dossier du projet git.
    1. Création du projet Unity avec comme paramêtre :
        * le Dossier du projet git local dans le champ Location.
        * le nom du futur sous-dossier contenant le projet unity dans le projet git dans le champ Project Name.
    2. Sauvegarde du projet unity et sortie de l'editeur Unity.
    3. Création ou déplacement du fichier .gitignore unity dans le sous-dossier projet unity
    4. commit des sous-dossiers et fichier généré indexé suivant le filtre .gitignore .
    5. push du projet dans github.
2. Création du projet dans un dossier temporaire puis copy des sous-dossiers du projet temporaire et fichiers généré dans le dossier projet git
    1. Création du projet Unity avec comme paramêtre :
        * la racine du futur dossier temporaire dans le champ location.
        * le nom du futur dossier temporaire contenant le projet unity dans le champ Project Name.
    2. Sauvegarde du projet unity et sortie de l'editeur Unity.
    3. copy des sous-dossiers et fichier généré par l'éditeur Unity dans le projet git
    4. ouverture du projet unity dans le projet git, sauvegarde et sortie ( pour verifié si l'opération précédente s'est bien passé).
    5. Création du fichier .gitignore unity à la racine du projet git ( si pas déja fait à la création projet avec GITHUB )
    6. commit des sous-dossiers et fichier généré indexé suivant le filtre .gitignore .
    7. push du projet dans github.
    8. effacement du dossier temporaire.
