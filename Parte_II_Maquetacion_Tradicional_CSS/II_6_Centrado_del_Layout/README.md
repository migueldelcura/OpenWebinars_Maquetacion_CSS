## Centrado del Layout

En muchas ocasiones cuando estamos maquetando queremos centrar algo para que todo encaje. Centramos toda la página, un texto de un título, una imagen en unas sección etc...

Al principio, esta actividad de centrar es algo que se atraganta a los que están aprendiendo HTML y CSS.

En este apartado y en alguno de los siguiente vamos a dar unas pocas pautas generales que, una vez aprendidas, harán que todo esto de centrar sea mucho más fácil.

Para centrar vamos a diferenciar entre:

- El centrado en horizontal, que yo creo que es el más importante.
- El centrado en vertical.

### Centrado en horizontal

Para centrar los elementos en horizontal:

- Si queremos centrar elementos en línea añadiremos la propiedad **_text-align:center_** al contenedor padre.

* Si queremos centrar un elemento en bloque dentro de su etiqueta contenedora añadiremos la propiedad CSS **_margin: X auto_** al elemento que queremos centrar (X es una distancia expresada en cualquier unidad). El elemento debe tener anchura.

- Si tenemos varios elementos en bloque dentro de un contenedor deberemos
  - Añadir la propiedad **_text-align:center_** al contenedor padre.
  - Añadir la propiedad **_display:inline-block_** a los elementos a centrar.

* Usaremos contenedores **flex** aunque este tipo de contenedores no es objeto de este curso.

### Centrado en vertical

#### Centrado vertical para elementos en línea:

Se puede conseguir:

- Con el mismo **_padding_** arriba y abajo.
- Añadiendo **_vertical-align:middle_** si estamos dentro de una celda de una tabla o lo estamos simulando con la propiedad display (ya hemos hablado en otros apartados de esto).
- Con contenedores **flex** (en cursos posteriores).

### Centrado vertical para elementos en bloque:

Se puede conseguir:

- Utilizando la propiedad **_position_** en el contenedor y en el elemento (lo veremos en el próximo apartado).
- Con contenedores **flex** (en cursos posteriores).

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
