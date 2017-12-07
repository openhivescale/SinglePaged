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


## Why a mechanical scale, and not a load cell?

- Because load cell are not supposed to be under continuous constraint.
  * A creep phenomen make measurement unstable after some time, this is well documented
  * Load cells manufacturers don't communicate on creep over 30 minutes...
  * Typical use case implies a tare between each measurement, not possible in hive monitoring scenario
  * We check this on our first prototype using load cells, it was worse than expected
  * Mechanical scale is not subject to this phenomena. Even if structure creeps, measurement doesn't change.

- Because we don't depend on any complicated part that we must outsource
  * This makes possible to keep price low
  * Easier to understand what could go wrong and repair
  * DIY-ers friendly

- Principle is simple and old as ancient Rome
