## Columnas

Usando CSS podemos dividir el contenido que queremos mostrar en varias columnas tal y como podemos ver en un periódico.

Para ello utilizaremos las siguiente propiedades CSS:

- **_column-count:_** para especificar el número de columnas que tendrá el elemento contenedor.
- **_column-width:_** si queremos fijar en ancho de las columnas del contenedor. El navegador calculará cuántas columnas al menos caben con ese ancho.
- **_column-gap:_** permite establecer la distancia que separa las distintas columnas.
- **_colum-rule:_** funciona de manera muy similar a borde y me permite especificar el estilo, color y anchura de la línea que separa las columnas.
- **_column-span:_** con valores _all_ o _none_ para indicar si el elemento en cuestión, que estará dentro del contenedor donde hemos especificado que habrá columnas, sigue el flujo en columnas o no.
- **_column-fill:_** para establecer cómo se rellenan las columnas. El contenedor debe tener altura. Los valore son _auto_ o _balance_ (todas las columnas la misma altura)
- **_break-inside:_** con valor _void_ si queremos que el elemento no quede roto de una columna a otra.

Podemos ver varios ejemplos en esta misma carpeta del repositorio.

**NOTA:** No todas estas propiedades son válidas en todos los navegadores.

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
