---
title: Apprendre à tester du code
author: Nicolas Borie
layout: post
---

# Doctest me bro !

Un template d'exercice pour apprendre à faire des tests dans les codes sources Python...

## Apprendre à élaborer des tests pour objectif

**Doctest me bro** est un nouveau template d'exercices que j'ai souvent voulu utiliser réellement en TP et en présenciel. 
L'objectif est d'apprendre aux jeunes programmeurs débutants à tester leurs productions informatiques. C'est 
un apprentissage difficile qu'est celui d'écrire des tests unitaires. On tente d'imaginer les pièges, on tente 
de lister les cas dégénérés, on tente d'exprimer quelques utilisations nominales. Mais les tests restent
malheuresement toujours des propositions et des suggestions. Les tests ne peuvent que très rarement garantir 
totalement le bon fonctionnement d'une fonction informatique.

Mais alors, quelles sont les activités pédagogiques qui permettent d'apprendre à élaborer des tests ?

* **La proposition puis la relecture humaine**. Et c'est souvent de cette manière qu'on fait travailler les 
élèves. Mais ça demande un temps incroyable de disponibilité des enseignants et ça doit se faire en face en 
face (ou via micro/caméra...) : le testeur et le relecteur doivent avoir les yeux sur les mêmes tests lorsque 
le relecteur commente oralement.

* **Le débogage**. Et là, il y a deux options. Soit on demande aux apprenants de déboguer leur propre code 
mais ça implique que cela porte sur un projet d'envergure inscrit dans le temps (il y a moins de débogage 
pertinent dans un simple TP de 2 heures). Soit on demande aux apprenants de déboguer un code, produit par autrui, 
proposé au téléchargement dans lequel la localisation des bogues n'est possible que si le code est correctement testé 
pas à pas. Cette dernière option constitue un excellent exercice mais souvent trop long. Sacrifier une séance 
entière de TP pour apprendre à tester/déboguer alors que les notions du cours doivent avancer est un lourd 
sacrifice rarement opéré par les enseignants en informatique.

* **Le doctest me bro template**. C'est un exercice aussi relativement standard : rien de vraiment nouveau. 
Pour apprendre aux élèves à tester, on va leur mettre à disposition deux collections de codes sources résolvant 
le même problème. La première collection de code sources contient des échantillons valides et corrects. La seconde
collection contient des échantillons ayant systématiquement au moins un bogue. Le but de l'élève est maintenant 
de produire une liste de tests raisonnables de manière que toute la collection de codes corrects valident 
l'intégralité des tests; mais aussi que chacun des codes de la seconde collection échoue sur au moins un test. De ce 
fait, la liste de tests produite par l'apprenant devient discrimante sur les deux collections et permet donc 
d'identifier les bons codes et les mauvais codes. Le défaut usuel de cette activité pédagogique est encore le 
temps. L'élève perd son temps à télécharger les collections de codes et à mettre en place les tests en rafalle.
Par contre, l'apport ultime est l'auto-correction! Plus besoin d'une relecture humaine si les échantillons de code 
contiennent suffisement de diversité (et elle est justement humaine cette diversité dans les codes propositions).
Ok, avec PLaTon, on va automatiser tout cela pour permettre à l'élève de juste écrire ses tests puis de faire 
un simple clic qui démarrera toute une moulinette d'éxécution de tests.


## Une grosse moulinette disponible en un clic

Un exemple valant mieux qu'un long discours, voici ici un 
[exercice en démonstration](https://pl.u-pem.fr/filebrowser/demo/20216/) dans lequel il faut proposer des tests 
pour une fonction qui fait la recherche d'un max dans une sous partie d'une liste : les éléments positifs.

Vous pouvez proposer des tests, ces derniers seront automatiquement lancés sur tous les codes des deux 
collections proposées par l'enseignant éditeur: good_code_X et bad_code_Y. Pour information, voici le code 
source complet de l'exercice. Le template *doctest_me_bro_template.pl* utilise par contre subprocess en 
casade sur toutes les clés de l'exercice ayant des préfixes identifiés.

<pre>
#*****************************************************************************
#  Copyright (C) 2020 Nicolas Borie <nicolas dot borie at univ-eiffel . fr>
#
#  Distributed under the terms of Creative Commons Attribution-ShareAlike 3.0
#  Creative Commons CC-by-SA 3.0
#
#    This code is distributed in the hope that it will be useful,
#    but WITHOUT ANY WARRANTY; without even the implied warranty of
#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
#
#  The full text of the CC-By-SA 3.0 is available at:
#
#            https://creativecommons.org/licenses/by-sa/3.0/
#            https://creativecommons.org/licenses/by-sa/3.0/fr/
#*****************************************************************************

title=Doctest challenge : indice du dernier max parmi les positifs

extends=doctest_me_bro_template.pl

text==
Les élèves avaient la consigne suivante :   

<div style="color:white; background-color: black; padding: 0.5em; border-radius: 0.5em;">
Écrivez une fonction python <b>lastMaxPositif</b> qui prend en argument une liste 
d'entiers et qui retourne l'indice du maximum de la liste parmi les nombres positifs.
Si le maximum est contenu plusieurs fois dans la liste, retournez l'index de la 
dernière occurrence. Si la liste ne contient aucun nombre positif, retourner <b>-1</b>.
</div>

Proposez des doctests Python pour detecter la validité et les erreurs 
potentielles des codes rendus par les élèves.
==

good_code_1==#|python|
def lastMaxPositif(L):
    """
    TEST_INCLUSION
    """
    last_max = -1
    for i, elem in enumerate(L):
        if elem >= 0:
            if last_max == -1 or elem >= L[last_max]:
                last_max = i
    return last_max
==

bad_code_1==#|python|                                                   
def lastMaxPositif(L):
    """
    TEST_INCLUSION
    """
    last_max = -1
    for i, elem in enumerate(L):
        if elem >= 0:
            if last_max == -1 or elem > L[last_max]:
                last_max = i
    return last_max
==

bad_code_2==#|python|
def lastMaxPositif(L):
    """
    TEST_INCLUSION
    """
    last_max = -1
    for i, elem in enumerate(L):
        if elem > 0:
            if last_max == -1 or elem >= L[last_max]:
                last_max = i
    return last_max
==

bad_code_3==#|python|
def lastMaxPositif(L):
    """
    TEST_INCLUSION
    """
    last_max = 0
    for i in range(len(L)):
        if L[i] >= 0:
            if L[i] >= L[last_max]:
                last_max = i
    return last_max
==

bad_code_4==#|python|
def lastMaxPositif(L):
    """
    TEST_INCLUSION
    """
    last_max = 0
    current = L[0]
    for i in range(len(L)):
        if L[i] >= 0:
            if L[i] >= current:
                last_max = i
                current = L[i]
    has_pos = False
    for elem in L:
        if elem >= 0:
            has_pos = True
    if not has_pos:
        return -1
    return last_max
==

bad_code_5==#|python|                                                   
def lastMaxPositif(L):
    """
    TEST_INCLUSION
    """
    return -1
==
</pre>


## Un exercice inscrit dans une longue stratégie d'apprentissage

Cet exercice est actuellement proposé à des élèves en L2 informatique à l'université Gustave Eiffel (et en distanciel). 
Il ne s'agit pas d'un exercice très conceptuel et ultra évolué mais il s'inscrit dans une stratégie long terme de 
développement de compétences.

Parmi les 4 grandes compétances de la formation Ingénieur informatique ESIPE de l'Université Gustave Eiffel, la 
seconde compétance portent sur la production, elle s'intitule : Mettre en oeuvre une solution informatique adaptée.
Les deux premières années du cycle ingénieur sont plutôt axés vers le savoir-produire. La dernière année propose 
une coloration qui tire vers l'argumentation et la certification. Ainsi, en troisième année, les élèves doivent :
* garantir la conformité de la solution aux exigences
* garantir le maintien en conditions opérationnelles de la solution
* garantir la qualité des processus de réalisation

Et bien cela doit faire écho aux tests unitaires bien élaborés... Garantir la conformité d'une solution informatique 
complète est surrement une compétence qui peut avoir un sens au niveau BAC+5. Mais on apprend pas à garantir du 
jour au lendemain. En apprenant à faire des tests discrimants en autonomie en BAC+2, les élèves travaillent 
leur capacité à rassembler des arguments qui constitueront les véritables validations qu'ils seront anemés à établir 
plus tard dans leur formation (que ce soit en allant vers un master informatique ou un cycle ingénieur informatique).
