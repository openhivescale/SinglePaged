---
title: "mecánica"
bg: green
color: black
fa-icon: cogs
ref: "mechanical"
lang: "es"
---

![romainefleury](img/romaine_larive_fleury_t3_175.png)

Basado sobre el principio de la antigua bascula Romana

Añadimos un motor para poder mover el contrapeso

Un detector óptico detecta el equilibrio

Un microcontrolador maneja el sistema y envía los datos...

-------------- 

## Resolución 6g, precisión 30g de 0 a 125Kg 
(Protocolo de prueba realizado para controlar la linearidad y la repetibilidad en curso de redacción)

-------------- 
## ¿Por qué una balanza mecánica, y no una celda de carga?

- Debido a que la celda de carga no se supone que esté bajo carga continua.
  * Un fenómeno de fluencia hace que la medida sea inestable después de un tiempo, esto está muy bien documentado.
  * Los fabricantes de células de carga no comunican sobre la deriva de la medida tras 30 minutos de carga ...
  * Habitualmente las basculas con celda de carga implican una tara entre cada medición, y no es posible en el escenario de monitoreo de colmena.
  * Comprobamos esto en nuestro primer prototipo usando celdas de carga, fue peor de lo esperado.
  * La escala mecánica no está sujeta a este fenómeno de deriva de la medida. Incluso si la estructura se desformara, la medida no cambiaria. 
  
  
[https://dipot.ulb.ac.be/dspace/bitstream/2013/146415/1/RAM_HBM.pdf](https://dipot.ulb.ac.be/dspace/bitstream/2013/146415/1/RAM_HBM.pdf)

"*Transducer manufacturers provide only information on the short-time stability like maximum creep after 30 minutes or maximum 1 hour under full load, but appear very reticent to provide figures on the long-term stability of their products......*

*Recording strains over long periods of time without having the opportunity to unload the test specimen or the structure and check zero reference is considered to be one of the most difficult applications of strain-gauges....*"

[http://www.analog.com/en/analog-dialogue/articles/a-reference-design-for-weigh-scales.html](http://www.analog.com/en/analog-dialogue/articles/a-reference-design-for-weigh-scales.html)

  
- Porque no dependemos de ninguna parte complicada que debemos subcontratar.
  * Esto permite mantener el costo bajo con una solidez y precisión sin igual.
  * Resulta más fácil entender lo que pasa en caso de avería y repararlo si necesario.
  * DIY-ers friendly (Do it Yourself).

- La electrónica es mucho más sencilla: sin capa analógica de la cual depende la calidad de la medida.

-------------- 

### integración bajo la colmena

A lo contrario de la antigua Romana, nuestra báscula debe integrarze bajo la colmena.
Con un contrapeso de 500g, y muy poco espacio disponible , los varios brazos de palanca permiten medir un peso de 125kg.

![principle](img/principle.png)

Diseñamos un kit fácil de montar, hecho de perfiles de aluminio y acero inoxidable cortado con láser, unidos principalmente con remaches y tornillería inoxidable. Muy pocas "otras" partes, un motor simple, una correa, un rodamiento linear, un sensor óptico. Eso es.

<div class="icontain">
  <iframe src="https://www.youtube.com/embed/kFrGVwb06q8" allowfullscreen></iframe>
</div>

No se necesita ninguna competencia específica para el ensamblaje.
El mismo nivel de rigor y paciencia que para montar un mueble Ikea será suficiente.

![photo](img/IMGP9335R.jpg)

Foto de presentación, la versión comercializada dispone de una caja IP65 para la electrónica y de un capotaje de protección por encima de los brazos de palanca.
