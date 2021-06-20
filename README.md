# Curso de CSS Grid Layout

## Lleva tus conocimientos de CSS a otro nivel

### Tips para llevar tu conocimiento de CSS a otro nivel + Quices

1. No es necesario memorizar todas las propiedades y valores 😊
2. Conoce los conceptos fundamentales 🧠: layour, selectores, responsive, flujo normal, modelo de caja, herencia y cascada, formatting contexts
3. Usar DevTools para encontrar errores y hacer pruebas rápidas 🕷
4. Sabér qué herramientas te sirven para aprender (y cuáles no)

[Repositorio del curso](https://github.com/platzi/CSS2020)

## ¿De dónde venimos y en dónde estamos?

### ¿Cómo fue pensado CSS cuando se creó?

Tim Berners-Lee inventó la W3C y HTML.

Viola fue un navegador que inició en 1993.

- Tenía su porpio lenguaje de estilos.
- Quería convertir su lenguaje en un estándar para la web.

Marc Andreessen en 1998 hizo el navegador NCSA Mosaic.

Hakon Wium Lie propuso 'Cascading HTML Style Sheets' (CHSS).

En 1994 se propuso CSS.

Bert Bos respondió al primer borrador de CSS y unió fuerzas con Hakon y se presentaron en la conferencia de WWW en 1995.

En 1996 nació CSS como recomendación de la W3C.

Los primeros navegadores compatibles con CSS fueron:

1. IE3 (Internet Explorer 3)
2. Netscape
3. Opera

CSS en ese entonces tenía muchas limitaciones y problemas con los elementos flotantes.

### Limitaciones de CSS y el problema de los elementos flotantes

Los primeros diseños de CSS eran una mezcla entre elementoy flotantes y posicionados.

Noodle Incident (Recursos en línea para copiar y pegar).

Había una falta de columnas que nos hiciera más fácil la vida. Incluso se usaban técnicas de columnas falsas.

Ethan Marcotte -> *Responsive Design* 🎇

Los elementos flotantes eran una solución muy limitada 😕

¡Usaron tablas! 😁 ... que terminó siendo muy molesto también 😣

Todos eran trucos muy raros.

### Herramientas que nos han facilitado el camino

- Arquitecturas
- Pre y post procesadores
- Diseño de componentes (Atomic Design)
- Frameworks
- Performance
- Accesibilidad
- Evergreen browsers

## ¿Cómo se llegó al concepto de CSS Grid?

### ¿CSS Grid es una idea nueva? La evolución de la especificación

El diseño de CSS se basó en las revistas de la época.

Rachel Andrew fue una mujer importante en el desarrollo de CSS.

Jen Simmons, una mujer que colocó muhcas demostraciones que creó para CSS Grid en la web.

A partir de 2017 CSS Grid fue añadido por los navegadores, empezando con Google y terminando con Microsoft en Edge.

### ¿Qué significa Grid para CSS?

- [CSS tricks - Grid guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [CSS Reference](https://cssreference.io/)
- [Learn CSS Grid](https://learncssgrid.com/)
- [CSS 3 Generator](https://css3generator.com/)
- [CSS Grid Garden](https://cssgridgarden.com/#es)

Grid ha cambiado complementa la forma de pensar sobre CSS y el diseño.

> No se trata simplemente de agregar propiedades a cada elemento individual. Ahora puedes tener un modelo diferente en el que comienzas con tu diseño priemro y luego incorporas los diferentes elementos en ese diseño. - Bert Bos
---
> Es la herramienta de diseño más poderosa que hemos inventado hasta ahora para CSS. - Atkins
---
> CSS Grid toma todas esas cosas complicadas que tuvimos que hacer para lograr diseños básciso y lo complemetamente innecesario. - Etemad
---
> Estoy entusiasmado con el futuro del diseño CSS. CSS Grid no es el final; en realidad es solo el comienzo. - Whitworth

## Control de alineamiento

### Técnicas de alineamiento antes de CSS Grid: margin y line-height

### Técnicas de alineamiento antes de CSS Grid: table-cell y positions

|Descripción/Position|static|relative|absolute|fixed|
|--------------------|------|--------|--------|-----|
Posicionado de acuerdo al flujo normal|✔|✔|❌|❌|
|Su posición final la determinan top, right, bottom y left|❌|✔|✔|✔|
|Crea un nuevo contexto de apilamiento|❌|✔|✔|✔|

`z-index != auto` -> relative y absolute

### Técnicas de alineamiento de CSS Grid: pros y contras

No hay una propiedad específica para alinear elementos en CSS2, eran "trucos de magia".

- margin
  - Ventaja: El valor *autro* alinea horizontalmente cualquier elemento con cualquier ancho.
  - Desventaja: Alinear verticalmente, ya que, en cada caso, deberán calcularse estos valores.
- line-height
  - Ventaja: Correcta alineación.
  - Desventaja: Si el texto ocupa más de una línea el elemento toma un alto más grande que lo necesario para los cálculos.
- table-cell
  - Ventaja: La alineación vertical no está condicionada por fuentes, tamaños de fuentes o alturas de línea.
  - Desventaja: vertical-align se aplica sólo a elementos Inline.

[Wextensible - Para ver cómo se hacían antes las alineaciones en el antiguo CSS](https://www.wextensible.com/)

Olvidemos las propiedades físicas (margin, padding, etc) y mejor empecemos a pensar en propiedades lógicas.

### Modos de escritura y ejes de alineamiento + Reto

[CSS Direction](https://developer.mozilla.org/es/docs/Web/CSS/direction)

`direction: [ ltr | rtl | inherit ]`

[Writing mode](https://developer.mozilla.org/es/docs/Web/CSS/writing-mode)

### Propiedades físicas y lógicas en CSS + Quiz

[Slides de propiedades físicas y lógicas en CSS](https://www.canva.com/design/DAEPwadrvmg/ldmhPG0L9qzRRhjTaYO9KQ/view?utm_content=DAEPwadrvmg&amp;utm_campaign=designshare&amp;utm_medium=link&amp;utm_source=sharebutton)

### Técnicas de alineamiento con Flexbox

### Dibujemos con CSS + Reto

[A single div](https://a.singlediv.com/)

## Conceptos generales para comenzar a trabajar con CSS Grid

### Grid y las relaciones padre e hijos inmediatos + Quíz

Debemos tener bien estructurado el HTML para poder manejarlo correctamente desde CSS.

### Lines, tracks, cell, area, gutters, grid axis, grid row, grid column + Reto

### ¡Iniciemos nuestro proyecto! Fase de creatividad e identificación de elementos

- Temáticas: Star wars
- Figuras: Cuadros
- Imágenes: Star Wars
- Fuente: google fonts
- Paleta de colores: coolors

## Propiedades y valores para el elemento padre

### Creando nuestro contenedor: ¿display: grid o display: inline-grid?

Display define el tipo de visualización de un elemento

A tomar en cuenta: valores *internos* y valores *externos*

Caundo dices **Display:Grid** lo que realmente estás diciendo es **Display:Block Grid** (en el nivel externo, pero interno es grid)

En CSS3 se agregaron nuevos displays:

- flex
- inline-flex
- grid
- inline-grid

### Creando filas, columnas y espaciado + Reto

### Funciones: repeat(), minmax() y fit-content() + Quíz

```css
.container {
  display: grid;
  /*grid-template-columns: 1fr 1fr 1fr;*/
  grid-template-columns: repeat(3, 1fr); /*Better*/
  grid-template-columns: repeat(3, minmax(200px, 300x)); /*Indicates the minimum and maximum size of the cards inside the container*/
}
```

## Propiedades y valores para los elementos hijos

### ¡Manos al código! Construcción del proyecto

### Alineameinto en los elementos hijos + Quiz

- justify-self (row axis)
- align-self (column axis)
- place-self (align-self / justify-self)

### ¡Manos al código! Fase de ubicación y alineamiento

### Continuando con la fase de ubicación y alineamiento

## Lo que podemos lograr adicionalmente con CSS Grid

### Responsive y CSS Grid
