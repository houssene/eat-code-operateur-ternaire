#Eat code - Opérateur tenaire en PHP

Dans ce poste je vous montrerais comment simplifier l’écriture des vos contions. J’utiliserais PHP dans ce cas de figure.

###Condition simple

En principe une condition en PHP comme dans tout autre langage de programmation débute par “if”

```` PHP 
<?php
if(condition){
  // action
}else {
  // seconde action
}
````

Prenons en exemple une personne __A__ qui pour âge __30 ans__ et une seconde âgé de __20 ans__

```` PHP
<?php

$peopleA = 30;
$peopleB = 20;
 

if($peopleA === $peopleB) {
	return "true";
}else {
 	return "false";
}

````

Le résultat est __false__ car, 30 est supérieur à 20 on est bien d'accord essayons de simplifier tout ceci

```` PHP
 ....
 
 if($peopleA === $peopleB) 
 	return "true";
 else
 	return "false"; 
 	
OR

 if($peopleA === $peopleB) return "true";
 else return "false";	
````

Là vous vous dites qu'il n'y a pas une grande différence allons plus loin grâce à l'opérateur ternaire

````PHP
...
return ($peopleA === $peopleB) ? "true" : "false";
````

Pour tous ces cas de figure le résultat est pareil __false__ à vous d'utiliser la bonne méthode au cours de votre projet.
