# snake-blockade

snake-blockade consiste en un **projet de fin d'année** pour l'Université UPEC (2023-2024) en Java. Le but du jeu est d'être le meilleur serpent des deux présents dans l'arène.

## snake-engine

snake-engine est le moteur du jeu : il gère les coups, s'assure que le joueur est en droit (ou non) de réaliser tels ou tels coups, et permet aussi la communication protocole
(voir dans la catégorie LAN).

## snake-renderer

Le snake-renderer transforme les données de l'arène données par le moteur de jeu en une interface graphique fonctionnelle.

## snake-fx

snake-fx fait le lien avec Java Swing (librairie permettant l'utilisation des fonctionnalités graphiques de Java) et permet l'affichage
en clair de l'arène, des serpents, des menus, ... au joueur.

## snake-game

snake-game assure la fonctionnalité du projet en associant les trois piliers ci-dessus mentionnés.

# Modes de jeu

### Inputs de base

Les mouvements pouvant être perpétrés par le joueur se basent sur les inputs des touches des joueurs :
- Flèche du haut : mouvement vers le haut
- Flèche du bas : mouvement vers le bas
- Flèche de droite : mouvement vers la droite
- Flèche de gauche : mouvement vers la gauche

### Comment perdre ?

Lors d'une partie, un des joueurs peut perdre de différentes manières :
- Rentrer dans son propre corps 
- Rentrer dans un obstacle
- Sortir de l'arène
- Rentrer dans le serpent adverse


## Mode 1 contre 1

Ce mode de jeu se joue au tour par tour sur un même ordinateur. Chaque joueur réalise un **input sur le clavier** pour 
permettre le mouvement de son serpent.

## Mode IA

Ce mode de jeu se joue en local : le joueur choisit d'être joueur 1 ou joueur 2 et joue avec une IA qui est en capacité 
de calculer quelques coups à l'avance. 

## Mode LAN

Ce mode de jeu utilise une API REST afin de permettre à notre IA de jouer contre d'autres IA utilisant le même protocole.

