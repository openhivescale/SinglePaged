---
title: "Mécanique"
bg: green
color: black
fa-icon: cogs
ref: "mechanical"
lang: "fr"
---

![romainefleury](img/romaine_larive_fleury_t3_175.png)

Basé sur le principe de la balance romaine

Nous ajoutons un moteur pour déplacer le contre-poids

Un capteur optique détecte l'équilibre

Un microcontrôleur pilote l'ensemble, et envoi les données...

-------------- 

### Résolution 6g, précision 30g quelque soit la charge de 0 à 125Kg 
(Protocole de test réalisé permettant de contrôler la linéarité et la répétabilité en cours de rédaction)

-------------- 
 
### Pourquoi une balance mécanique et non pas des jauges de contraintes habituellement utilisées?

Car les jauges de contraintes ne sont pas adaptées à une charge permanente.
  * Les appareils de pesage habituels nécéssitent une tare entre chaque mesure, impossible dans un scénario de surveillance de la ruche
  * Il existe un phénomène de dérive de la mesure connu et documenté, que nous avons pu constater sur notre premier prototype qui utilisait ce type de capteur. Et il n'existe pas de bon compromis coût/qualité de la mesure.
  * Une balance mécanique n'est pas sujette à ce phénomène et même si la structure venait à se déformer, la mesure ne pourrait dériver.


[https://dipot.ulb.ac.be/dspace/bitstream/2013/146415/1/RAM_HBM.pdf](https://dipot.ulb.ac.be/dspace/bitstream/2013/146415/1/RAM_HBM.pdf)

"*Transducer manufacturers provide only information on the short-time stability like maximum creep after 30 minutes or maximum 1 hour under full load, but appear very reticent to provide figures on the long-term stability of their products......*

*Recording strains over long periods of time without having the opportunity to unload the test specimen or the structure and check zero reference is considered to be one of the most difficult applications of strain-gauges....*"

[http://www.analog.com/en/analog-dialogue/articles/a-reference-design-for-weigh-scales.html](http://www.analog.com/en/analog-dialogue/articles/a-reference-design-for-weigh-scales.html)

Parceque nous ne dépendons d'aucun composant complexe sur la partie mécanique (moteur, fourche optique)
  * Cela permet d'obtenir un prix inégalé pour un tel niveau de précision et de robustesse 
  * En cas de problème, le diagnostic et la réparation sont aisés
  * *DIY-ers friendly (Do It Yourself)*
 
L'électronique est beaucoup plus simple : pas d'étage analogique dont dépend la qualité de la mesure
 
--------------
 
### Enjeu : intégration sous la ruche
Contrairement à la romaine qui est suspendue, notre balance doit s'intégrer sous la ruche
Vu le poids à peser (100kg), le contrepoids souhaitée (500g), et l'espace disponible, avoir un seul bras de levier est impossible (1:200, 40cm, le bras de levier primaire devrait faire 2mm.). D'où un design à deux "étages".

![principle](img/principle.png)

Nous avons conçu un kit durable, réparable, modifiable, évolutif.

Composé de profilés en aluminium et d'acier inoxydable découpé au laser, assemblé par de la visserie inox. Très peu d'autres pièces, un simple moteur, une courroie, un palier linéaire, un capteur optique. C'est tout.

<div class="icontain">
  <iframe src="https://www.youtube.com/embed/kFrGVwb06q8" allowfullscreen></iframe>
</div>
<br>

Aucune compétence particulière n'est nécéssaire au montage. 

Le même niveau de rigueur et de patience que pour un meuble ikea suffira.

![photo](img/IMGP9335R.jpg)

Photo de présentation, la version commercialisée dispose d'un boitier étanche pour l'électronique et d'un capotage de protection au dessus des des bras de levier.


<iframe width="1264" height="550" seamless frameborder="0" scrolling="no" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSkP-vBIrygrKL4rIhkSzMw3B0RTOQDyZ21LOhGQGx0f2L3cipl1LCMDOu8Xt_0CLbM8wPw9Htej1xK/pubchart?oid=1184278694&amp;format=interactive"></iframe>

Exemple de protocole de test réalisé avec un module Sigfox:
Après la pose d'un sol de ruche, on ajoute des masses A, B, puis C, puis on les enlève progressivement et on les repositionne dans le même ordre. Vous pouvez constater la précision... 
Au niveau de l'autonomie on obtient un résultat de 1325 mesures avec les 3 piles AA.
