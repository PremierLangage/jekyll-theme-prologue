---
title: Yggdrasil 2019-2020
author: Nicolas Borie
layout: post
---

# L'édition de ressources pédagogiques sous PLaTon

Un bilan du serveur central de ressources à partir des commits git extraits jusqu'au 11 Mai 2020...


Voici un résumé rapide de l'édition partagée des ressources pédagogiques
sur la plateforme PLaTon. Ce document est généré à l'aide du
gestionnaire de versions **git** qui permet notamment de suivre toute
action sur les fichiers du serveur central de ressources de PLaTon.


## Les chiffres depuis la création d'Yggdrasil


La plateforme PLaTon rassemble aujourd'hui 22 dépôts git sur sa page
[github de PLaTon](https://github.com/PremierLangage). Parmi tous ces
dépôts, il y a [Yggdrasil : dépôt git centralisant les
ressources](https://github.com/PremierLangage/Yggdrasil). Les données
qui vont suivre sont construites à partir des logs de tous les commits
de ce dépôt.


### Les disciplines des éditeurs de ressources


L'informatique et les mathématiques sont les deux disciplines
largement représentées. En effet, les outils numériques étant plus
courants dans ces matières, les acteurs enseignants sont plus à l'aise
pour prendre en main PLaTon. 


![Répartition des éditeurs selon leur discipline]({{ site.url }}/PLaTon-web/assets/images/disciplines.png)


### Les fonctions exercées par les éditeurs de ressources


Tous les acteurs enseignants de l'université sont représentés parmi les
utilisateurs concepteurs et éditeurs de ressources pédagogiques dans
PLaTon. Il a principalement des permanents de l'enseignement supérieur
mais aussi des agents temporaires d'enseignement et de recherche, des
vacataires, des élèves stagiaires et des apprentis.


![Répartition des éditeurs selon leur fonction]({{ site.url }}/PLaTon-web/assets/images/fonction.png)


### Activités des éditeurs de ressources


Actuellement, on peut classer les personnes éditant les ressources en trois groupes :

* Les power users : 3-4 utilisateurs qui repoussent les capacités de
  la plateforme. Ces utilisateurs conçoivent des exercices pour leurs
  élèves mais aussi pour d'autres enseignants. Ils sont les
  concepteurs des patrons génériques d'exercices réutilisables.

* Les adeptes : une dizaine de personnes relativement autonomes qui
  contribuent aux ressources via des ajouts et des corrections. 

* Les novices : une petite vingtaine d'utilisateurs qui utilisent des
  patrons d'exercices préparés par d'autres utilisateurs plus avancés. 

![Répartition des éditeurs selon leur fonction]({{ site.url }}/PLaTon-web/assets/images/editeurs.png)

* **Ajouts** : compte les ajouts de nouveaux fichiers dans les ressources

* **Délétions** : compte les suppressions de fichiers dans les ressources

* **Modifications** : compte les modifications de fichiers dans les ressources

* **Rayon d'action** : compte le nombre total de fichiers sur lesquels l'utilisateur a eu un impact


## Quelques critiques et réflexions


Sachant que PLaTon n'est toujours pas dans sa version 1.0, l'année
scolaire 2019-2020 est riche d'expérience et devrait mettre la
plateforme sur de bon rails pour son réel lancement.


La plateforme UPEM enregistre aujourd'hui 1200 utilisateurs (18 août
2020) profs et élèves et ces derniers ont sollicité 465835 fois les
scripts d'auto-correction des exercices. Principalement utilisée pour
les trois années de licence en math et info, 34 personnes ont édité des
ressources pédagogiques via l'éditeur interne de la
plateforme. Seulement deux professeurs en informatique récalcitrants
du Laboratoire de Recherche en Informatique de l'université Paris-Sud
refusent l'éditeur intégré de la plateforme au profit de solutions
plus "ligne de commande". Leur travaux d'édition n'entrent pas dans les
statistiques au dessus et ils ne sont pas comptés dans les données
présentées plus haut.


Les ressources représentent actuellement 1943 fichiers dont 1324
fichiers d'extension pl désignant le plus souvent des exercices
PLaTon. Parmi les choses remarquables, on peut faire les observations
suivantes :

* Bien que PLaTon soit très jeune, la répartition des utilisateurs
  selon leur expérience est tout à fait naturelle et normale. On a
  actuellement 3-4 experts, une dizaine d'adeptes et le reste de
  novices (On divise pas deux environ d'un niveau à un autre).
  
* Toutes les contributions sont bonnes à prendre et tous les éditeurs
  jouent un rôle important quelques soient leurs expériences et
  compétences. Sans novices motivés, il est impossibles pour les power
  users de valider la simplicité d'utilisation des patrons
  d'exercices. Les novices sont aussi souvent les meilleurs sources
  d'informations pour identifier les erreurs et bogues. Les récits de
  leurs expériences permet aux développeurs et power users d'établir
  les priorités sur les prochaines taches de développement.
  
* Plus les enseignants éditeurs ont de l'expérience, plus ils
  commencent à raffiner les ressources produites. On le voit notamment
  sur le nombre de fichiers supprimés pour chaque utilisateur. Alors
  que le novice a souvent pour objectif de produire une ressource
  opérationnelle à rattacher rapidement dans Moodle pour le soumettre
  à ces élèves ; les contributeurs avancés ont parfois déjà procédé à
  des refactoring. Petit à petit, la finesse est recherchée et des
  tentatives d'augmentation de l'expérience utilisateur sont
  faites. Actuellement, les ressources hébergent au moins trois types de
  Q.C.M., chaque implémentation augmentant la précédente via une
  meilleure ergonomie ou des fonctionnalités enrichies.

* La plupart des ressources profitent automatiquement des évolutions
  de la plateforme. Le coeur du serveur très technique (Django,
  Docker, Angular, etc) est complètement détaché des ressources
  pédagogiques (le fameux dépôt Yggdrasil indépendant). Les ressources
  pédagogiques utilisent de manière formelle les fonctionnalités du
  serveur PLaTon. Moteur et ressources étant ainsi très faiblement
  couplés, les productions pédagogiques de cette année 2019-2020 sont
  une excellente capitalisation pour les années prochaines et en
  particulier la rentrée à venir avec les conditions imposées par la
  crise sanitaire.
