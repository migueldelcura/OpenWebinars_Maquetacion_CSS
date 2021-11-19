## Posicionando Elementos. La propiedad position

En apartados anteriores de este mismo curso hemos visto como se comportaban las etiquetas HTML, a nivel de diseño y estructura, cuando eran mostradas en el navegador.

Conforme vayamos aprendiendo querremos hacer diseños más complejos y mover los elementos con respecto a dónde les correspondería según el flujo normal atendiendo a su propiedad display.

Para este posicionamiento más exacto y concreto CSS nos proporciona la propiedad **_position_** cuyo valores van intimamente asociados a las propiedades CSS **_top_**,**_bottom_**, **_left_**, **_right_** y **_z-index_**. Las 4 primera de estas propiedades indicar desplazamientos conforme a un punto de referencia en concreto y la propiedad **_z-index_** nos va a permitir trabajar con capas:

Los distintos valores que puede tomar esta propiedad son:

- **_static:_** Es es valor por defecto. El elemento sigue el flujo que lo que corresponde. Aunque use top,bottom,left,right o z-index al elemento no se aplica ningún desplazamiento.
- **_relative:_** Es como _static_ pero si atiende a los desplazamiento expresados en top,bottom,left,right o z-index.
- **_fixed:_** Se le aplica top,bottom,right o z-index en relación al documento. No atiende al scroll una vez generada por lo que su posición siempre permanece fija.
- **_absolute:_** Se comporta como fixed pero en relación a la primera etiqueta padre que tenga _position:relative_.
- **_sticky:_** Se comporta como _relative_ hasta llegar a una posición de scroll y a partir de entonces _fixed_.

### La propiedad z-index

Al posicionar los elementos con las propiedad **_position_** puede suceder que nos encontremos que haya elementos que lleguen a solaparse por tener que ocupar la misma área.

Con z-index podemos establecer capas decidienco el orden de solapamiento de estos elementos. Se mostrará arriba del todo aquel elemento de los que se solapen con el mayor valor de z-index.

### Centrado vetical de elementos de bloque

Una vez ya sabemos usar la propiedad position podemos centrar verticalemente elementos de bloque. Nos encontraremos con dos casos:

- Cuando conocemos la altura del elemento.
- Cuando desconocemos la altura del elemento.

Si conocemos la altura del elemento y esta es por ejemplo 150px;

```css {
.contenedor {
  position: relative;
}

.elemento_a_centrar {
  height: 150px;
  margin-top: -75px; /** La mitad de la altura **/
  position: absolute;
  top: 50%;
}
```

Si desconocemos al altura del elemento:

```css
.contenedor {
  position: relative;
}
.elemento_a_centrar {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}
```

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
