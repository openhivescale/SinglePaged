---
title: "Principle"
bg: green
color: black
fa-icon: align-left
ref: "principle"
lang: "en"
---

<div class="i4x3">
  <div id="slideshow">

<div markdown="1">
## Original steelyard roman balance
![1](img/principe01.png)
</div>
    
<div markdown="1">
## We add a motor to put counter-weight in motion
![2](img/principe02.png)
</div>
    
<div markdown="1">
### An optical endstop detects balance
![3](img/principe03.png)
</div>
    
<div markdown="1">
### A microcontroller drives the system
![4](img/principe04.png)
</div>

<div markdown="1">
### And sends the data...
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

!(img/principle.png)
