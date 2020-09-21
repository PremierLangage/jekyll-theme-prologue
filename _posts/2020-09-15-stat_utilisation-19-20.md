---
title: Bilan PLaTon 2019-2020
author: Nicolas Borie
layout: post
---

# Utilisation de PLaTon sur l'année universitaire 2019-2020

Statistiques compilées à partir des logs bruts de la plateforme entre
septembre 2019 et septembre 2020...


## Les grands nombres de PLaTon cette dernière année


Les statistiques de l'année universitaire 2019-2020 sont déjà
relativement affolantes sachant qu'elles correspondent à une année de
test. Durant cette année, c'est la version 0.7.4 de Premier Langage
devenant PLaTon qui a été déployée. 


L'équipe n'a aucun regret car la version 1.0, qui devrait arrivée dans
peu de temps, va bénéficier de toute l'expérience accumulée durant
l'année dernière. Aussi, nous possédons maintenant de nombreuses
ressources pédagogiques déjà testées et opérationnelles.


**Bilan annuel 2019-2020 :**   

**150 107** corrections d'exercice en direct effectués par les sandbox (24h/24 et 7j/7)   
**58 984** exercices parfaitement réussis (note maximale 100/100)   
**1 110** utilisateurs actifs (ayant travaillé sur au moins un exercice)   
**5239.0 h 35.0 m** temps de travail cumulé des utilisateurs sur PLaTon    
**4.0 h 43.0 m** temps de travail moyen pour chacun des **1110** utilisateurs   
**34** enseignants éditeurs de ressources   
**1324** fichiers ressources pédagogiques d’extension .pl   
**18345** actions d'édition sur les ressources opérées par les enseignants éditeurs.   
**31** cours PLaTon créés (une vingtaine diffusés à grande échelle aux élèves, une dizaine pour des tests)   
**615** exercices auto corrigés déployés (sans compter les différentes versions)   
**88** activités (fiches de TP) déployés (sans compter les différentes versions)   
**5** relances manuelles des sandbox suite à blocage   
**2** universités sur le serveur-assets de Marne-La-Vallée : U. Gustave Eiffel et U. Paris Saclay   


## Activité par jour de la semaine sur toute la période

L'activité est ici mesurée par nombre d'appels aux sandbox docker. Ces
sandbox docker sont les environnements sécurisés dans lesquels PLaTon
fabrique les exercices et mène les corrections. Quand un élève ouvre
un exercice, un programme Python est sollicité sur ces sandbox pour
fabriquer l'exercice et ses parties intelligentes. Si l'exercice est
aléatoire, cela signifie qu'un ordinateur doit lancer des dés pour
obtenir des nombres aléatoires. Ce sont les sandbox qui se chargent de
cette tache.

Pour les corrections, c'est pareil. Certaines corrections sont très
élémentaires mais certaines demandent d'exécuter des programmes
tiers. Par moment, comme l'exercice porte sur de la programmation, il
faut carrément exécuter du code d'élèves, possiblement dangereux pour
un ordinateur. Ainsi toute correction est confinée dans les sandbox
et même si un problème devait se déclarer, la plateforme n'est pas en
péril.

Mesurer le nombre de sollicitations sur les sandbox, c'est ainsi
complètement mesuré l'activité ses élèves qui utilisent PLaTon.

![activité selon les jours de la semaine]({{ site.url }}/PLaTon-web/assets/images/blog/semaine.png)

Les Lundis sont les jours de plus grande activité, suivis de peu des
mercredis et mardis. Les jeudis après-midis sont très souvent
banalisés à l'Université Gustave Eiffel pour laisser les étudiants
libres à la pratique du sport ou d'autres activités extra scolaires.


Durant les week-ends, la plateforme n'est pas en sommeil. Le dimanche
soir a été utilisé par certains enseignants comme date limite de
rendu.


## Activité heure par heure d'une journée typique hors week-end

![Jour classique de semaine hors week-end]({{ site.url }}/PLaTon-web/assets/images/blog/jour_semaine.png)

Ce graphique présente les moyennes d'activité heure par heure opérées
sur les jours du lundi au vendredi inclus. La forme de cet histogramme
de répartition lisse les artefacts journaliers apparaissant sur les
courbes dûs, par exemple, au choix des emplois du temps. La forme finale
représente donc la répartition classique d'une journée typique de semaine.


## Activité pour jour de la semaine


### Les lundis

![Activité les lundis]({{ site.url }}/PLaTon-web/assets/images/blog/lundi.png)

### Les mardis

![Activité les mardis]({{ site.url }}/PLaTon-web/assets/images/blog/mardi.png)

### Les mercredis

![Activité les mercredis]({{ site.url }}/PLaTon-web/assets/images/blog/mercredi.png)

### Les jeudis

![Activité les Jeudis]({{ site.url }}/PLaTon-web/assets/images/blog/jeudi.png)

### Les vendredis

![Activité les vendredis]({{ site.url }}/PLaTon-web/assets/images/blog/vendredi.png)

### Les samedis

![Activité les samedis]({{ site.url }}/PLaTon-web/assets/images/blog/samedi.png)

### Les dimanches

![Activité les dimanches]({{ site.url }}/PLaTon-web/assets/images/blog/dimanche.png)

Les activités par jour et par heures sont sensibles aux placements des
groupes de TP en première année de Licence math-info à l'Université
Gustave Eiffel. Une épreuve de seconde session organisée avec les 
première année de licence à L'Université Paris-Sud durant un
mardi à 14h00 fait aussi explosé ponctuellement l'activité associée
à cette horaire.


Dans ces tableaux, les barres noires correspondent à des horaires de
semaine, en horaire ouvrable, c'est à dire de 8 heures à 18 heures. Le
gros enseignement de ces tableaux est que vous ne savez pas quand vos
étudiants seront disposé et en conditions pour travailler. La crise du
COVID-19 n'a pas changé les horaires de travail. Beaucoup travaillent le
soir tard (ce qui n'est pas l'idéal pour le suivi le lendemain en
cours) car les domiciles sont plus calmes et l'on peut jouir du
matériel informatique quand ce dernier est en partage avec le reste de
la famille. Cette répartition ne tient même pas compte des vacances
scolaires mais observe l'activité selon les horaires et les jours de
toute l'année.


Nombre total de sollicitations sandbox en 2019-2020 : **315 606**   
Nombre de sollicitations sandbox en dehors de la plage 8h00 - 18h00 du lundi au vendredi : **148 442**   
**47.03 %** de l'activité à eu lieu durant des horaires où les élèves
ne sont pas supposés se trouver à l'université et ce calcul ne tiens
pas compte des vacances scolaires encore une fois. Sachant que les
cours durent deux fois douze semaines avec environs 8 à 10 semaines
autour pour les révisions et examens divers (sur 52 semaines annuels),
il parait évident que plus de la moité de l'activité de la plateforme
PLaTon a lieu à des horaires où les enseignants ne sont pas
disponibles.


## Activité par mois

### Comparaison de septembre 2019 à août 2020


Nous avons déployé PLaTon le 12 septembre et il manque deux jours de
statistiques à la fin d'août (les 30 et 31), sinon l'année universitaire 2019-2020
est complète.

![Activité chaque mois]({{ site.url }}/PLaTon-web/assets/images/blog/mois.png)

Nous avons procédé à de nombreux tests de charge durant Octobre (en
incitant les étudiants à se défouler pour voir si, techniquement,
PLaTon tenait la charge). Février est le mois de transition entre les
deux semestres de l'université. Durant le mois de mars, plusieurs
enseignants sont venus rencontrer l'équipe de développement de PLaTon
pour voir ce qu'il était possible de faire en urgence avec le
confinement lié au COVID-19.


La plateforme a été maintenue opérationnelle par le centre de
ressources informatiques de l'Université Gustave Eiffel les mois de
juillet et d'août. certains examens de secondes sessions ayant été
repoussés début septembre, les étudiants volontaires pouvaient
continuer de travailler à distance s'ils le souhaitaient durant les
vacances d'été.


### Septembre

![Activité en septembre 2019]({{ site.url }}/PLaTon-web/assets/images/blog/septembre.png)

### Octobre

![Activité en octobre 2019]({{ site.url }}/PLaTon-web/assets/images/blog/octobre.png)

### Novembre

![Activité en novembre 2019]({{ site.url }}/PLaTon-web/assets/images/blog/novembre.png)

### Décembre

![Activité en décembre 2019]({{ site.url }}/PLaTon-web/assets/images/blog/decembre.png)

### Janvier

![Activité en janvier 2020]({{ site.url }}/PLaTon-web/assets/images/blog/janvier.png)

### Février

![Activité en février 2020]({{ site.url }}/PLaTon-web/assets/images/blog/fevrier.png)

### Mars

![Activité en mars 2020]({{ site.url }}/PLaTon-web/assets/images/blog/mars.png)

### Avril

![Activité en avril 2020]({{ site.url }}/PLaTon-web/assets/images/blog/avril.png)

### Mai

![Activité en mai 2020]({{ site.url }}/PLaTon-web/assets/images/blog/mai.png)

### Juin

![Activité en juin 2020]({{ site.url }}/PLaTon-web/assets/images/blog/juin.png)

### Juillet

![Activité en juillet 2020]({{ site.url }}/PLaTon-web/assets/images/blog/juillet.png)

### Août

![Activité en août 2020]({{ site.url }}/PLaTon-web/assets/images/blog/aout.png)
