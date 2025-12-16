# PHP-Partie-4-Fonctions

## Fonctions

Une fonction en PHP, c'est comme une machine qui fait une tâche spécifique. Tu lui donnes des ingrédients (les paramètres), elle fait son travail et te donne le résultat.


Voici comment on déclare une fonction en PHP :

```php
function nomDeLaFonction($parametre) {
    // Code à exécuter
    return $resultat;
}
```

Et voici comment on utilise une fonction :

```php
$resultat = nomDeLaFonction($ingredient);
```

Par exemple, on peut créer une fonction qui calcule la moyenne de deux nombres :

```php
function calculerMoyenne($nombre1, $nombre2) {
    $somme = $nombre1 + $nombre2;
    $moyenne = $somme / 2;
    return $moyenne;
}

$moyenne = calculerMoyenne(10, 20);
echo $moyenne; // Affiche 15
```

### A vous de jouer ! 

## Exercice 1
Faire une fonction qui retourne **true**.

## Exercice 2
Faire une fonction qui prend en paramètre une chaine de caractères et qui retourne cette même chaine.

## Exercice 3 : Concaténation
Faire une fonction qui prend en paramètre deux chaines de caractères et qui revoit la concaténation de ces deux chaines

## Exercice 4 : Comparaisons
Faire une fonction qui prend en paramètre deux nombres. La fonction doit retourner :
- **Le premier nombre est plus grand** si le premier nombre est plus grand que le deuxième
- **Le premier nombre est plus petit** si le premier nombre est plus petit que le deuxième
- **Les deux nombres sont identiques** si les deux nombres sont égaux

## Exercice 5
Faire une fonction qui prend en paramètre un nombre et une chaine de caractères et qui renvoit la concaténation de ces deux paramètres.

## Exercice 6 : Présentation
Faire une fonction qui prend trois paramètres : **le nom, le prénom et l'âge d'une personne**. Elle doit renvoyer une chaine de la forme :  
"Bonjour" + **nom** + **prénom** + ",tu as" + **age** + "ans".

## Exercice 7 : Vérification du genre et du rôle d'un personnage
Écrivez une fonction PHP qui prend deux paramètres : le genre et le rôle d'un personnage. Le genre peut être :
- Masculin
- Féminin

Les rôles peuvent être :
- Guerrier
- Mage
- Voleur
- Archer

### Consignes :

1. La fonction doit vérifier les deux paramètres (genre et rôle) et afficher un message spécifique en fonction de ces paramètres.
2. Voici les messages attendus en fonction des combinaisons :
   - "Vous êtes un guerrier masculin."
   - "Vous êtes un mage masculin."
   - "Vous êtes un voleur masculin."
   - "Vous êtes un archer masculin."
   - "Vous êtes une guerrière féminine."
   - "Vous êtes une magicienne féminine."
   - "Vous êtes une voleuse féminine."
   - "Vous êtes une archère féminine."
   - Si les paramètres ne correspondent pas à un genre ou rôle valide, afficher : "Genre ou rôle invalide."

## Exercice 8 : Somme
Faire une fonction qui prend en paramètre trois nombres et qui renvoit la somme de ces nombres.  
Tous les paramètres doivent avoir une valeur par défaut.

## Exercice 9 : Calcul du score total dans un jeu
Écrivez une fonction PHP qui calcule le score total d'un joueur en fonction du nombre de niveaux qu'il a franchis et du score obtenu à chaque niveau.

### Consignes :
1. Déclarez une fonction `calculerScore` qui prend deux paramètres :
   - `$niveaux` : le nombre de niveaux franchis.
   - `$scoreParNiveau` : le score obtenu à chaque niveau.
2. La fonction doit retourner le score total, qui est le produit du nombre de niveaux et du score par niveau.
3. Affichez le score total du joueur.

## Exercice 10 : Vérification des points de vie d'un personnage

Écrivez une fonction PHP qui vérifie si un personnage a encore des points de vie (HP) après avoir subi des dégâts.

### Consignes :

1. Déclarez une fonction `verifierPointsDeVie` qui prend deux paramètres :
   - `$pointsDeVie` : les points de vie actuels du personnage.
   - `$degats` : les dégâts subis par le personnage.
2. La fonction doit calculer les nouveaux points de vie du personnage en soustrayant les dégâts des points de vie.
3. Si les nouveaux points de vie sont supérieurs à 0, affichez "Le personnage a des points de vie restants."
4. Sinon, affichez "Le personnage est mort."

## Exercice 11 : Code promo
Créez une fonction qui applique une réduction sur un prix en fonction d'un code promo.  
Elle prend deux parametres - le prix et le code promo.  
Il existe trois codes promo différents (10%, 20%, 30%).  
Faire un switch/case  et retournez et affichez le prix après réduction.
