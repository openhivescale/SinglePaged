---
title: "Mechanical"
bg: green
color: black
fa-icon: cogs
ref: "mechanical"
lang: "en"
---
![romainefleury](img/romaine_larive_fleury_t3_175.png)

Original steelyard roman balance

We add a motor to put counter-weight in motion

An optical endstop detects balance

A microcontroller drives the system and send the data

-------------- 

### Resolution 6g, precision 30g whatever the load is from 0 to 125Kg 

(Documentation of the tests allowing to control linearity and repeatabiliy is under progress)

-------------- 

## Why a mechanical scale, and not using load cells?

Because load cell are not supposed to be under continuous load
  * Typical use case implies a tare between each measurement, not possible in hive monitoring scenario
  * A creep phenomen make measurement unstable after some time, this is well documented, that we check on our first prototype
  * Mechanical scale is not subject to this phenomen. Even if structure creeps, measurement wouldn't change.

[https://dipot.ulb.ac.be/dspace/bitstream/2013/146415/1/RAM_HBM.pdf](https://dipot.ulb.ac.be/dspace/bitstream/2013/146415/1/RAM_HBM.pdf)

"*Transducer manufacturers provide only information on the short-time stability like maximum creep after 30 minutes or maximum 1 hour under full load, but appear very reticent to provide figures on the long-term stability of their products......*

*Recording strains over long periods of time without having the opportunity to unload the test specimen or the structure and check zero reference is considered to be one of the most difficult applications of strain-gauges....*"

[http://www.analog.com/en/analog-dialogue/articles/a-reference-design-for-weigh-scales.html](http://www.analog.com/en/analog-dialogue/articles/a-reference-design-for-weigh-scales.html)

Because we don't depend on any complicated part that we must outsource on the mechanical part (motor, optical endstop)
  * This makes possible to keep cost low
  * Easier to understand what could go wrong and repair
  * DIY-ers friendly

Electronic is much simpler : no analog layer on which measurement quality depends
 
--------------

### Enjeu : intégration sous la ruche
Unlike steelyard that is suspended, our scale has to intergrate under the hive
Given the object to weigh (100kg), the expected counter weight (500g), and available space, having a single beam is impossible (1:200, 40cm, primary beam should be 2mm long). Here is why a 2 stages design

![principle](img/principle.png)

We designed a long lasting, fixable, customisable kit.


It's made of aluminium profiles and laser cut stainless steel, joint by stainless bolts.

Very few 'other' parts, a simple motor, a belt, linear bearing, optical end stop. That's it.

<div class="icontain">
  <iframe src="https://www.youtube.com/embed/kFrGVwb06q8" allowfullscreen></iframe>
</div>
<br>

No special skills required for assembly.
If you're able to mount an ikea furniture, you should be fine.

![photo](img/IMGP9335R.jpg)

The picture doesn't show modifications that will be on the kit sold : a waterproof case for electronic, and a protection above beams.

