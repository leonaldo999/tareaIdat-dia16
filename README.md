# [![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1000&color=30F714&background=703BE2BE&center=true&vCenter=true&width=435&lines=Dia+16+Tarea;Sass+CSS;IDAT+frontEnd)](https://git.io/typing-svg)

## Sass

- [](#)
  - [Sass](#sass)
  - [CSS PLANO (DESVENTAJAS)](#css-plano-desventajas)
  - [QUE ES UN PREPROCESADOR](#que-es-un-preprocesador)
  - [SASS (VENTAJAS Y DESVENTAJAS)](#sass-ventajas-y-desventajas)
  - [VARIABLES EN SASS](#variables-en-sass)
    - [Declaración de variables](#declaración-de-variables)
    - [Tipos de variables](#tipos-de-variables)
  - [ANIDAMIENTO (SELECTORES) EN Sass](#anidamiento-selectores-en-sass)
    - [Sintaxis de anidamiento](#sintaxis-de-anidamiento)
    - [Ventajas del anidamiento](#ventajas-del-anidamiento)
  - [ANIDAMIENTO AMPERSAND (\&) EN Sass](#anidamiento-ampersand--en-sass)
    - [Sintaxis de anidamiento con ampersand](#sintaxis-de-anidamiento-con-ampersand)
    - [Ventajas del anidamiento con ampersand](#ventajas-del-anidamiento-con-ampersand)
  - [IMPORTACION (MODULARIDAD) y PARTIAL EN Sass](#importacion-modularidad-y-partial-en-sass)
    - [Sintaxis de importación](#sintaxis-de-importación)
    - [Partial](#partial)
    - [Importación de partials](#importación-de-partials)
    - [Ventajas de la importación y partials](#ventajas-de-la-importación-y-partials)

## CSS PLANO (DESVENTAJAS)

CSS plano, también conocido como CSS vanilla, se refiere al lenguaje de hoja de estilos en cascada (Cascading Style Sheets) convencional, sin utilizar ningún preprocesador como Sass o Less. Es el lenguaje de estilos que se utiliza directamente en los archivos .css y se interpreta directamente por los navegadores web.

```css
/* CSS plano */
body {
  background-color: #242424;
  color: white;
  font-family: Arial, Helvetica, sans-serif;
}
```

[☝️](#sass)

[</br>](html)

## QUE ES UN PREPROCESADOR

En el caso de los lenguajes de estilos como CSS, un preprocesador es un programa que toma un archivo de código CSS escrito en un lenguaje de estilos extendido (como Sass o Less) y lo convierte en un archivo de código CSS estándar que puede ser interpretado por los navegadores web.

>- Ejemplos de preprocesadores
>
>*Sass* y *Less* son preprocesadores de *CSS* que permiten escribir código *CSS* con características avanzadas y luego lo convierten en código CSS estándar.
>
>*Babel* es un preprocesador de *JavaScript* que permite escribir código *JavaScript* con características avanzadas y luego lo convierte en código JavaScript estándar que puede ser ejecutado por los navegadores web.
>

[☝️](#sass)

[</br>](html)

## SASS (VENTAJAS Y DESVENTAJAS)

Sass es un preprocesador de CSS que permite generar hojas de estilo de manera automática. Es un lenguaje de hoja de estilos en cascada que se utiliza para extender las capacidades del CSS convencional . Sass permite utilizar variables, funciones, selectores anidados, herencia y otras características que no están disponibles en CSS convencional. Esto facilita la creación y el mantenimiento de hojas de estilo complejas y reutilizables. Sass se compila en CSS convencional, lo que significa que los navegadores pueden interpretarlo sin problemas. Sass es compatible con la mayoría de los navegadores y se utiliza ampliamente en la industria del desarrollo web.

>### Ventajas de usar Sass
 >
 >1. Reduce el tiempo para crear y mantener el CSS.
 >2. Permite tener una organización modular de los estilos, lo cual es vital para proyectos grandes.
 >3. Proporciona estructuras avanzadas propias de los lenguajes de programación, como variables, listas, funciones y estructuras de control.
 >4. Permite generar distintos tipos de salida, comprimida, normal o minimizada, trabajando tanto en desarrollo como en producción.
 >5. Permite vigilar los ficheros, de tal manera que, si ha habido un cambio en la hoja de estilos, se regenera automáticamente (modo watch).
 >6. Tiene muy pocas dependencias, sobre todo la nueva versión, que es dart-sass.
 >
>### Desventajas de usar Sass
 >
 >1. Hay que aprender a utilizar una nueva herramienta, lo que para algunos supone una desventaja.
 >2. Hay un tiempo de consumo en el proceso de generación o compilación del CSS, sobre todo si es el archivo SCSS es muy grande.
 >3. Tiene una sintaxis más compleja que CSS.

[☝️](#sass)

[</br>](html)

## VARIABLES EN SASS

En Sass, las variables se utilizan para almacenar valores que se pueden reutilizar en diferentes partes del código. Las variables se definen utilizando el símbolo de dólar ($) seguido del nombre de la variable.

### Declaración de variables

Para declarar una variable en Sass, se utiliza la siguiente sintaxis:

```scss
$variable-name: value;
```

**Por ejemplo:**

```scss
$primary-color: #333;
```

- **Uso de variables**

Una vez declarada una variable, se puede utilizar en cualquier parte del código Sass utilizando el símbolo de dólar ($) seguido del nombre de la variable.

```scss
.button {
  background-color: $primary-color;
}
```

- **Ventajas de utilizar variables**

*Las variables en Sass ofrecen varias ventajas, como*:

Reutilización de código: las variables permiten reutilizar valores en diferentes partes del código, lo que reduce la duplicación de código y facilita el mantenimiento.
Flexibilidad: las variables permiten cambiar fácilmente el valor de un estilo en todo el proyecto sin tener que buscar y reemplazar manualmente el valor en cada lugar donde se utiliza.
Legibilidad: las variables mejoran la legibilidad del código, ya que permiten utilizar nombres descriptivos para los valores en lugar de valores literales.

### Tipos de variables

*Sass admite varios tipos de variables, como:*

1. Números: se pueden utilizar para almacenar valores numéricos, como tamaños de fuente o anchuras de bordes.
2. Cadenas: se pueden utilizar para almacenar valores de texto, como nombres de fuentes o colores.
3. Colores: se pueden utilizar para almacenar valores de color, como #333 o rgba(0, 0, 0, 0.5).
4. Booleanos: se pueden utilizar para almacenar valores booleanos, como true o false.
5. Listas: se pueden utilizar para almacenar colecciones de valores, como una lista de fuentes o una lista de anchuras de bordes.

- **Ejemplos de variables**

Aquí hay algunos ejemplos de variables en Sass:

```scss
$primary-color: #333;
$secondary-color: #666;
$font-size: 16px;
$border-width: 1px;
```

[☝️](#sass)

[</br>](html)

## ANIDAMIENTO (SELECTORES) EN Sass

En *Sass*, el anidamiento (también conocido como "nested selectors" en inglés) se refiere a la capacidad de definir selectores dentro de otros selectores. Esto permite crear estilos más organizados y reutilizables.

### Sintaxis de anidamiento

La sintaxis de anidamiento en Sass es similar a la de CSS, pero con una pequeña diferencia. En lugar de escribir cada selector en una línea separada, se pueden anidar selectores dentro de otros selectores utilizando bloques de código indentados.

**Por ejemplo:**

```scss
nav {
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  li {
    display: inline-block;
  }
  a {
    color: #333;
    text-decoration: none;
  }
}
```

>En este ejemplo, el selector nav contiene tres selectores anidados: ul, li y a. Cada selector anidado hereda el contexto del selector padre.

### Ventajas del anidamiento

*El anidamiento en Sass ofrece varias ventajas, como:*

1. **Organización**: el anidamiento permite organizar los estilos de manera lógica y jerárquica, lo que facilita la lectura y el mantenimiento del código.
2. **Reutilización**: los selectores anidados pueden ser reutilizados en diferentes partes del proyecto, lo que reduce la duplicación de código.
3. **Legibilidad**: el anidamiento mejora la legibilidad del código, ya que los selectores anidados se presentan de manera clara y organizada.

- **Ejemplos de anidamiento**

```scss
.header {
  background-color: #333;
  .logo {
    font-size: 24px;
    color: #fff;
  }
  .nav {
    ul {
      list-style: none;
      margin: 0;
      padding: 0;
    }
    li {
      display: inline-block;
    }
  }
}
```

>- En este ejemplo, el selector *.header* contiene dos selectores anidados: *.logo* y *.nav*.
>- El selector *.nav* a su vez contiene dos selectores anidados: ul y li.

[☝️](#sass)

[</br>](html)

## ANIDAMIENTO AMPERSAND (&) EN Sass

En Sass, el anidamiento con ampersand (&) es una forma de anidar selectores que permite referirse al selector padre desde un selector anidado.

### Sintaxis de anidamiento con ampersand

La sintaxis de anidamiento con ampersand es similar a la de anidamiento normal, pero se utiliza el símbolo de ampersand (&) para referirse al selector padre.

**Por Ejemplo:**

```scss
.button {
  &.primary {
    background-color: #333;
    color: #fff;
  }
  &.secondary {
    background-color: #666;
    color: #fff;
  }
}
```

>- En este ejemplo, el selector .button contiene dos selectores anidados: .primary y .secondary.
>- El ampersand (&) se utiliza para referirse al selector padre .button, lo que permite crear selectores como .button.primary y .button.secondary

### Ventajas del anidamiento con ampersand

*El anidamiento con ampersand en Sass ofrece varias ventajas, como:*

1. **Flexibilidad**: el anidamiento con ampersand permite crear selectores más flexibles y reutilizables.
2. **Legibilidad**: el anidamiento con ampersand mejora la legibilidad del código, ya que los selectores anidados se presentan de manera clara y organizada.
3. **Reutilización**: los selectores anidados con ampersand pueden ser reutilizados en diferentes partes del proyecto, lo que reduce la duplicación de código.

- **Ejemplos de anidamiento con ampersand**

```scss
.header {
  &.fixed {
    position: fixed;
    top: 0;
  }
  &.sticky {
    position: sticky;
    top: 0;
  }
}
```

>- En este ejemplo, el selector .header contiene dos selectores anidados: .fixed y .sticky.
>- El ampersand (&) se utiliza para referirse al selector padre .header, lo que permite crear selectores como .header.fixed y .header.sticky.

[☝️](#sass)

[</br>](html)

## IMPORTACION (MODULARIDAD) y PARTIAL EN Sass

En *Sass*, la importación (también conocida como modularidad) y partial son características que permiten dividir el código en módulos más pequeños y reutilizables.

### Sintaxis de importación

*La sintaxis de importación en Sass es la siguiente:*

```scss
@import 'nombre-del-archivo';
```

*Por ejemplo:*

```scss
@import 'variables';
@import 'mixins';
@import 'estilos';
```

> En este ejemplo, se importan tres archivos Sass individuales: variables, mixins y estilos.

### Partial

*La sintaxis de partial en Sass es la siguiente:*

```scss
// _nombre-del-partial.scss
```

*Por ejemplo:*

```scss
// _variables.scss
$primary-color: #333;
$secondary-color: #666;
```

> En este ejemplo, se crea un partial llamado _variables que contiene dos variables.

### Importación de partials

Para importar un partial en un archivo Sass, se utiliza la directiva @import seguida del nombre del partial.

```scss
@import '_variables';
```

> En este ejemplo, se importa el partial _variables en el archivo actual.

### Ventajas de la importación y partials

**La importación y los partials en Sass ofrecen varias ventajas:**

1. *Organización*: la importación y partials permiten organizar el código de manera más eficiente y reutilizable.
2. *Reutilización*: los partials pueden ser reutilizados en diferentes partes del proyecto, lo que reduce la duplicación de código.
3. *Legibilidad*: la importación y partials mejoran la legibilidad del código, ya que los archivos se presentan de manera clara y organizada.
4. *Mantenimiento*: la importación y partials facilitan el mantenimiento del código,
ya que es más fácil identificar y actualizar los cambios en un solo lugar.
5. *Escalabilidad*: la importación y partials permiten que el proyecto crezca sin que el código se vuelva inmanejable.

[☝️](#sass)

 >Crear un menu de navegacion perfecto
>
1- como componente de scss
>
2- Menu.scss
>
3- html crear la maqueta
<!-- 
- CSS PLANO (DESVENTAJAS)
- QUE ES UN PROCESADOR
- SASS (VENTAJAS)
- VARIABLES
- ANIDAMIENTO (SELECTORES)
- ANIDAMIENTO AMPERSAn(&)
- IMPORTACION (MODULARIDAD)(PARTIAL) -->
