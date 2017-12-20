---
title: "mecánica"
bg: green
color: black
fa-icon: cogs
ref: "mechanical"
lang: "es"
---

![romainefleury](img/romaine_larive_fleury_t3_175.png)
### Antigua bascula romana
### Añadimos un motor para poder mover el contrapeso
### Un detector óptico detecta el equilibrio
### Un microcontrolador maneja el sistema y envía los datos...

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

![principle](img/principle.png)

Diseñamos un kit fácil de montar, hecho de perfiles de aluminio y acero inoxidable cortado con láser, unidos principalmente con remaches y tornillería inoxidable. Muy pocas "otras" partes, un motor simple, una correa, un rodamiento linear, un sensor óptico. Eso es.

<div class="icontain">
  <iframe src="https://www.youtube.com/embed/kFrGVwb06q8" allowfullscreen></iframe>
</div>

No se necesita ninguna competencia específica para el ensamblaje.
El mismo nivel de rigor y paciencia que para montar un mueble Ikea será suficiente.

![photo](img/IMGP9335R.jpg)
