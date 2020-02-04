---
title: Documentation
subtitle: Toutes les documentations autour de PLaTon
layout: "page"
icon: fa-book-open
order: 3
---

PLaTon est une application complexe. Comme elle se veut ouverte au partage, idéalement PLaTon
est documenté à tous les niveaux. Suivant le rôle que vous souhaitez jouer, vous devriez trouver une documentation adapté à
vos intentions. <a href="https://documentationpl.readthedocs.io/fr/latest/contribuer/" target="blank">Voici ici quelques 
conseils pour contribuer.</a>


Pour les plus spécialistes de l'informatique souhaitant participer au coeur de l'application PLaTon, la
documentation est porté par le code source dans le dépôt dédié 
<a href="https://github.com/PremierLangage/premierlangage">permierlangage</a>. L'architecture logicielle et le design 
applicatif est discuter plutôt ici <a href="https://github.com/PremierLangage/plconception">plconception</a>.


Les enseignants éditeurs travaillent sur l'éditeur en ligne de PLaTon. Pour cela, vous devrez être identifié 
sous une application utilisant le protocole L.T.I. (avec moodle par exemple). Une fois identifié sur une application de 
votre structure (université, lycée, ...) avec L.T.I. en ayant le rôle d'enseignant, il suffit alors de suivre le lien 
suivant <a href="https://pl.u-pem.fr/activity/play/0/">serveur Premier Langage</a>


La documentation de PLaTon pour les enseignants est une compilation web du dépôt github 
suivant <a href="https://github.com/PremierLangage/premierlangage-doc">premierlangage-doc</a>. Le 
rendu web est disponible publiquement <a href="https://documentationpl.readthedocs.io/fr/latest/">sur 
cette page</a>. Toute aide pour augmenter la qualité de la documentation (y compris des aides orthographiques) est 
bienvenue.


<h2>Librairie scientifique autour de PLaTon</h2>
    
    
PLaTon est une expérience de développement ambitieuse. Aussi, adopter une démarche rigoureuse est primordial 
pour assurer la pérennité du logiciel. Cette page rassemble des documents scientifiques et techniques autour de PLaTon.
    

<h3>Documents relatifs à la conception de l'outil PLaTon</h3>

<ul>

<li>La présentation suivante raconte un peu <a href="https://github.com/PremierLangage/PLPR/blob/master/PL_dev_philo.pdf">notre 
philosophie de développement</a>. La présentation justifie nos choix organisationnel dans le développement de PLaTon.</li>

<li>Schéma du mécanisme de <a href="https://github.com/PremierLangage/PLPR/blob/master/doc_technique/structure.pdf">jeu 
des ressources</a> dans PLaTon en Octobre 2018. Le schéma montre comment un exercice atomique est traité
par le serveur pour être proposé à l'élève puis corrigé. Les actions sensibles (comme les exécutions de code proposé par
des élèves) sont effectuées en machines virtuelles.</li>

<li>Schéma de l'<a href="https://github.com/PremierLangage/PLPR/blob/master/doc_technique/archi.pdf">architecture logicielle</a> 
de PLaTon en Novembre 2018. Cette architecture à bien changer depuis mais le document illustre notre vision de l'application 
à la date précisée.</li>
  
<li>Schéma simplifié du <a href="https://github.com/PremierLangage/PLPR/blob/master/doc_technique/playexo.pdf">jeu 
d'une ressource</a> de PLaTon. Le Schéma situe les deux programmes python utilisés lors du jeu d'un exercice 
: le builder et le grader. Le premier prépare une ressource (en tirant au hasard une question par exemple). Le second
programme a pour rôle de corriger et de conseiller l'élève suivant la réponse qu'il a fournit à l'exercice.</li>

</ul>
    

<h3>Articles pédagogiques et didactiques autour de PLaTon</h3>

Rien pour le moment, mais l'équipe de conception de PLaTon a clairement l'intention de faciliter toute personne 
ou équipe souhaitant utiliser PLaTon comme lieu d'expérimentation. Les besoins statistiques et logiques seront 
écouté pour permettre à tout enseignant et/ou chercheur de mener à bien son expérience.
