---
title: "Principio"
bg: green
color: black
fa-icon: align-left
ref: "principle"
lang: "es"
---

<div class="i4x3">
  <div id="slideshow">

<div markdown="1">
### Antigua bascula romana
![1](img/principe01.png)
</div>
    
<div markdown="1">
### Añadimos un motor para poder mover el contrapeso
![2](img/principe02.png)
</div>
    
<div markdown="1">
### Un detector óptico detecta el equilibrio
![3](img/principe03.png)
</div>
    
<div markdown="1">
### Un microcontrolador maneja el sistema
![4](img/principe04.png)
</div>

<div markdown="1">
### Y envía los datos...
![5](img/principe05.png)
</div>

  </div>
</div>.


## ¿Por qué una balanza mecánica, y no una celda de carga?

- Debido a que la celda de carga no se supone que esté bajo carga continua.
  * Un fenómeno de fluencia hace que la medida sea inestable después de un tiempo, esto está muy bien documentado
  * Los fabricantes de células de carga no comunican sobre la deriva de la medida tras 30 minutos de carga ...
  * Habitualmente las basculas con celda de carga implican una tara entre cada medición, y no es posible en el escenario de monitoreo de colmena
  * Comprobamos esto en nuestro primer prototipo usando celdas de carga, fue peor de lo esperado
  * La escala mecánica no está sujeta a este fenómeno de deriva de la medida. Incluso si la estructura se desformara, la medida no cambiaria. 

  
- Porque no dependemos de ninguna parte complicada que debemos subcontratar
  * Esto hace posible mantener el precio bajo
  * Resulta más fácil entender lo que pasa en caso de avería y repararlo si necesario
  * DIY-ers friendly (hágalo usted mismo)

- El principio es básico y antiguo como la antigua Roma
