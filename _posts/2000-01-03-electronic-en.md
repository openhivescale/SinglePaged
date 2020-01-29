---
title: "Electronic"
bg: purple
color: black
fa-icon: microchip
ref: "electronic"
lang: "en"
---

![IMGP9367.jpg](img/IMGP9367.jpg)

## Connectivity

- WiFi
  * Included in every board
  * Cheapest option if you have a hotspot accessible
  * User-friendly configuration with a smartphone or laptop
  * Master-slave scenario, for sharing a single GSM or Sigfox endpoint
  * Wifi connection allows future slave modules

- Sigfox (optional)
  * Sigfox is a new cellular network dedicated to IoT. Low bandwidth, low power, long range.
  * Best option for battery life if no hotspot
  * Subscription cheaper than GSM
  * Network coverage complementary with GSM
  * [World roll-out in progress](https://www.sigfox.com/en/coverage)

- GSM (optional)
  * Best coverage all around the world
  * Possible to interrogate via SMS without internet connection

- Lora (optional)
  * Alternative network to Sigfox, similar power consumption and coverage (LPWAN)
  * Possible to use the collaborative network [TheThingsNetwork](https://www.thethingsnetwork.org/)
  * We don't propose yet subscription using commercial networks

-------------------------
  
## Autonomy

Best energy is the one you don't use...

- First, highly optimized electronic
  * 100nA sleep current
  * Motor driving strategy to reduce motor use
  * Modular measurement frequency and data send along the year

- Then we look for the best trade-off between environmental impact, cost, availability of batteries
  * We managed to achieve a good autonomy with simple alkaline batteries
  * On a 10 years life cycle, rechargeable battery, Li-ion or Ni-MH, with or without solar panel as an higher cost and impact
  * AA alkaline batteries are the most available battery all around the world

With 3xAA alkaline batteries, we expect 2-5 years autonomy, depending on climate, measurement frequency etc...

