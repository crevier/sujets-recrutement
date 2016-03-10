SUJET MAISON : TEST JAVA
========================

En utilisant les librairies standards de JAVA, écrivez un composant de validation de données numériques:

Données en entrée 
-----------------

### Regles
Soit une liste de règles qui respecte la syntaxe suivante : 
nom_du_champ operateur valeur   (séparés par exactement un espace)
par ex. [ "A = 1", "B < 3", "C != 8",  "B = 1" ]

les opérateurs supportés sont = , > , < et  != 

### Les faits
Soit une collection de données (chaque champ ne peut avoir qu'une valeur) 
par ex. : 

"A" : 10

"B" : 22

"DATA" : 7

Données en sortie
-----------------

Une collection de champs associés à la liste des règles violées 
par ex. 

"A" : [ "A = 1"]

"B" : [ "B < 3", "B = 1"]

Exemples
--------

Entrées :

 - Règles : liste vide 
 - Données : "A" : 1 , "B" : 2 , "C" : 3	

Sortie : Collection vide

Entrées 	

 - Règles : [ "A = 1", "B < 3", "C !=  8",  "B > 1" ]
 - Données : Collection vide	

Sortie : Collection vide

Entrées : 
 
 - Règles : [ "A = 2", "B = 3 ]
 - Données : "A" : 1 , "B" : 2 , "C" : 3	

Sortie : "A" : [ "A = 2"], "B" : [ "B = 3"]

Précisions
----------

Fournissez des tests unitaires écris avec Junit4 pour vérifier votre implémentation. Vous êtes libre d’utiliser la version de JAVA que vous souhaitez, vous pouvez également utilisez un build manager. 

Important : Partez du principe que votre implémentation fera partie d'une librairie utilisée par d'autres personnes.
Vous n'avez pas de temps limite pour rendre le devoir, il est conseillé de ne pas se précipiter.

Livraison attendu : une archive contenant les sources du projet, et les instructions pour les utiliser.
