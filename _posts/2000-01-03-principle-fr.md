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


## Pourquoi une balance mécanique et non pas des jaugs de contraintes habituellement utilisées?

- Car les jauges de contraintes ne doivent être soumises à une charge permanente.
  * Un phénomène de fluage rend la mesure non linéaire après un certain temps, ceci est bien documenté
  * Les fabricants de jauges de contraintes ne précisent pas la dérive après 30 minutes...
  * Les appareils de pesage habituels permettent une tare entre chaque mesure, impossible dans un scénario de surveillance de la ruche
  * Nous avons constaté ce phénomène de dérive sur notre premier prototype qui utilisait des jauges de contraintes, les résultats ont été pires qu'attendu
  * Mechanical scale is not subject to this phenomena. Even if structure creeps, measurement doesn't change.

- Because we don't depend on any complicated part that we must outsource
  * This makes possible to keep price low
  * Easier to understand what could go wrong and repair
  * DIY-ers friendly

- Principle is simple and old as ancient Rome
