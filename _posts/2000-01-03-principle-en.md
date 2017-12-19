---
title: "Mechanical"
bg: green
color: black
fa-icon: align-left
ref: "mechanical"
lang: "en"
---


![principe 01](img/principe01.png)
## Original steelyard roman balance
## We add a motor to put counter-weight in motion
## An optical endstop detects balance
## A microcontroller drives the system and send the data
<div markdown="1">


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

![principle](img/principle.png)
