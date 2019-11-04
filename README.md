# Demo_Git2

Demo de l'utilisation d'un repo git de project Unity 3D

## Comment Insérer un projet Unity dans un dossier git déjà existant?

( unity ne supporte pas de créer un nouveau projet dans un dossier déjà existant ).

Deux solutions possible :

1. Création du projet Unity avec son dossier en sous-dossier du projet git local.
    1. Création du projet Unity avec comme paramêtre :
        * le Dossier du projet git local dans le champ Location.
        * le nom du futur sous-dossier contenant le projet unity dans le projet git dans le champ Project Name.
    2. Sauvegarde du projet unity et sortie de l'éditeur Unity.
    3. Création ou déplacement du fichier .gitignore pour unity dans le sous-dossier projet unity
    4. Commit des sous-dossiers et fichiers généré indexé suivant le filtre .gitignore .
    5. Push du projet dans github.
2. Création du projet dans un dossier temporaire puis copie des sous-dossiers du projet temporaire et fichiers généré dans le dossier projet git local
    1. Création du projet Unity avec comme paramêtre :
        * la racine du futur dossier temporaire dans le champ location.
        * le nom du futur dossier temporaire contenant le projet unity dans le champ Project Name.
    2. Sauvegarde du projet unity et sortie de l'éditeur Unity.
    3. Copie des sous-dossiers et fichiers généré par l'éditeur Unity dans le dossier du projet git
    4. Ouverture du projet unity dans le projet git, sauvegarde et sortie ( pour vérifié si l'opération précédente s'est bien passé).
    5. Création du fichier .gitignore pour unity à la racine du projet git ( si non fait à la création projet avec GITHUB )
    6. Commit des sous-dossiers et fichiers généré indexé suivant le filtre .gitignore .
    7. Push du projet dans github.
    8. éffacement du dossier temporaire.
