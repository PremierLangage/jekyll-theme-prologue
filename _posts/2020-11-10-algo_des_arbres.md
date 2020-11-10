---
title: Algo des arbres
author: Nicolas Borie
layout: post
---


# Quelques petits exercices P.O.C. pour de l'algo des arbres

J'ai programmé quelques prototypes d'exercices autour de l'algorithmique des arbres. Le
composant **Graph Viewer** donne un plein accès à l'utilitaire **DOT** et les graphes sont
possiblement constructibles et exploitables à la fois dans les **builders** et les 
**graders** des exercices dans PLaTon.
 
  
## Statistiques simples sur les arbres binaires

On commence avec un exercice très très fortement aléatoire. Le builder tire un entier entre
8 et 14, puis construit un arbre binaire ayant cet entier pour nombre total de nœuds. Les 
étiquettes de l'arbre construit sont systématiquement aléatoires et différentes.

![statistique sur arbre binaire]({{ site.url }}/PLaTon-web/assets/images/blog/stat.png)

Une fois l'arbre constuit, une des statistiques suivantes est demandée à l'apprenant...

* la hauteur
* le nombre de feuilles
* l'étiquette maximale dans les feuilles
* l'étiquette minimale dans les feuilles
* le nombre de nœuds internes
* l'étiquette maximale parmi les nœuds internes
* l'étiquette minimale parmi les nœuds internes

Pour tester et retester cet exercice, il suffit de cliquer sur le lien suivant : 
<a href="https://pl.u-pem.fr/filebrowser/demo/31473/" target="_blank">Statistique dans un arbre binaire</a>.


## Exercices de programmation en C pour les arbres

À l'université Gustave Eiffel, sur le campus de Marne-La-Vallée, le cours d'algo des arbres 
est professé en seconde année de la licence Math-Info. Ce même cours est historiquement fait 
avec le langage C pour la partie programmation des algorithmes.

Il a suffit de customiser (un template peut hériter d'un autre template sous PLaTon) le 
template pour les exercices de programmation en C. Pour les experts sytème, le template
standard pour les exos de programmation en C utilise des séries arguments, des entrées 
standards avec une solution enseignant. L'apprenant doit alors coder un morceau de code
C tel qu'avec les arguments et les contenus d'entrée standard fourni par le prof, le 
code de l'élève génère les mêmes sorties standard que la version de l'enseignant 
(dans l'esprit des doctests Python mais à l'échelle d'un programme).

La seule chose surchargée dans ce template est le feedback du **grader**. Lorsque 
l'entrée standard contient le code textuel d'un arbre binaire ayant moins de 20 nœuds,
ce dernier est affiché graphiquement après génération d'une image par **DOT**. C'est quelque 
chose que nous n'avons jamais eu avant en TP (même en présentiel, visualiser les arbres
avec **DOT** est possible mais long et pénible à mettre en place). PLaTon permet d'automatiser
la génération des arbres et de les inscruster dans le feedback, c'est un gain de temps
incroyable et une grosse amélioration de l'expérience utilisateur.

![statistique sur arbre binaire]({{ site.url }}/PLaTon-web/assets/images/blog/code_arbre_dot.png)

Pour tester l'exercice (c'est de la programmation en C, ça reste technique...), il faut cliquer par là :
<a href="https://pl.u-pem.fr/filebrowser/demo/31475/" target="_blank">Fonction calculant la hauteur d'un arbre binaire</a>.


## Un exercice d'imagination et modélisation

Parce que plus les questions sont ouvertes, plus le challenge est motivant et authentique. 
Et aussi parce l'on ne fait jamais assez de dessins (soi-même ou avec les élèves...). Voici 
un exercice ou le nombre de bonnes réponses possibles est très important, il suffit d'en 
construire sa bonne réponse.

L'exercice construit un arbre aléatoire avec entre 4 et 8 nœuds. On pourrait mettre des 
enjeux plus gros mais un bon exercice doit rester fluide et ne pas blocquer trop longtemps.
Les statisiques montrent que l'apprenant sous PLaTon entreprend une action (un clic, une 
soumission de réponse, etc...) toute les minutes. Une fois l'abre construit, un certain 
nombre de statistiques sont extraites de cet arbre. Une fois qu'un bon vecteur de contraintes
est construit, l'exercice est enfin proposé à l'élève. La consigne est la suivante : 
construire un arbre cohérent par son codage textuel qui valide toutes les contraintes.

Les contraintes restent toutefois bien stéréotypées :

* étiquettes entières toute différentes
* un nombre de nœuds au total
* la hauteur
* le nombre de feuille
* Soit ça penche récursivement à gauche ou à droite (les nœuds voient toujours plus de feuilles à gauche ou à droite)
* Les étiquettes de l'arbre sont croissantes ou décroissantes le long des branches

![Un arbre est recherché !]({{ site.url }}/PLaTon-web/assets/images/blog/arbre_cherche.png)

![Vérification des contraintes]({{ site.url }}/PLaTon-web/assets/images/blog/feedback.png)

Ces contraintes ont systématiquement au moins une solution mais souvent bien plus. Ici, 
il faut faire des choix et imaginer sa propre solution.

Pour tester cet exercice d'imagination, c'est ici :
<a href="https://pl.u-pem.fr/filebrowser/demo/31476/" target="_blank">Construire l'arbre qui va bien !</a>.

Si vous ne comprennez pas comment fonctionnent les codages textuels proposés dans ces exercices,
en bien il existe un exercice (aussi aléatoire et répétable moult fois) pour apprendre comment 
cela fonctionne :
<a href="https://pl.u-pem.fr/filebrowser/demo/31477/" target="_blank">Codage textuel d'un arbre binaire</a>.
