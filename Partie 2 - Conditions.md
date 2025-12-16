# PHP-Partie-2-Conditions
Les Conditions


Une condition en PHP, c'est comme un carrefour. Selon la direction que tu prends, tu arrives à une destination différente.

La structure de contrôle la plus courante pour les conditions en PHP est if...else.

Voici comment on utilise if...else :

```php
if ($condition) {
    // Code à exécuter si la condition est vraie
} else {
    // Code à exécuter si la condition est fausse
}
```

Et voici une variante avec elseif :

```php
if ($condition1) {
    // Code à exécuter si la condition1 est vraie
} elseif ($condition2) {
    // Code à exécuter si la condition1 est fausse et la condition2 est vraie
} else {
    // Code à exécuter si aucune des conditions n'est vraie
}
```

Par exemple, tu peux afficher un message différent selon l'âge de l'utilisateur :

```php
$age = 20;
if ($age < 13) {
    echo "Salut, petit!";
} elseif ($age < 18) {
    echo "Salut, ado!";
} else {
    echo "Salut, adulte!";
}
```

Tu peux aussi utiliser la syntaxe ternaire :

```php
// Déclaration d'une variable
$nombre = 10;

// Utilisation de l'opérateur ternaire
$message = ($nombre >= 20) ? "C'est plus de 20" : "C'est moins de 20";

// Affichage du résultat
echo $message;
```

Tu peux enfin utiliser la structure **switch/case**.

```php
$jour = "lundi";

switch ($jour) {
    case "lundi":
        echo "Aujourd'hui, c'est lundi.";
        break;
    case "mardi":
        echo "Aujourd'hui, c'est mardi.";
        break;
    case "mercredi":
        echo "Aujourd'hui, c'est mercredi.";
        break;
    default:
        echo "Jour non reconnu.";
}
```

Explications : On déclare une variable `$jour` et lui attribue la valeur "lundi".  
La structure `switch` compare cette variable avec les différents `case` ("lundi", "mardi", "mercredi"). Dès qu'une correspondance est trouvée, le code dans ce `case` est exécuté, puis on utilise `break` pour sortir de la structure `switch`.  
Si aucune correspondance n'est trouvée, le `default` est exécuté.

### A vous de jouer ! 

## Exercice 1 : if/else
Créer une variable **age** et l'initialiser avec une valeur.  
Si l'âge est supérieur ou égale à 18, afficher **Vous êtes majeur**. Dans le cas contraire, afficher **Vous êtes mineur**.

## Exercice 2 : boolean
Créer une variable **isEasy** de type booléan et l'initialiser avec une valeur.  
Afficher **C'est facile!!** si c'est vrai. Dans le cas contraire afficher **C'est difficile !!!**.  
**Bonus :** L'écrire de deux manières différentes.

## Exercice 3 : if/elseif/else
Créer une variable **temperature**  
Afficher **Trop froid** si < 0, **Frais** si ≥ 0 et ≤ 15, - **Tempéré** si > 15 et ≤ 25, - **Chaud** si > 25.

## Exercice 4 : switch/case
L'échelle de Richter est un outil de mesure qui permet de définir la magnitude de moment d'un tremblement de terre.  
Cette échelle va de 1 à 9.  
Créer une variable **magnitude**. Selon la valeur de **magnitude**, afficher la phrase correspondante.  

Magnitude   |   Phrase
------      |    ---
1           |   Micro-séisme impossible à ressentir.
2           |   Micro-séisme impossible à ressentir mais enregistrable par les sismomètres.
3           |   Ne cause pas de dégats mais commence à pouvoir être légèrement ressenti.
4           |   Séisme capable de faire bouger des objets mais ne causant généralement pas de dégats.
5           |   Séisme capable d'engendrer des dégats importants sur de vieux bâtiments ou bien des bâtiments présentants des défauts de construction. Peu de dégats sur des bâtiments modernes.
6           |   Fort séisme capable d'engendrer des destructions majeures sur une large distance (180 km) autour de l'épicentre.  
7           |   Séisme capable de destructions majeures à modérées sur une très large zone en fonction de la distance.
8           |   Séisme capable de destructions majeures sur une très large zone de plusieurs centaines de kilomètres.
9           |   Séisme capable de tout détruire sur une très vaste zone.  

Gérer tous les cas.  
**Utiliser une structure switch/case**

## Exercice 5
Traduire ce code avec des if et des else :  


    <?php
      echo ($gender != 'Homme') ? 'C\'est une développeuse !!!' : 'C\'est un développeur !!!';
    ?>

## Exercice 6
Traduire ce code avec des if et des else :  


    <?php
      echo ($age >= 18) ? 'Tu es majeur' : 'Tu n\'es pas majeur';
    ?>
    
## Exercice 7
Traduire ce code avec des if et des else :  


    <?php
      echo ($isOk == false) ? 'c\'est pas bon !!!' : 'c\'est ok !!';
    ?>
    
## Exercice 8
Selon l’âge de l’utilisateur, afficher un message différent dynamiquement. La variable `$message` sera déclaré vide au départ de l'exercice. 

Moins de 12 ans → tarif enfant,  
12 à 17 ans → tarif réduit,  
18 à 64 ans → tarif normal,  
≥ 65 ans → tarif senior.  

## Exercice 9 : Vérification de mots de passe

Écrivez un script PHP qui vérifie si deux mots de passe saisis sont identiques.

### Consignes :
1. Déclarez deux variables `$password1` et `$password2` pour stocker les mots de passe.
2. Comparez-les en utilisant une structure conditionnelle.
3. Si les mots de passe sont identiques, affichez : "Les mots de passe correspondent.".
4. Sinon, affichez : "Les mots de passe ne correspondent pas.".

## Exercice 10 : Calculateur de notes

Écrivez un script PHP qui attribue une mention en fonction d'une note sur 20.

### Consignes :
1. Déclarez une variable `$note` pour stocker la note d'un étudiant (par exemple, 16).
2. Utilisez une structure `if/else if/else` pour attribuer les mentions suivantes :
    - **"Excellent"** : si la note est supérieure ou égale à 16.
    - **"Bien"** : si la note est comprise entre 12 et 15 inclus.
    - **"Assez Bien"** : si la note est comprise entre 10 et 11 inclus.
    - **"Insuffisant"** : si la note est inférieure à 10.
3. Affichez la mention correspondante.

## Exercice 11 : Déterminer le type de Pokémon

Écrivez un script PHP qui, en fonction du nom d'un Pokémon, affiche son type. Par exemple, si le nom du Pokémon est "Bulbizarre", le script doit afficher "Plante / Poison". Utilisez une structure **switch/case**.

### Consignes :
1. Déclarez une variable `$pokemon` pour stocker le nom d'un Pokémon (par exemple, "Pikachu").
2. Utilisez une structure `switch` pour tester différentes valeurs de `$pokemon`.
3. Pour chaque Pokémon, affichez son type avec un message comme : "Pikachu est un Pokémon de type Électrique."
4. Si le Pokémon n'est pas dans la liste, affichez un message indiquant "Pokémon inconnu."

## Exercice 12 : Météo

Afficher un message différent selon la météo.
Déclarez une variable `$meteo` avec les valeurs possibles : "soleil", "pluie", "neige", "vent"
Utilisez un **switch/case**

Affichez des messages personnalisés :

 - soleil → "Sortez les lunettes 😎"
 - pluie → "Prenez un parapluie ☔"
 - neige → "Attention ça glisse ❄️"
 - vent → "Couvrez-vous bien"
 - défaut → "Météo inconnue".
