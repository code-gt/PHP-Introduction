# PHP-Partie-3-Boucles
Les Boucles

Une boucle en PHP, c'est comme un tour de manège. Tant que le manège tourne, tu fais le même tour encore et encore.

Il y a plusieurs types de boucles en PHP, mais les plus courantes sont `for` et `foreach`.

Voici comment on utilise une boucle `for` :

```php
for ($i = 0; $i < 10; $i++) {
    echo $i;
}
```

Cette boucle affiche les nombres de 0 à 9 
La boucle tourne et affiche la valeur de du variable $i à chaque tour.

À la fin de chaque tour la variable $i comptabilise un tour de plus (0 puis 1 puis 2 etc etc...) 
Tant qui $i est toujours inférieur à 10 nous allons refaire un tour jusqu'à que la condition soit valide


Pour un exemple avec `foreach`, disons que tu as une liste de films à regarder et que tu veux les afficher un par un :

```php
$films = ["Star Wars", "Harry Potter", "Le Seigneur des Anneaux"];

foreach ($films as $film) {
    echo $film . "<br>";
}
```

Cette boucle parcourt le tableau `$films` et affiche chaque film sur une nouvelle ligne.

### A vous de jouer ! 

## Exercice 1
Créer une variable et l'initialiser à 0.  
Tant que cette variable n'atteint pas 10, il faut :
- l'afficher
- l'incrementer

## Exercice 2
Créer deux variables. Initialiser la première à 0 et la deuxième avec un nombre compris en 1 et 100.  
Tant que la première variable n'est pas supérieure à 20 :
- multiplier la première variable avec la deuxième
- afficher le résultat
- incrementer la première variable

## Exercice 3
Créer deux variables. Initialiser la première à 100 et la deuxième avec un nombre compris en 1 et 100.  
Tant que la première variable n'est pas inférieure ou égale à 10 :
- multiplier la première variable avec la deuxième
- afficher le résultat
- décrémenter la première variable

## Exercice 4
En allant de 200 à 0 avec un pas de 12, afficher le message **Hop**.

## Exercice 5 : Somme des entiers
Écrivez un script PHP qui calcule et affiche la somme de tous les entiers de 1 à 100 en utilisant une boucle `for`.

## Exercice 6 : Table de multiplication
Écrivez un script PHP qui affiche la table de multiplication de 5.
Affichez chaque résultat sous la forme : "5 x 1 = 5", "5 x 2 = 10", etc.

## Exercice 7 : Compte à rebours personnalisé

Créez une variable `$depart` initialisée à 10.  
Utilisez une boucle while.  
Décrémentez-la jusqu’à atteindre 0.  
À la fin, affichez le message **"Décollage !"**.  

## Exercice 8 : Carré des nombres
Écrivez un script PHP qui affiche le carré des nombres de 1 à 10.
