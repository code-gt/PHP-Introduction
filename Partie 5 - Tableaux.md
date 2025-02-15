# PHP-Partie-5-Tableaux
Les Tableaux

## Petit tips 
En PHP, un tableau est une structure de données qui permet de stocker plusieurs valeurs dans une seule variable. 

C'est un peu comme une boîte où tu peux ranger plusieurs paires de chaussures.

Il existe deux types de tableaux en PHP : les tableaux indexés et les tableaux associatifs.

1. **Tableaux indexés** : Les valeurs sont stockées dans un ordre précis et chaque valeur a un index correspondant. **L'index commence toujours à 0**. Par exemple :

```php
$couleurs = ["rouge", "vert", "bleu"];
echo $couleurs[0]; // Affiche "rouge"
echo $couleurs[1]; // Affiche "vert"
echo $couleurs[2]; // Affiche "bleu"
```

2. **Tableaux associatifs** : Chaque valeur est associée à une clé. La clé peut être un nombre ou une chaîne de caractères. On parle ici d'un format clé => valeur
Par exemple :

```php
$ages = ["John" => 35, "Jane" => 27, "Bob" => 55];
echo $ages["John"]; // Affiche 35, On accède à la valeur qui est 35 grâce à la clé "John" 
```

Pour parcourir un tableau, on peut utiliser une boucle `foreach`. Par exemple :

```php
$ages = ["John" => 35, "Jane" => 27, "Bob" => 55];
foreach ($ages as $key => $age) {
    echo $key . "est agé de " . $age ." ans" . "<br>";  // Ici je crée une phrase en mettant bout à bout des chaines de caractère ainsi que des variables contenant une valeur, nous appelons ça la concaténation
}
```

Ce code affiche l'age de la personne sur une nouvelle ligne.

A ton tour d'utiliser des tableaux 😎!

### A vous de jouer ! 

## Exercice 1
Créer un tableau **months** et l'initialiser avec les valeurs suivantes :
- **janvier**
- **février**
- **mars**
- **avril**
- **mai**
- **juin**
- **juillet**
- **aout**
- **septembre**
- **octobre**
- **novembre**
- **décembre**

## Exercice 2
Avec le tableau de l'exercice 1, afficher la valeur de la troisième ligne de ce tableau.

## Exercice 3
Avec le tableau de l'exercice , afficher la valeur de l'index 5.

## Exercice 4
Avec le tableau de l'exercice 1, modifier le mois de **aout** pour lui ajouter l'accent manquant.

## Exercice 5
Créer un tableau associatif avec comme index le numéro des départements des Hauts de France et en valeur leur nom.

## Exercice 6
Avec le tableau de l'exercice 5, afficher la valeur de l'index 59.

## Exercice 7
Avec le tableau de l'exercice 5, ajouter la ligne correspondant au département de la ville de Reims.

## Exercice 8
Avec le tableau de l'exercice 1 et une boucle, afficher toutes les valeurs de ce tableau.

## Exercice 9
Avec le tableau de l'exercice 5, afficher toutes les valeurs de ce tableau.

## Exercice 10
Avec le tableau de l'exercice 5, afficher toutes les valeurs de ce tableau ainsi que les clés associés.  
Cela pourra être, par exemple, de la forme : **"Le département" + nom du département + "a le numéro" + numéro du département**

## Exercice 11 : Tableau des marques de voitures
Écrivez un script PHP qui utilise un tableau simple pour stocker quelques marques de voitures, puis affichez-les.

### Consignes :

1. Déclarez un tableau simple `$marquesVoitures` et y inclure six ou sept marques de voiture au choix.

2. Utilisez une boucle `foreach` pour afficher chaque marque de voiture dans une nouvelle ligne.

3. Affichez également le nombre total de marques de voitures présentes dans le tableau.

## Exercice 12 : Tableau des matériaux de Minecraft

Écrivez un script PHP qui utilise un tableau pour stocker quelques matériaux de Minecraft et leurs caractéristiques. Ensuite, vous devez afficher ces informations à l'aide d'une boucle.

### Consignes :

1. Déclarez un tableau associatif `$materiauxMinecraft` avec les éléments suivants :
   - "Bois" : "Obtient par coupe d'arbres"
   - "Pierre" : "Obtient par minage avec une pioche en pierre ou plus"
   - "Fer" : "Obtient par minage avec une pioche en fer ou plus"
   - "Diamant" : "Obtient par minage avec une pioche en diamant"
   - "Sable" : "Obtient en minant du sable"

2. Utilisez une boucle `foreach` pour afficher pour chaque matériau de Minecraft :
   - Le nom du matériau
   - La méthode pour l'obtenir
   - Exemple de sortie : "Le matériau Bois est obtenu par coupe d'arbres."

## Exercice 13 : Trier un tableau de prénoms
Écrivez un script PHP qui trie un tableau contenant des prénoms par ordre alphabétique et les affiche.

## Consignes :

1. Déclarez un tableau `$prenoms` contenantune dizaine de prénoms.

2. Utilisez la fonction PHP `sort()` pour trier le tableau par ordre alphabétique.

3. Affichez chaque prénom ou ville dans le tableau trié avec une boucle `foreach`.


# Exercices PHP - Tableaux Associatifs (Jeux Vidéo & Consoles)

## Exercice 1 : Création du tableau
Voici un tableau associatif $jeuxVideo contenant des jeux vidéo en clé et leur console respective en valeur.

```php
$jeuxVideo = [
    "The Legend of Zelda: Breath of the Wild" => "Nintendo Switch",
    "God of War" => "PlayStation 4",
    "Halo Infinite" => "Xbox Series X",
    "Super Mario Odyssey" => "Nintendo Switch",
    "Spider-Man" => "PlayStation 4",
    "Forza Horizon 5" => "Xbox Series X"
];
```

## Exercice 2 : Afficher la console d'un jeu spécifique  
À partir du tableau `$jeuxVideo`, affichez la console associée au jeu **"God of War"**.

## Exercice 3 : Ajouter un nouveau jeu au tableau  
Ajoutez au tableau `$jeuxVideo` le jeu **"Elden Ring"** et sa console **"PlayStation 5"**.  
Affichez ensuite le tableau mis à jour.

## Exercice 4 : Modifier la console d’un jeu  
Modifiez la valeur associée au jeu **"Halo Infinite"** pour la remplacer par **"PC"**.  
Affichez ensuite la nouvelle valeur pour vérifier la modification.

## Exercice 5 : Afficher tous les jeux vidéo  
À l'aide d'une boucle, affichez tous les jeux vidéo contenus dans le tableau `$jeuxVideo`.

## Exercice 6 : Afficher tous les jeux et leurs consoles  
Utilisez une boucle pour afficher chaque jeu avec sa console sous la forme :  
**"Le jeu [Nom du jeu] est disponible sur [Nom de la console]"**.

```plaintext
Le jeu The Legend of Zelda: Breath of the Wild est disponible sur Nintendo Switch
Le jeu God of War est disponible sur PlayStation 4
...
```

## Exercice 7 : Vérifier si un jeu est présent dans le tableau  
Créez une fonction qui prend un nom de jeu en paramètre et vérifie s'il est présent dans le tableau.  
- Si le jeu existe, affichez un message confirmant sa présence.  
- Sinon, affichez un message indiquant qu'il n'est pas dans la liste.  

Testez la fonction avec différents jeux. Vous aurez besoin ici de la méthode `array_key_exists()`.

## Exercice 8 : Trier le tableau par ordre alphabétique des jeux  
Utilisez `ksort()` pour triez le tableau `$jeuxVideo` en fonction du **nom des jeux** et affichez le tableau trié.

## Exercice 9 : Trier le tableau par ordre alphabétique des consoles  
Utilisez `asort()` pour triez le tableau `$jeuxVideo` en fonction du **nom des consoles** et affichez le tableau trié.
