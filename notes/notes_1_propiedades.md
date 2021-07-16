---
title: "Curso frontend developer - platzi"
day: "1"
publishDate: "2021-06-19"
thumbnailImage: ""
shareText: " Description:  "
hashtags: ['learn', 'frontend', 'html', 'css']
draft: false

---

## Funciones de las propiedades CSS más usadas

| Source:      | [URL Platzi](https://platzi.com/clases/1640-frontend-developer/) |
| ------------ | ------------------------------------------------------------ |
| **Course:**  | Curso frontend developer - platzi                            |
| **Teacher:** | Estefany Agilar                                              |



**width**: Define el ancho de un elemento. Por ejemplo: `width: 20px;`.

**height**: Define el alto de un elemento. Por ejemplo: `height: 20px;`.

------

**background**: Puede definir el color de fondo o la url de fondo de un elemento. Por ejemplo: `background: url(';puppy.png';);`.

**background-color**: Define el color de fondo de un elemento. Por ejemplo: `background-color: red;`.

**color**: Define el color de nuestros textos. Estos colores los podemos escribir de 3 formas en CSS:

- Con los **nombres de los colores**. Por ejemplo: black, red, green.
- **Sistema hexadecimal**: Donde blanco se define como `#FFFFFF` y negro como `#000000`. Una página que me gusta mucho para sacar colores en hexadecimal es [colorhunt.co](https://colorhunt.co/).
- **RGB**: Donde la R significa Red, G significa Green y B significa Blue; por lo que escribimos rgb(red, green, blue) y cada uno de ellos es un valor de 0 a 255 que describe la intensidad de ese color. Por ejemplo, para denotar el color verde, escribimos: rgb(0, 255, 0). También a estos valores se les puede agregar una opacidad (transparencia) que va de 0 a 1, por ejemplo: rgba(0, 255, 0, 0.5) lo que quiere decir que el color verde lo queremos con una transparencia del 50%.

------

**border**: Define el tamaño, estilo y color del borde de un elemento. Por ejemplo: `border: 2px solid yellow;`.

**border-radius**: Define qué tan redondeado quiero mi elemento. Por ejemplo: `border-radius: 20px;`.

------

**margin**: Define la margen de un elemento. Por ejemplo: `margin: 2px` (lo que quiere decir que mi elemento tendrá márgenes en todos sus lados de 2px).

Si quiero que mi elemento tenga margen superior de 2px, margen inferior de 4px, margen derecha de 3px y margen izquierda de 5px, lo escribiría de la siguiente forma: `margin: 2px 3px 4px 5px`. El primer valor es la margen superior y siempre va en sentido de las manecillas del reloj.

Si solo quiero que mi elemento tenga una margen a la derecha de 10px, escribiría `margin-right: 10px;`. Y para los demás valores sería `margin-top: 10px;` para la margen superior, `margin-bottom: 10px;` para la margen inferior y `margin-left: 10px;` para la margen izquierda.

**padding**: Define la distancia del borde de un elemento hasta su contenido. Por ejemplo: `padding: 2px` (lo que quiere decir que mi elemento tendrá un “margen interno” en todos sus lados de 2px).

Si quiero que mi elemento tenga padding superior de 2px, padding inferior de 4px, padding a la derecha de 3px y un padding a la izquierda de 5px, lo escribiría de la siguiente forma: `padding: 2px 3px 4px 5px`. El primer valor es la padding superior y siempre va en sentido de las manecillas del reloj al igual que con las márgenes.

Si solo quiero que mi elemento tenga un padding a la derecha de 10px, escribiría: `padding-right: 10px;`. Y para los demás valores sería `padding-top: 10px;` para la margen superior, `padding-bottom: 10px;` para la margen inferior y `padding-left: 10px;` para la margen izquierda.

------

**font-size**: Define el tamaño de la fuente. Por ejemplo: `font-size: 20px;`.

**font-family**: Define la familia tipográfica de la fuente. Por ejemplo: `font-family: 'Roboto', sans-serif;`.

Una página de fuentes que me gusta mucho es [fonts.google.com](https://fonts.google.com/).

------

**opacity**: Determina la transparencia del elemento. Tiene valores entre 0 y 1, que pueden verse como un porcentaje. Por ejemplo, si quiero que mi elemento se vea con una transparencia del 50%, escribiría: `opacity: 0.5;`.

**outline**: Un término algo desconocido es el esquema de los elementos HTML. Un esquema es una línea (por defecto, de color azúl) que se dibuja alrededor de los elementos que hace que se “destaquen”.

Lo anterior sucede mucho en elementos como los <input>s y los <button>s. Si no queremos ver esa línea, lo que hacemos es `outline: none;`. Aunque también podemos decirle que tenga determinado estilo, color, tamaño, entre otras. Por ejemplo:

```css
outline-style: solid;
outline-color: red;
outline-width: 5px;
```

**box-sizing**: Cuando trabajamos con paddings, por ejemplo, veremos que el tamaño de nuestro elemento crece. Es decir, si tengo:

```css
div {
   background: pink;
   width: 20px;
   height: 20px;
}
```

Y luego le agrego un padding de 20px, veré en el navegador que mi `div` ya no tiene un ancho y un alto de `20px`, sino de `40px` cada uno. Lo que quiere decir que el padding hizo que creciera mi elemento. Sin embargo, si yo no quiero que el padding afecte los 20px originales, le agrego la propiedad `box-sizing` para que el tamaño total del elemento incluya el padding también y no se vea afectado por él.

------

**transition**: Las transiciones CSS le permiten cambiar los valores de las propiedades sin problemas durante una duración determinada. Debemos tener presente que una transición NO es una animación. Una transición va de un punto A, a un punto B sin interrupciones o saltos en medio.

Te comparto la siguiente documentación para que puedas visualizar las propiedades y valores que puedes utilizar:

- https://www.w3schools.com/css/css3_transitions.asp.
- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions
- https://css-tricks.com/almanac/properties/t/transition/

**animation**: Esta propiedad permite que animemos nuestros elementos.

Te comparto la siguiente documentación para que puedas visualizar las propiedades y valores que puedes utilizar:

- https://www.w3schools.com/css/css3_animations.asp
- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations
- https://css-tricks.com/almanac/properties/a/animation/



