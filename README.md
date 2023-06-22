# Bienvenido a Pokédex ✨

**Link del Proyecto [Aqui](https://mp-keyner.github.io/Pokemon/)**

Este proyecto se realizo con la finalidas de reforzar y ver nuevos conceptos y tecnicas de **HTML** y **CSS** desarrollado por tu Coach favorito [Keyner de la Hoz](https://github.com/Mp-keyner/)

## **Propiedades de CSS nuevas y que se usan en este proyecto**

> transition **CSS**

- permite controlar cómo se animan los cambios de una propiedad de estilo a otra durante un período de tiempo definido. Proporciona una transición suave y gradual entre los estados de un elemento, lo que mejora la experiencia visual del usuario.

La sintaxis básica de la propiedad `transition` es la siguiente:

```css
transition: <propiedad> <duración> <función-timing> <retraso>;
```

- `<propiedad>` especifica la propiedad o propiedades CSS a las que se aplicará la transición. Puede ser una única propiedad o una lista separada por comas de varias propiedades.

- `<duración>` define la duración de la transición en segundos o milisegundos. Por ejemplo, `0.5s` representa medio segundo y `500ms` representa medio segundo en milisegundos.

- `<función-timing>` establece la función de temporización de la transición, que determina cómo se acelerará o desacelerará la animación a lo largo de su duración. Algunos ejemplos comunes son `ease` (predeterminado), `linear`, `ease-in`, `ease-out`, `ease-in-out`, entre otros. También se pueden utilizar funciones de temporización personalizadas utilizando la notación `cubic-bezier`.

- `<retraso>` (opcional) establece un retraso antes de que comience la transición. Puede ser útil cuando deseas que la transición ocurra después de un cierto período de tiempo.

Por ejemplo, si deseas aplicar una transición suave al color de fondo de un elemento cuando cambia, puedes usar la siguiente regla CSS:

```css
.elemento {
  transition: background-color 0.3s ease;
}
```

Esto hará que cualquier cambio en la propiedad `background-color` del elemento tenga una transición suave con una duración de 0.3 segundos y una función de temporización "ease".

---

> display: grid **CSS**

Se utiliza para crear diseños de cuadrícula flexible y alineada. Permite dividir el espacio disponible en una página o contenedor en filas y columnas, y luego colocar los elementos dentro de esa cuadrícula.

Al utilizar `display: grid`, defines una cuadrícula bidimensional que consta de filas y columnas. Puedes especificar el número de filas y columnas, así como su tamaño y distribución. Los elementos hijos del contenedor se colocan automáticamente en las celdas de la cuadrícula.

La sintaxis básica para utilizar `display: grid` es la siguiente:

```css
.contenedor {
  display: grid;
  grid-template-rows: valor1 valor2 ...;
  grid-template-columns: valor1 valor2 ...;
}
```

- `grid-template-rows` se utiliza para definir el tamaño y la cantidad de filas de la cuadrícula. Puedes especificar los tamaños de las filas utilizando unidades de medida como píxeles (`px`), porcentaje (`%`), fracciones (`fr`), contenido automático (`auto`) u otras unidades.

- `grid-template-columns` se utiliza para definir el tamaño y la cantidad de columnas de la cuadrícula. Al igual que con las filas, puedes especificar los tamaños de las columnas utilizando unidades de medida.

Una vez definida la cuadrícula, puedes colocar los elementos dentro de ella utilizando propiedades adicionales como `grid-row` y `grid-column`. Estas propiedades especifican en qué filas y columnas deben colocarse los elementos.

Además, `display: grid` ofrece otras propiedades para controlar la alineación, el espaciado y el dimensionamiento de las celdas de la cuadrícula, como `grid-gap`, `justify-items`, `align-items`, entre otras.

---

> Position: relative **CSS**

Se utiliza para establecer el posicionamiento relativo de un elemento con respecto a su posición original en el flujo normal del documento.

Cuando se aplica `position: relative;` a un elemento, se crea un nuevo contexto de posicionamiento para ese elemento. Esto significa que el elemento mantendrá su espacio en el flujo normal del documento, pero se puede desplazar utilizando las propiedades de desplazamiento como `top`, `right`, `bottom` y `left`.

Algunas características clave de `position: relative;` son las siguientes:

1. Desplazamiento relativo: Puedes utilizar las propiedades `top`, `right`, `bottom` y `left` para desplazar el elemento relativo a su posición original. Estas propiedades aceptan valores positivos y negativos, lo que te permite mover el elemento en cualquier dirección.

2. Interacción con elementos adyacentes: Aunque el elemento puede ser desplazado, aún ocupará su espacio original en el flujo del documento. Esto significa que los elementos adyacentes seguirán respetando el espacio ocupado por el elemento relativo.

3. Contexto de apilamiento: Cuando se utilizan múltiples elementos con `position: relative;`, se crea un contexto de apilamiento. Los elementos posicionados relativamente se apilan en orden de aparición en el documento. Esto puede afectar cómo se muestran y se superponen entre sí.

Es importante tener en cuenta que `position: relative;` es relativo al flujo normal del documento y no afecta a otros elementos. Si se desea un posicionamiento más preciso o un control de superposición más avanzado, se pueden utilizar otras propiedades de posicionamiento como `absolute` o `fixed`.

---

> position: absolute **CSS**

Se utiliza para establecer el posicionamiento absoluto de un elemento en relación con su elemento padre más cercano que tenga una posición no estática (es decir, con `position` establecido en `relative`, `absolute`, `fixed` o `sticky`).

Cuando se aplica `position: absolute;` a un elemento, se crea un nuevo contexto de posicionamiento para ese elemento, independiente del flujo normal del documento. El elemento se posiciona en función de las propiedades `top`, `right`, `bottom` y `left`, que determinan su posición relativa al elemento padre posicionado.

Algunas características clave de `position: absolute;` son las siguientes:

1. Posicionamiento absoluto: El elemento se retira del flujo normal del documento y se posiciona en relación con su elemento padre posicionado más cercano. No ocupa espacio en el flujo del documento, lo que significa que otros elementos se comportan como si el elemento absoluto no estuviera presente.

2. Desplazamiento preciso: Se pueden utilizar las propiedades `top`, `right`, `bottom` y `left` para especificar las distancias desde los bordes del elemento padre posicionado, lo que permite un control preciso sobre la ubicación del elemento absoluto.

3. Superposición y z-index: Al utilizar `position: absolute;`, se puede controlar la superposición de elementos y su orden de apilamiento mediante la propiedad `z-index`. Un valor mayor de `z-index` coloca un elemento encima de otros elementos con un valor inferior.

Es importante tener en cuenta que `position: absolute;` posiciona un elemento en relación con su elemento padre más cercano con una posición no estática. Si no hay ningún elemento padre posicionado, el elemento absoluto se posicionará en relación con el elemento raíz del documento (`<html>`).

### **Propiedades `Top`, `left`, `right`, `bottom` de CSS**

| Propiedad | Descripción                                                                                                                                                            |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `top`     | Establece la distancia desde la parte superior del elemento al borde superior del elemento padre posicionado. Controla la posición vertical del elemento absoluto.     |
| `left`    | Establece la distancia desde el borde izquierdo del elemento al borde izquierdo del elemento padre posicionado. Controla la posición horizontal del elemento absoluto. |
| `right`   | Establece la distancia desde el borde derecho del elemento al borde derecho del elemento padre posicionado. Controla la posición horizontal del elemento absoluto.     |
| `bottom`  | Establece la distancia desde la parte inferior del elemento al borde inferior del elemento padre posicionado. Controla la posición vertical del elemento absoluto.     |

Estas propiedades se utilizan en conjunto con `position` para definir la ubicación precisa de un elemento en relación con su elemento padre más cercano con una posición no estática.

Aquí tienes un ejemplo de cómo se aplicarían estas propiedades en CSS:

```css
.elemento {
  position: absolute;
  top: 20px;
  left: 30px;
  right: 40px;
  bottom: 50px;
}
```

En este ejemplo, el elemento con la clase "elemento" se posicionará de la siguiente manera:

- Estará 20 píxeles desde la parte superior del elemento padre posicionado.
- Estará 30 píxeles desde el borde izquierdo del elemento padre posicionado.
- Estará 40 píxeles desde el borde derecho del elemento padre posicionado.
- Estará 50 píxeles desde la parte inferior del elemento padre posicionado.

Estas propiedades te permiten controlar la ubicación precisa de un elemento absoluto en tu diseño.

---

> Opacity **CSS**

Se utiliza para controlar la opacidad de un elemento, es decir, la transparencia o visibilidad del contenido. Esta propiedad acepta un valor numérico entre 0 y 1, donde 0 representa la completa transparencia (elemento invisible) y 1 representa la opacidad completa (elemento totalmente visible).

Aquí tienes algunos aspectos importantes sobre la propiedad `opacity`:

- Cuando se aplica la propiedad `opacity` a un elemento, afecta tanto al contenido del elemento como a sus hijos.
- Los valores decimales entre 0 y 1 se utilizan para establecer diferentes niveles de opacidad. Por ejemplo, un valor de `0.5` hará que el elemento y su contenido sean semitransparentes.
- La propiedad `opacity` se hereda por los elementos secundarios, lo que significa que si se establece en un elemento padre, los hijos también heredarán la misma opacidad.
- La opacidad también se aplica a los pseudo-elementos (::before y ::after) y a los elementos de fondo (background).
- Ten en cuenta que la opacidad también afecta a los eventos del elemento y sus hijos. Si un elemento tiene una opacidad menor que 1, es posible que los eventos de clic o interacción no funcionen correctamente.

Aquí tienes un ejemplo de cómo se utiliza la propiedad `opacity` en CSS:

```css
.elemento {
  opacity: 0.7;
}
```

En este caso, el elemento con la clase "elemento" se mostrará con una opacidad del 70%, lo que lo hará parcialmente transparente.

La propiedad `opacity` es útil cuando deseas crear efectos de transparencia, superposición de elementos o animaciones suaves al cambiar la opacidad gradualmente.

---

> scroll-snap-align **CSS**

Se utiliza en combinación con la propiedad `scroll-snap-type` para controlar el comportamiento de desplazamiento suave y el posicionamiento de elementos de desplazamiento en un contenedor con desplazamiento (scroll).

Cuando se aplica `scroll-snap-align: center` a un elemento dentro de un contenedor con desplazamiento, se asegura de que dicho elemento se alinee en el centro del área de desplazamiento visible cuando se realiza un desplazamiento. Esto es especialmente útil cuando se trabaja con un diseño de tipo carrusel o desplazamiento por elementos, donde se desea que los elementos se alineen de forma centralizada al hacer scroll.

Aquí tienes algunos aspectos importantes sobre `scroll-snap-align: center`:

- Esta propiedad solo tiene efecto cuando se utiliza en conjunto con `scroll-snap-type` en el contenedor padre.
- `scroll-snap-align: center` alinea el elemento de desplazamiento en el centro del área visible del contenedor cuando se realiza un desplazamiento.
- Es posible utilizar otros valores para `scroll-snap-align`, como `start`, `end`, `none`, `start [safe | unsafe]`, `end [safe | unsafe]`, etc., para controlar diferentes formas de alineación y comportamiento de desplazamiento.
- La propiedad `scroll-snap-align` se aplica a cada elemento que se desea controlar en el contenedor de desplazamiento individualmente.

Aquí tienes un ejemplo de cómo se utiliza `scroll-snap-align: center` en CSS:

```css
.contenedor-scroll {
  scroll-snap-type: x mandatory;
  overflow-x: scroll;
}

.elemento-scroll {
  scroll-snap-align: center;
}
```

En este caso, se tiene un contenedor con la clase "contenedor-scroll" que tiene desplazamiento horizontal habilitado utilizando `scroll-snap-type`. Los elementos dentro de este contenedor con la clase "elemento-scroll" se alinearán en el centro del área visible del contenedor cuando se realice un desplazamiento horizontal, gracias a `scroll-snap-align: center`.

---

> @keyframes **CSS**

Se utiliza para definir animaciones personalizadas y especificar cómo deben cambiar los estilos de un elemento a lo largo del tiempo.

Con `@keyframes`, puedes establecer varios puntos clave (keyframes) que representan los diferentes estados de la animación en distintos momentos durante su reproducción. Cada punto clave se define con un porcentaje que indica el progreso de la animación en ese momento específico.

La sintaxis básica de `@keyframes` es la siguiente:

```css
@keyframes animationName {
  keyframe1 {
    /* Estilos en el primer keyframe */
  }
  keyframe2 {
    /* Estilos en el segundo keyframe */
  }
  /* ... */
}
```

Dentro de cada keyframe, puedes especificar los estilos que deseas aplicar al elemento en ese punto de la animación. Por ejemplo, puedes cambiar la posición, el tamaño, el color u otras propiedades de estilo.

Luego, puedes aplicar la animación a un elemento utilizando la propiedad `animation` en CSS. Por ejemplo:

```css
.element {
  animation: animationName duration timing-function delay iteration-count
    direction;
}
```

Donde `animationName` es el nombre que le has dado a la animación con `@keyframes`. Los valores `duration`, `timing-function`, `delay`, `iteration-count` y `direction` son opcionales y controlan aspectos como la duración de la animación, la función de temporización, el retraso antes de que comience, el número de repeticiones y la dirección de reproducción.

---

> ::-webkit-scrollbar y ::-webkit-scrollbar-thumb **CSS**

Son pseudo-elementos de CSS utilizados para personalizar la apariencia de las barras de desplazamiento en los navegadores web basados en WebKit, como Google Chrome y Safari.

`::-webkit-scrollbar` se aplica al elemento contenedor de la barra de desplazamiento y se utiliza para establecer estilos generales, como el color de fondo, el tamaño y la forma de la barra de desplazamiento.

Por ejemplo, puedes utilizar `::-webkit-scrollbar` para establecer un color de fondo personalizado para la barra de desplazamiento:

```css
::-webkit-scrollbar {
  background-color: #f1f1f1;
}
```

`::-webkit-scrollbar-thumb` se aplica a la perilla o manija de la barra de desplazamiento y se utiliza para definir los estilos específicos de la perilla, como el color, la forma y el tamaño.

Por ejemplo, puedes utilizar `::-webkit-scrollbar-thumb` para establecer un color personalizado para la perilla de la barra de desplazamiento:

```css
::-webkit-scrollbar-thumb {
  background-color: #888;
}
```

Además, también puedes establecer propiedades como `border-radius` para dar forma a la perilla de la barra de desplazamiento:

```css
::-webkit-scrollbar-thumb {
  background-color: #888;
  border-radius: 8px;
}
```

Estos pseudo-elementos son específicos de los navegadores basados en WebKit y pueden no ser compatibles con otros navegadores. Es posible que sea necesario utilizar prefijos de proveedores adicionales para lograr la compatibilidad en algunos casos.

**`Recuerda que estos pseudo-elementos solo afectarán la apariencia de las barras de desplazamiento en los navegadores compatibles con WebKit y pueden variar según la versión del navegador.`**

## Colores usados en el proyecto

---

| Color      | #Hexadecimal |
| ---------- | ------------ |
| Primario   | #232323      |
| Secundario | #616161      |
| Agua       | #428bbb      |
| Fuego      | #f37823      |
| Fantasma   | #79609f      |
| Bicho      | #709c3e      |
| Planta     | #9acb50      |
| Hada       | #fdb9e9      |
| Psíquico   | #f366b9      |
| Eléctrico  | #eed535      |

---

# **[Aqui encontraras las imagenes necesarias](https://drive.google.com/drive/folders/1_DI0TlUgw_Vti2a2JXvoUeE1VsfcHrYn?usp=sharing)**

Desarrollado por [Steam Academy](https://www.steamacademy.com.co/) bajo la supervición de [Keyner de la hoz ](https://github.com/Mp-keyner/)
