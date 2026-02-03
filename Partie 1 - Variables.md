# les variables en PHP

Une variable en PHP, c'est comme une boîte dans laquelle tu peux stocker une valeur. Tu peux donner un nom à cette boîte pour pouvoir la retrouver plus tard.

Voici comment on déclare une variable en PHP :

```php
$nomDeLaVariable = valeur;
```

Et voici comment on affiche le resultat d'une variable sur une page :

```php
echo $nomDeLaVariable;
```

Par exemple, on peut créer une variable qui stocke ton âge :

```php
$age = 20;
echo $age; // Affiche 20
```

On peut aussi créer une variable qui stocke ton prénom :

```php
$prenom = "John";
echo $prenom; // Affiche "John"
```

Et on peut même utiliser des variables pour faire des calculs :

```php
$nombre1 = 10;
$nombre2 = 20;
$somme = $nombre1 + $nombre2;
echo $somme; // Affiche 30
```

## Les types de données dans les variables

Une variable est un conteneur pour stocker une valeur. Cette valeur peut être de différents types :

- **Entiers** (`int`) : Ce sont des nombres sans décimales. Par exemple, `$age = 20;`.
- **Flottants** (`float`) : Ce sont des nombres avec des décimales. Par exemple, `$prix = 9.99;`.
- **Chaînes de caractères** (`string`) : Ce sont des séquences de caractères. Par exemple, `$nom = "John";`.
- **Booléens** (`bool`) : Ce sont des valeurs de vérité. Ils ne peuvent être que `true` ou `false`. Par exemple, `$estMajeur = true;`.
- **Tableaux** (`array`) : Ce sont des collections de valeurs. Par exemple, `$couleurs = array("rouge", "vert", "bleu");`.
- **Objets** (`object`) : Ce sont des instances de classes. Par exemple, `$voiture = new Voiture();`.
- **NULL** : C'est une valeur spéciale qui représente une variable sans valeur. Par exemple, `$inconnu = NULL;`.

On déclare une variable avec le symbole `$` suivi du nom de la variable. On peut ensuite utiliser cette variable dans notre code en la rappelant par son nom.


### A vous de jouer ! 

## Exercice 1
Créer une variable **name** et l'initialiser avec la valeur de votre choix.  Afficher son contenu.

## Exercice 2
Créer trois variables **lastname** , **firstname** et **age** et les initialiser avec les valeurs de votre choix.  **Attention** age est de type entier.  Afficher leur contenu.

## Exercice 3
Créer une variable **km**. L'initialiser à 1. Afficher son contenu.  
Changer sa valeur par 3. Afficher son contenu.  
Changer sa valeur par 125. Afficher son contenu.

## Exercice 4
Créer une variable **name** et l'initialiser avec la valeur de votre choix.  
Afficher : "Bonjour" + **name** + ", comment vas tu ?".

## Exercice 5
Créer trois variables **lastname** , **firstname** et **age** et les initialiser avec les valeurs de votre choix.  **Attention** age est de type entier.  
Afficher : "Bonjour" + **lastname** + **firstname** + ",tu as" + **age** + "ans".

## Exercice 6
Créer 3 variables.  
Dans la première mettre le résultat de l'opération **3 + 4**.  
Dans la deuxième mettre le résultat de l'opération **5 * 20**.  
Dans la troisième mettre le résultat de l'opération **45 / 5**.  
Afficher le contenu des variables.

## Exercice 7 : Manipulation de chaînes de caractères

Déclarez deux variables :  
- `$prenom` contenant votre prénom  
- `$nom` contenant votre nom  

1. Concaténez les deux variables dans une nouvelle variable `$nomComplet` en ajoutant un espace entre les deux.  
2. Affichez la longueur de la chaîne `$nomComplet` à l'aide de la fonction `strlen()`.  

   Exemple :  
   ```php
   $texte = "Bonjour";  
   echo strlen($texte); // Affiche 7
   ```
3. Affichez `$nomComplet` en majuscules à l'aide de la fonction `strtoupper()`.  

   Exemple :  
   ```php 
   $texte = "hello";  
   echo strtoupper($texte); // Affiche HELLO
   ```
   
## Exercice 8 : Les opérateurs mathématiques
   
1. Déclarez deux variables `$nombre1` et `$nombre2` contenant des nombres entiers.  
2. Calculez et affichez :  
   - Leur **somme**  
   - Leur **produit**  
3. Si `$nombre2` est différent de 0, calculez et affichez :  
   - Leur **division**  
   - Le **reste** de leur division (modulo)  

Assurez-vous de vérifier que `$nombre2` n'est pas égal à 0 avant de tenter une division ou un modulo.

## Exercice 9 : Les constantes et les variables

1. Déclarez une constante nommée `PI` avec la valeur `3.14159`.
  
   Exemple :  
   ```php
   define("NOM_CONSTANTE", valeur);
   ```
2. Déclarez une variable $rayon pour stocker un rayon de cercle (par exemple, 5).

3. Calculez et affichez :

 - Le périmètre du cercle
 - L'aire du cercle

4. Affichez les résultats avec un message descriptif.

   Exemple de sortie attendue :
   ```php
   Le périmètre du cercle est de 31.4159.
   L'aire du cercle est de 78.53975.
   ```

## Exercice 10 : Calcul du prix TTC 

1. Déclarez une constante `TVA` avec la valeur `0.2` (pour représenter 20 % de TVA).  

   Exemple :  
   ```php
   define("TVA", 0.2);
   ```
2. Déclarez une variable $prixHT pour stocker un prix hors taxes (par exemple, 50).

3. Calculez le prix TTC en utilisant la formule :

   ```java
   prix TTC = prix HT + (prix HT * TVA)
   ```

4. Affichez les résultats avec un message descriptif.

   Exemple de sortie attendue :
   ```java
   Le prix HT est de 50.
   Le prix TTC avec une TVA de 20% est de 60.
   ```
