# Histoire dont tu es le héros

# Résumé :

Dans cette activité, crée une histoire interactive où le joueur choisit la suite de l’histoire. Pour se faire, utilise des conditions et affiche uniquement la suite de l’histoire dans le Terminal selon le choix de l’utilisateur. Ton histoire aura plusieurs fins possible mais l’utilisateur n’en verra qu’une.

# Domaine :

![programmation.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/89d0a8a9-5a49-4737-9cbd-867fc4f478a9/programmation.png)

# Difficulté :

![etoile.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/87bb1a61-62a4-41b0-9070-179ca3d67ecb/etoile.png)

# Langage de programmation :

- Au choix - le langage C est utilisé dans cette activité.

# Fonctionnalités du programme :

- Afficher une histoire dans le Terminal ;
- Proposer à l’utilisateur de faire un choix entre deux (ou plus) suite à l’histoire ;
- Récupérer le choix de l’utilisateur ;
- Afficher uniquement la partie de l’histoire choisie par l’utilisateur.

# Notions abordées dans cette activité :

## Programmation :

- Conditions
- Manipulations d’entrée / sortie dans le terminal

# Déroulement du programme :

1. Préparer une histoire à choix multiple sur une feuille. 
    1. Choisir le genre de l’histoire : Fantaisie, science-fiction, policier, horreur…
    2. Pour s’aider, commencer par faire un tableau sur feuille à 4 colonnes :
        
        
        | Personnage principal | Lieux | Antagoniste | Péripéties |
        | --- | --- | --- | --- |
        |  |  |  |  |
        
        Et y indiquer tout ce qui peut se trouver comme personnages principaux / lieux / antagonistes (méchants) / péripéties (changement de situations, actions) dans le genre d’histoire choisie.
        
    3. Écrire la situation initiale, puis à chaque choix proposant une péripétie différente, créer une branche et indiquer les points importants de l’action et de la suite de l’histoire. Pour que l’histoire soit interactive, il faut proposer des choix tout au long de l’histoire.
2. Créer un nouveau fichier `[histoire.c](http://histoire.py)` (ici, le langage C a été choisi, mais d’autres langages de programmation peuvent être utilisés comme Python, Java, C++…) ;
3. Préparer le fichier :
    
    ```c
    #include <stdio.h>
    #include <stdlib.h>
    
    int main(){
    	// On mettra l'histiore ici
    	// ...
    	// ...
    
    	// On laissera ce return 0; pour que le programme fonctionne.
    	return 0;
    }
    ```
    
4. Positionner son curseur à la ligne n°5 (ligne sous `int main(){`, à  la place des commentaires).
    1. Initialiser une variable pour stocker la réponse de l’utilisateur :
    `int reponse = 0;`
    2. Afficher la situation initiale dans le Terminal en utilisant la fonction `printf()`. Par exemple :
    `printf("Il était une fois...");`
    3. Pour proposer un choix à l’utilisateur, afficher ses options puis récupérer sa réponse. Par exemple :
    
    ```c
    printf("Choix 1 : Manger la pomme\n Choix 2 : Prendre la fuite.\n (Tapez 1 ou 2)\n");
    scanf("%d", &reponse); 
    ```
    
    1. Utiliser la réponse du joueur pour afficher le morceau d’histoire correspondant. Pour cela utiliser une condition. Par exemple :
        
        ```c
        if (reponse == 1){
        	printf("Miam la pomme...\n");
        }
        else{
        	printf("Je cooooouuuuurs !!\n");
        }
        ```
        
    2. Puis, répéter les instructions ***b. c.*** et ***d.* dans** chaque condition. C’est-à-dire, développer les deux branches de l’histoire séparément. 

# Améliorations :

- Proposer au lecteur recommencer l’histoire quand celle-ci prend fin.
- Stocker le nom du joueur dans une variable pour la réutiliser pour impliquer d’avantage le lecteur dans l’histoire.
- Pour une histoire plus visuelle et plus complexe, utiliser un outil comme `Ren’Py`.

# Ressources :

Description d’une fiction interactive : https://pixees.fr/introduction-aux-fictions-interactives/

Exemples de fictions interactives : [https://encrelin.fr/livres-dont-vous-etes-le-heros-jeunesse.html](https://www.heroyouare.fr/stories)
https://secret-santa-stephane.glitch.me/
