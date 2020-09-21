---
title: Exos système Unix
author: Nicolas Borie
layout: post
---

# Ressources autour d'un cours de système en L2 informatique


Toujours dans le but de présenter un évantail d'exercices réalisables 
sous la plateforme PLaTon, voici un ensemble de ressources produites 
dans l'urgence du confinement du second semestre de l'année 
universitaire 2019-2020.

Les ressources qui vont suivre ont été créées pour un cours intitulé 
**architecture des systèmes informatiques** donné en L2 parcours 
informatique. Cette matière introduit un cours de programmation système
donné en L3 informatique. Il s'agit donc de présenter les mécanismes
des systèmes d'exploitation ainsi que de les utiliser mais pas de les 
programmer.

Systématiquement, chacun des templates qui suivent a été déclinés en 
une demi-douzaine d'exercices. Ainsi, avec 5 QCMs, une vingtaine 
d'exercices sur les commandes bash, une dizaine de circuits logiques 
de taille différente, 6 fonctions à tester pour certifier le bon 
fonctionnement, etc... On arrive à ventiller tout le programme et 
toutes les technos avec un simple navigateur web. 

Effectivement, un des problèmes des élèves durant le confinement est 
que tout le monde ne possède pas un ordinateur à la maison avec un 
système Unix d'installé. De ce fait, certains élèves avaient du mal à 
pouvoir réaliser les exercices des TP de système chez eux. 
Sous PLaTon, les sandbox tournent sur une distribution Debian de Linux. 
Ainsi, la plupart de ces exercices fonctionnent sur tout support 
numérique quelques soit les systèmes d'exploitation (PC windows, 
Linux et OS X ; smartphone et tablette android, iOS ou windows-phone).
 

## Des QCMs

Des QCMs, relativement standards, mais qui portent sur des notions 
de systèmes ou de données ici par exemple:

<a href="https://pl.u-pem.fr/filebrowser/demo/25605/" target="_blank">
Quizz sur les données binaires</a> 

Ces QCMs réutilisent un template produit par un enseignant en 
mathématiques. Ils suivent à peu près le format AMC-txt de l'utilitaire
Auto Multiple Choice permettant de générer des QCM pouvant être
corrigés par lecture optique (un scan standard donné dans AMC permet
ensuite d'obtenir un tableau de notes).

Il a fallu ainsi seulement produire des questions sous le format suivant :

```
** Quel sont les avantages pour nos ordinateurs actuels de manipuler du binaire ?
+ Les électroniciens savent fabriquer des composants numériques performants.
+ On fait de l'algorithmique sur les nombres depuis plusieurs millénaires.
+ Il est plus commode de manipuler des nombres que des couleurs ou des sons.
- C'est pas du tout astucieux, les ordinateurs sont lents et ne font rien.
- Ça permet de mieux enregistrer et restituer les sons.
- Les images s'encodent naturellement en binaire.
```

L'exemple vous rend expert, il suffit de partager deux ou trois exemples de 
questions au format AMC-txt avec son équipe pédagogique pour que chacun 
puisse remonter à l'enseignant responable du cours une petite dizaine 
de questions.


## Des exercices pour des commandes bash

Des exercices avec des questions de bash, l'exerice suivant 
est aléatoire sur trois questions différentes mais de 
complexité semblables (comptage de caractères, de mots ou de 
lignes avec wc).

<a href="https://pl.u-pem.fr/filebrowser/demo/25609/" target="_blank">
Comptage textuel dans Germinal</a>

![Comptage textuel dans Germinal]({{ site.url }}/PLaTon-web/assets/images/blog/systeme1.png)

Voici un même type d'exercice avec une question plus 
compliquée, même pour les habitués du bash sous unix. Cet 
exerice a lui aussi 3 variantes tirés au hasard durant 
la construction de l'exercice par la plateforme.

<a href="https://pl.u-pem.fr/filebrowser/demo/25610/" target="_blank">
Comptage d'occurences dans Germinal</a>


Un autre exercice aléatoire sur les commandes du terminal 
Unix, ici en particulier cut et grep ainsi que leurs 
assemblages via des pipes.

<a href="https://pl.u-pem.fr/filebrowser/demo/25611/" target="_blank">
Requête évoluée dans un fichier structuré</a>


## Un template pour script bash

Sur ce patron d'exercice, on attend carrément un petit 
programme bash. Une fois validé, le code de l'élève va 
passer une série de tests. Le script est alors correct 
s'il passe tous les tests automatiques...

<a href="https://pl.u-pem.fr/filebrowser/demo/25612/" target="_blank">
Un script bash qui affiche ses arguments</a>

![Exemples de tests sur les scripts bash]({{ site.url }}/PLaTon-web/assets/images/blog/systeme2.png)


## Circuits logiques aléatoires

Ça commence avec des évaluations de la sortie de circuits 
logiques aléatoires. Ici, c'est le builder qui contient 
beaucoup d'algorithmique avancé car l'exercice commence 
par construire un arbre aléatoire dont les noeuds sont 
des opérateurs logiques d'arités 1 ou 2. Ensuite les 
feuilles de l'arbre sont étiquetées avec une variable 
(l'enseignant choisit le nombre de variable en amont). 
Enfin, des booléens sont tirés aléatoiremenent parmi 
les variables et l'unique sortie du circuit est calculée 
avec une fonction récursive sur le circuit. La génération 
et l'affichage du circuit sont gérés par l'utilitaire Unix 
**dot** ainsi que les composants Angular. 

<a href="https://pl.u-pem.fr/filebrowser/demo/25613/" target="_blank">
Évaluation d'un circuit logique moyen</a>

![Correction graphique d'une évaluation de circuit logique]({{ site.url }}/PLaTon-web/assets/images/blog/systeme3.png)

Dans l'exercice suivant, l'élève doit reconstruire intégralement 
la table de vérité d'un circuit logique aléatoire sous la forme 
d'un tableau de Karnaugh.

<a href="https://pl.u-pem.fr/filebrowser/demo/25614/" target="_blank">
Table de vérité d'un circuit logique</a>

![Circuit et table de Karnaugh]({{ site.url }}/PLaTon-web/assets/images/blog/systeme4.png)

Dans l'exercice qui suit, un tableaux de Karnaugh aléatoire 
est tiré (65536 possibilités). L'élève doit, ce coup ci, 
proposer une fonction python à 4 variables telle que les 16 
évalutations de cette fonction sur les quadruplets de booléens 
coïncident avec les valeurs du tableaux de Karnaugh.

<a href="https://pl.u-pem.fr/filebrowser/demo/25615/" target="_blank">
Une fonction Python pour un tableau de Karnaugh</a>

![Une fonction Python pour une table de Karnaugh]({{ site.url }}/PLaTon-web/assets/images/blog/systeme5.png)


## Mise en place de tests discriminants

C'est un template pour apprendre à tester du code. L'enseignant 
fourni deux paquets de réponses. Un paquets de bonnes réponses 
et un paquet de mauvaises réponses. L'objectif de l'élève est 
de concevoir à l'aveugle une série de tests discriminants. Il 
faut que les bons codes valident positivement tous les tests et 
il faut que, systématiquement, chaque mauvais code échoue sur 
un test au minimum.


Voici un exemple ou il faut proposer des tests pour valider 
le calcul d'une médiane de manière robuste. Il faut imaginer 
des tests, les plus différents possibles, de manière à invalider
les mauvaises médianes tout en gardant les bonnes.

<a href="https://pl.u-pem.fr/filebrowser/demo/25617/" target="_blank">
Doctest challenge : calcul de la médiane</a>

![5 tests ont permis de séparer les bons des mauvais codes]({{ site.url }}/PLaTon-web/assets/images/blog/systeme6.png)


## Mini Brain : simulation d'un petit CPU

Le Mini Brain est un programme Python qui simule le comportement 
d'un processeur minimal à 5 registres et possédant uniquement une 
unité arithmétique en nombre entier.

Il s'agit clairement d'un jeu avec un minimum de règles dans 
lequel on peut programmer des fonctionnalités parfois évoluées 
(par exemple un test de primalité). Il s'agit d'un clone du 
[little thinker](http://sylvain.cherrier.free.fr/LT.html) 
(projet aussi originaire de Marne-La-Vallée) mais adapté pour PLaTon.


<a href="https://pl.u-pem.fr/filebrowser/demo/25618/" target="_blank">
Addition simple avec Mini-Brain</a>

![Exemple de tests et traces dans le Mini Brain]({{ site.url }}/PLaTon-web/assets/images/blog/systeme7.png)

Ce dernier exercice est un peu plus ambitieux :

<a href="https://pl.u-pem.fr/filebrowser/demo/25619/" target="_blank">
Factorielle d'un entier avec Mini-Brain
</a>
