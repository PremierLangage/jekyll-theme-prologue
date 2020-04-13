---
title: Tour de PLaTon pour le C
author: Nicolas Borie
layout: post
---   

Voici un petit tour des contenus opérationnels pour le langage C. Ces
exercices de programmation ont déjà été utilisés pour renforcer les acquis
des élèves en programmation C. Ce sont principalement des exercices
utilisant un grader opérant une série de tests du type (arguments du
programme + entrée standard) --> (sortie standard). 


Les sorties standards sont auto-générées par un code source secret
établit par l'enseignant éditeur de l'exercice. À chaque soumission
d'élève, le code proposé est compilé puis exécuté si possible pour
faire une comparaison des sorties standards générés par le code de
élève comparé à celui du prof. Le test est valide si les sorties sont
exactement les mêmes (attention comparaison au retour chariot près
'\n').


Les exercices qui suivent ont été utilisés uniquement en autonomie
mais pour des élèves relativement avancés (en BAC+3). Ce sont des
élèves qui ont déjà un peu appris à apprendre. Les exercices sont
classé par thème, du plus simple au plus avancé. Les premiers
exercices sont triviaux, les derniers exercices sont relativement
difficiles.


Pour toute précision facilitant ré-utilisation, mutualisation, 
correction (énoncé, orthographe, ...), le mieux est encore de me 
joindre par mail à prénom point nom arobase u-pem point fr ou d'aller 
directement corriger les ressources dans l'éditeur de PLaTon.


Nicolas Borie.


### Premier programme, notion de programme C

* <a href="https://pl.u-pem.fr/filebrowser/demo/11075/" target="blank">Premier programme C</a>, ça commence par un "Hello World".
* <a href="https://pl.u-pem.fr/filebrowser/demo/11078/" target="blank">Ordonner quelques appels</a> de fonctions dans un **main**.
* Les <a href="https://pl.u-pem.fr/filebrowser/demo/11079/" target="blank">étapes de compilation</a> durant un appel à **gcc**.
* <a href="https://pl.u-pem.fr/filebrowser/demo/11080/" target="blank">Assembler deux fonctions</a> pour en fabriquer une troisième.
* Les <a href="https://pl.u-pem.fr/filebrowser/demo/11081/" target="blank">caractéristiques du langage C</a>.
* Écrire un <a href="https://pl.u-pem.fr/filebrowser/demo/11082/" target="blank">programme qui affiche ses arguments</a>.


### Les variables en C

* Les <a href="https://pl.u-pem.fr/filebrowser/demo/11083/" target="blank">caractéristiques des variables</a> en langage C.
* Identifier les <a href="https://pl.u-pem.fr/filebrowser/demo/11084/" target="blank">identificateurs légaux</a> pour des variables en C.
* Identifier des <a href="https://pl.u-pem.fr/filebrowser/demo/11085/" target="blank">right values</a> (valeur stockable) en C.
* Identifier des <a href="https://pl.u-pem.fr/filebrowser/demo/11086/" target="blank">left values</a> (conteneur affectable) en C.
* Ordonner quelques <a href="https://pl.u-pem.fr/filebrowser/demo/11087/" target="blank">taille mémoire de variables</a>.
* <a href="https://pl.u-pem.fr/filebrowser/demo/11088/" target="blank">Associer variable et objet modélisé</a>.


### Les types de base

* Lecture de quelques <a href="https://pl.u-pem.fr/filebrowser/demo/11089/" target="blank">types de base</a>.
* <a href="https://pl.u-pem.fr/filebrowser/demo/11090/" target="blank">Ordonner les tailles mémoires</a> des types entiers basiques.
* <a href="https://pl.u-pem.fr/filebrowser/demo/11091/" target="blank">Corriger une erreur de type 1</a>.
* <a href="https://pl.u-pem.fr/filebrowser/demo/11092/" target="blank">Corriger une erreur de type 2</a>.
* <a href="https://pl.u-pem.fr/filebrowser/demo/11093/" target="blank">Corriger une erreur de type 3</a>.
* <a href="https://pl.u-pem.fr/filebrowser/demo/11094/" target="blank">Articulation entiers caractères</a> pour les valeurs ASCII en C.


### Écrire des fonctions en C

* Écrire une fonction <a href="https://pl.u-pem.fr/filebrowser/demo/11095/" target="blank">mettant au cube</a> un entier passé par adresse.
* Écrire une fonction calculant <a href="https://pl.u-pem.fr/filebrowser/demo/11096/" target="blank">un polynôme</a> aléatoire (tirage dans une liste finie hardcodée).
* Rechercher la <a href="https://pl.u-pem.fr/filebrowser/demo/11097/" target="blank">première voyelle</a> dans une chaîne de caractère.
* Écrire une fonction qui opère un <a href="https://pl.u-pem.fr/filebrowser/demo/11098/" target="blank">incrément</a> (en argument) sur une variable entière passée par adresse.
* Écrire une fonction qui dessine un <a href="https://pl.u-pem.fr/filebrowser/demo/11099/" target="blank">triangle en ASCII art</a> à partir d'une taille donné.
* Écrire une fonction qui retourne le <a href="https://pl.u-pem.fr/filebrowser/demo/11100/" target="blank">maximum de trois entiers</a>.
* Écrire une fonction qui retourne le <a href="https://pl.u-pem.fr/filebrowser/demo/11101/" target="blank">minimum de trois entiers</a>.
* Écrire une fonction qui retourne la <a href="https://pl.u-pem.fr/filebrowser/demo/11102/" target="blank">moyenne de trois entiers</a>.
* Associer <a href="https://pl.u-pem.fr/filebrowser/demo/11103/" target="blank">prototypes et fonctionnalités</a> sur quelques exemples.
* Écrire une fonction qui calcule des <a href="https://pl.u-pem.fr/filebrowser/demo/11104/" target="blank">puissances entières</a>.


### Notion de tableaux

* Appliquer un <a href="https://pl.u-pem.fr/filebrowser/demo/11107/" target="blank">traitement (mettre au carré)</a> sur toutes les entrées d'un tableau.
* Calculer la <a href="https://pl.u-pem.fr/filebrowser/demo/11108/" target="blank">moyenne des éléments</a> d'un tableau d'entiers.
* Écrire une fonction qui <a href="https://pl.u-pem.fr/filebrowser/demo/11109/" target="blank">affiche un tableau</a> d'entiers.
* Écrire une fonction qui recherche <a href="https://pl.u-pem.fr/filebrowser/demo/11110/" target="blank">l'index de la première occurrence</a> d'un élément dans un tableau.
* Écrire une fonction qui <a href="https://pl.u-pem.fr/filebrowser/demo/11111/" target="blank">initialise un tableau à deux dimension</a> (tableau statique, non alloué dynamiquement et à tailles connues).
* Écrire une fonction qui <a href="https://pl.u-pem.fr/filebrowser/demo/11112/" target="blank">initialise avec les premiers carrés parfaits</a> un tableau d'entiers.
* Écrire une fonction qui calcule la <a href="https://pl.u-pem.fr/filebrowser/demo/11113/" target="blank">somme des éléments positifs</a> d'un tableau.


### Chaînes de caractères

* Écrire une fonction qui calcule la <a href="https://pl.u-pem.fr/filebrowser/demo/11114/" target="blank">longueur d'une chaîne</a> de caractères.
* Écrire une fonction qui compte les <a href="https://pl.u-pem.fr/filebrowser/demo/11115/" target="blank">occurrences d'un caractère</a> donné dans une chaîne.
* Écrire une fonction qui compte le <a href="https://pl.u-pem.fr/filebrowser/demo/11116/" target="blank">nombre de lettres minuscules</a> dans une chaîne de caractères.
* Écrire une fonction qui <a href="https://pl.u-pem.fr/filebrowser/demo/11117/" target="blank">encadre avec des dièses</a> une chaîne de caractères.
* Écrire une fonction qui <a href="https://pl.u-pem.fr/filebrowser/demo/11120/" target="blank">détecte une sous-chaîne</a> dans une chaîne.
* Écrire une fonction qui <a href="https://pl.u-pem.fr/filebrowser/demo/11122/" target="blank">détecte si une chaîne</a> représente un nombre entier relatif.
* Écrire un programme qui <a href="https://pl.u-pem.fr/filebrowser/demo/11123/" target="blank">détecte le plus long de ses arguments</a>.
* Écrire une fonction qui <a href="https://pl.u-pem.fr/filebrowser/demo/11124/" target="blank">met en majuscules</a> toutes les lettres d'une chaîne.


### Définir et utiliser des structures

* Définir une structure pour des <a href="https://pl.u-pem.fr/filebrowser/demo/11125/" target="blank">points entiers en dimension 2</a>.
* Définir une structure modélisant <a href="https://pl.u-pem.fr/filebrowser/demo/11126/" target="blank">une personne</a>.
* Définir une structure modélisant <a href="https://pl.u-pem.fr/filebrowser/demo/11127/" target="blank">un plateau de jeu</a> rectangulaire.
* Écrire une fonction calculant le <a href="https://pl.u-pem.fr/filebrowser/demo/11128/" target="blank">produit scalaire</a> de deux vecteurs en dimension 3.
* Définir une structure modélisant <a href="https://pl.u-pem.fr/filebrowser/demo/11129/" target="blank">les jours de la semaine</a>.
* Définir une structure d'<a href="https://pl.u-pem.fr/filebrowser/demo/11130/" target="blank">énumération pour des valeurs</a> précisées.
* Définir une structure pour modéliser une <a href="https://pl.u-pem.fr/filebrowser/demo/11131/" target="blank">couleur avec sa fonction d'allocation</a>.
* Exercice où l'on définit <a href="https://pl.u-pem.fr/filebrowser/demo/11132/" target="blank">deux structures simples emboîtées</a>.
* Définir un <a href="https://pl.u-pem.fr/filebrowser/demo/11133/" target="blank">tableau de structures</a> simples.


### Les macros et directives préprocesseur

* Manipuler la macro prédéfinie DATE pour faire une <a href="https://pl.u-pem.fr/filebrowser/demo/11134/" target="blank">fonction qui affiche la date de compilation</a> dans un programme.
* Établir quelques <a href="https://pl.u-pem.fr/filebrowser/demo/11135/" target="blank">macros constantes</a> pour un interface graphique.
* Définir une <a href="https://pl.u-pem.fr/filebrowser/demo/11136/" target="blank">macro à paramètre</a> calculant un carré.
* Mettre une <a href="https://pl.u-pem.fr/filebrowser/demo/11138/" target="blank">macro de sécurisation</a> pour éviter des appels multiples.
* Définir une macro à paramètres qui se substitue au <a href="https://pl.u-pem.fr/filebrowser/demo/11140/" target="blank">minimum des deux arguments</a>.
* Écrire une macro à paramètre <a href="https://pl.u-pem.fr/filebrowser/demo/11142/" target="blank">utilisant l'opérateur transformant en chaîne</a> un paramètre de macro.


### Notions d'entrées/sorties

* Faire un programme qui calcule la <a href="https://pl.u-pem.fr/filebrowser/demo/11143/" target="blank">somme de deux entiers</a> entrés au clavier.
* Faire un programme qui <a href="https://pl.u-pem.fr/filebrowser/demo/11144/" target="blank">récupère puis affiche une ligne complète</a> de l'entrée standard.
* Faire un programme qui retourne une <a href="https://pl.u-pem.fr/filebrowser/demo/11146/" target="blank">nouvelle structure</a> à partir d'information lu sur l'entrée standard.
* Faire un programme qui affiche le <a href="https://pl.u-pem.fr/filebrowser/demo/11149/" target="blank">produit de tous ses arguments</a> flottants.
* Faire un programme qui affiche le <a href="https://pl.u-pem.fr/filebrowser/demo/11150/" target="blank">nombre d'entiers non nuls</a> apparaissant sur l'entrée standard durant son exécution.
* Écrire un programme qui calcule le nombre de <a href="https://pl.u-pem.fr/filebrowser/demo/11151/" target="blank">caractères sur l'entrée standard</a>.
* Écrire un programme qui affiche tous les <a href="https://pl.u-pem.fr/filebrowser/demo/11152/" target="blank">mots reçus sur l'entrée standard de manière triée</a>.


### Récursivité en C

* Calculer la <a href="https://pl.u-pem.fr/filebrowser/demo/11153/" target="blank">factorielle d'un entier</a>.
* Calculer la <a href="https://pl.u-pem.fr/filebrowser/demo/11154/" target="blank">suite de Fibonacci</a> récursivement.
* Implémenter une fonction qui calcule les valeurs <a href="https://pl.u-pem.fr/filebrowser/demo/11155/" target="blank">d'Ackermann</a>.
* Calculer les <a href="https://pl.u-pem.fr/filebrowser/demo/11156/" target="blank">nombres binomiaux</a> récursivement.
* Calculer la <a href="https://pl.u-pem.fr/filebrowser/demo/11157/" target="blank">somme des chiffres</a> apparaissant dans un nombre.
* Implémenter un critère de <a href="https://pl.u-pem.fr/filebrowser/demo/11158/" target="blank">divisibilité par 7</a>.
* Faire un <a href="https://pl.u-pem.fr/filebrowser/demo/11159/" target="blank">égrenage récursif</a> des nombres entiers.
* Calculer des puissances entières via <a href="https://pl.u-pem.fr/filebrowser/demo/11160/" target="blank">l'exponentiation rapide</a>.
* Implémenter un algorithme calculant le <a href="https://pl.u-pem.fr/filebrowser/demo/11161/" target="blank">PGCD de deux entiers</a> seulement avec des soustractions et des divisions par deux (algo logarithmique comme Euclide).
* Algorithme déterminant une <a href="https://pl.u-pem.fr/filebrowser/demo/11162/" target="blank">zone contiguë</a> dans un tableau à deux dimensions (algo similaire à la coloration de zone).
* Coder le <a href="https://pl.u-pem.fr/filebrowser/demo/11163/" target="blank">problème du sac à dos</a> en langage C.
* Coder un <a href="https://pl.u-pem.fr/filebrowser/demo/11164/" target="blank">tri récursif</a> non rapide mais mieux que quadratique.


### Allocation dynamique

* Procéder à une <a href="https://pl.u-pem.fr/filebrowser/demo/11165/" target="blank">allocation simple de tableau</a> à une dimension.
* Déterminer le <a href="https://pl.u-pem.fr/filebrowser/demo/11166/" target="blank">nombre d'appels à malloc</a> à procéder suivant les situations.
* Rappel des <a href="https://pl.u-pem.fr/filebrowser/demo/11167/" target="blank">règles d'or d'usage de malloc</a> à Marne-la-Vallée (L3 et ESIPE à minima pour du C ansi).
* Déterminer <a href="https://pl.u-pem.fr/filebrowser/demo/11168/" target="blank">quand doit-on raisonnablement utiliser malloc</a>.
* Allouer correctement une <a href="https://pl.u-pem.fr/filebrowser/demo/11169/" target="blank">structure à deux chaînes</a> de caractères.
* Écrire une fonction d'<a href="https://pl.u-pem.fr/filebrowser/demo/11170/" target="blank">allocation de cellule</a> pour liste chaînée de double.
* Écrire une fonction d'<a href="https://pl.u-pem.fr/filebrowser/demo/11171/" target="blank">allocation pour liste chaînée de mots</a>.
* Écrire une fonction d'<a href="https://pl.u-pem.fr/filebrowser/demo/11172/" target="blank">allocation pour matrice carrée</a> d'entiers.
* Allouer un <a href="https://pl.u-pem.fr/filebrowser/demo/11173/" target="blank">tableau de chaînes de caractères</a> lues au clavier.


### Les opérateurs bit à bit

* Coder une fonction comptant le <a href="https://pl.u-pem.fr/filebrowser/demo/11174/" target="blank">nombre de bits à 1</a> dans une zone mémoire.
* Coder une fonction faisant un <a href="https://pl.u-pem.fr/filebrowser/demo/11175/" target="blank">miroir binaire</a> dans un octet.
* Coder une fonction déterminant la taille du <a href="https://pl.u-pem.fr/filebrowser/demo/15483/" target="blank">paquet de bits à 1</a> de poids faible dans un octet.
* Écrire une fonction comptant le <a href="https://pl.u-pem.fr/filebrowser/demo/11178/" target="blank">nombre d'alternances de bits</a> dans un entier long positif.
* Écrire une fonction qui <a href="https://pl.u-pem.fr/filebrowser/demo/11179/" target="blank">détecte le motif 1101</a> dans la donnée binaire d'un entier long positif.
* Écrire une fonction qui détermine la <a href="https://pl.u-pem.fr/filebrowser/demo/11180/" target="blank">taille du plus grand paquet de bits</a> consécutifs de même valeur dans une zone mémoire.
* Écrire une fonction qui opère un <a href="https://pl.u-pem.fr/filebrowser/demo/11182/" target="blank">miroir binaire</a> dans une zone mémoire.
