## En línea y en bloque, la propiedad display

Pese a que todos los elementos de mi página HTML son cajas lo cierto es que no todas las cajas se comportan igual cuando las añadimos.

![Modelo de Caja CSS](./img/caja.png)

El comportamiento viene determinado por la propiedad CSS **_display_**.

Cada etiqueta tiene un valor por defecto para esta propiedad pero, para conseguir lo que el diseño que queremos, podremos modificarlas si lo estimamos necesario. Los valores que puede tomar son muchos pero los más usados son:

- **_inline_**
- **_inline-block_**
- **_block_**
- **_none_**
- Valores relacionados con tablas (veremos una lista detellada más abajo).
- Valores **_flex_** y **_grid_** que veremos en próximos cursos de este itinerario.

Si estamos interesados podemos descubrir la lista completa de valora [aquí](https://developer.mozilla.org/es/docs/Web/CSS/display).

### Elementos inline e inline-block

- Los elementos **_inline_** no rompen el flujo de la línea y se van colocando uno detrás de otro mimntras caben. Aceptan _margin_ y _padding_ pero sólo se tienen en cuenta los valores horizontales. Ignoran _width_ y _height_. Ejemplos: _<span>,<img>,<a>, <b>_ etc...

- Los elementos **_inline-block_** funcionan exactamente como los anteriores pero podremos asignarles _width_ y _height_.

### Elementos en bloque

Los elementos en bloque rompen el flujo de la línea y provocan _"un salto de línea"_ tanto anterior como posterior. Por defecto, si no lo especificamos, ocuparán toda la anchura de la etiqueta que los contiene, la etiqueta contenedora. Ejemplos: _<h1>,<p>,<section>,<div>,<li>,<nav>_ etc..

### Elementos con valor none en la propiedad display

Son elementos que desaparecen de la página. No dejan un espacio vacío aunque siguen en el código HTML. La propiedad _visibility:hidden_ sí que se deja ese hueco aunque no se muestre.

### Elementos con valores relativos a tablas en la propiedad display

Al poner uno de estos valores en la propiedad display a una etiqueta HTML esta etiqueta simulará el comportamiento del elemento de tabla análogo. De esta manera tenemos los siguientes posibles valores.

- **_table_**
- **_table-row_**
- **_table-cell_**
- **_table-caption_**
- **_table-column_**
- **_table-colgroup_**
- **_table-header-group_**
- **_table-footer-group_**
- **_table-row-group_**

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
