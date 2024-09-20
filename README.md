# GameJam 2024 : ChronoSpy

## Scénario:
Game en 2D sur un labyrinthe, un agent aux pouvoirs temporels spéciaux doit parcourir 2 niveaux avec le but de désamorcer une bombe, tout en échappant aux gardes du laboratoire. Sur les deux niveaux, l’agent aura un objectif différent, avec le but final d’échapper du labo dans un temps imparti qu’il devra manipuler pour y arriver
Le chronometre est le timing de la bombe. Ce chronomètre sera ralenti par des bonus pris par l’agent.

En récupérant un bonus placé sur la labyrinth pendant une petite durée ( 10 secondes )

## Premier niveau:
L’agent devra en premier lieu, parcourir le labyrinthe et de récupérer un code lui permettant de désamorcer la bombe placée au 2ème niveau, tout en échappant aux ennemis.
Un checkpoint est placé dans le labyrinthe qui permet de sauvegarder l'instant et de pouvoir y revenir en appuyant sur C.
Si les ennemies sont alertés (l’agent arrive dans leur champs de vision), tous les ennemis poursuivent le joueur.
Si l’agent récupère le code il se dirige vers le deuxième niveau
S’il se fait toucher par un agent, il perd.


## Deuxième niveau:
Le but de ce niveau sera de désamorcer la bombe. C’est à dire que l’agent va parcourir le labyrinthe, toujours en échappant aux enemies de la même manière et d’aller chercher la bombe.
Dès que la bombe est désamorcée, une porte apparait dans le labyrinthe lui permettant de s’échapper.


## Gestion de temps:
La gestion du temps arrivera avec les capacités du joueur qui vont être :
L'arret du temps
Remonter le temps à un checkpoint sauvegarde
