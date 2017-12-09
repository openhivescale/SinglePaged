---
title: "Principe"
bg: green
color: black
fa-icon: align-left
ref: "principle"
lang: "fr"
---

<div class="i4x3">
  <div id="slideshow">

<div markdown="1">
### Balance Romaine originale
![1](img/principe01.png)
</div>
    
<div markdown="1">
### Nous ajoutons un moteur pour déplacer le contre-poids
![2](img/principe02.png)
</div>
    
<div markdown="1">
### Un capteur optique détecte l'équilibre
![3](img/principe03.png)
</div>
    
<div markdown="1">
### Un microcontrôleur pilote l'ensemble
![4](img/principe04.png)
</div>

<div markdown="1">
### Et envoie les données...
![5](img/principe05.png)
</div>

  </div>
</div>.


## Pourquoi une balance mécanique et non pas des jauges de contraintes habituellement utilisées?

- Car les jauges de contraintes ne doivent être soumises à une charge permanente.
  * Un phénomène de fluage rend la mesure non linéaire après un certain temps, ceci est bien documenté
  * Les fabricants de jauges de contraintes ne précisent pas la dérive après 30 minutes...
  * Les appareils de pesage habituels permettent une tare entre chaque mesure, impossible dans un scénario de surveillance de la ruche
  * Nous avons constaté ce phénomène de dérive sur notre premier prototype qui utilisait des jauges de contraintes, les résultats ont été pires qu'attendu
  * Une balance mécanique n'est pas sujette à ce phénomène et même si la une structure venait à se déformer, la mesure ne pourrait dériver.

- Parceque nous pouvons construire nous même tous les organes et que nous n'achetons aucun composant complexe
  * Cela permet d'obtenir un prix inégalé pour un tel niveau de précision et de robustesse
  * En cas de problème, le diagnostic et la réparation est aisé
  * DIY-ers friendly (Do It Your Self)
  
- Le principe est simple et vieux comme la Rome antique

![principle](img/principle.png)
